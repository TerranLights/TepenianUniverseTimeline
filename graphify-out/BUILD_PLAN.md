# graphify build plan — Tepenian Universe Timeline knowledge graph

Adapted from the InnerTepeniaGDD build plan (`../../games/Inner Tepenia/InnerTepeniaGDD/graphify-out/BUILD_PLAN.md`),
scaled down: this repo is 479 files / ~294K words vs. that repo's 2,763 files / ~5.15M words, so this build fits
in a single Phase B checkpoint of 22 chunks instead of 14 checkpoints of ~10 chunks each. Same lessons apply.

**Extraction backend: host subagents.** No `GEMINI_API_KEY`/`GOOGLE_API_KEY` available — user confirmed. The
host agent dispatches `general-purpose` subagents per chunk, per the skill's no-key path. Settled, do not re-raise.

**Corpus:** 479 files (478 document, 1 code) · ~294K words · **22 chunks** (~21-22 files/chunk).

**AST pass:** 0 nodes (the one code file, `settings.local.json`, is not a code-import file — expected, this
corpus is prose/lore).

---

## ⚠ Lesson from InnerTepeniaGDD, confirmed true here too

"Failed: session limit" subagent notifications do NOT mean the agent died — several chunks in this repo's own
build (01, 02, 04-19) reported `status: failed` from a session-limit hit but had **already written valid,
complete JSON to disk** before the notification fired. Confirmed by direct file read after the fact: all 19
chunk files present are well-formed with real node/edge counts. **Before re-dispatching any "failed" chunk,
check the file on disk first** — do not assume failure from the notification alone.

---

## Phase B — semantic extraction

Single checkpoint, all 22 chunks, dispatched in one large wave (small corpus, low risk vs. InnerTepeniaGDD's
wave-of-5 caution which was for 10-chunk checkpoints).

| Chunk | Status | Nodes | Edges |
|---|---|---|---|
| 01 | [x] done | 100 | 136 |
| 02 | [x] done | 71 | 84 |
| 03 | [x] done | 70 | 71 |
| 04 | [x] done | 38 | 62 |
| 05 | [x] done | 52 | 95 |
| 06 | [x] done | 121 | 132 |
| 07 | [x] done | 33 | 44 |
| 08 | [x] done | 37 | 46 |
| 09 | [x] done | 38 | 27 |
| 10 | [x] done | 47 | 53 |
| 11 | [x] done | 25 | 23 |
| 12 | [x] done | 49 | 61 |
| 13 | [x] done | 23 | 33 |
| 14 | [x] done | 37 | 51 |
| 15 | [x] done | 38 | 57 |
| 16 | [x] done | 22 | 23 |
| 17 | [x] done | 46 | 67 |
| 18 | [x] done | 40 | 44 |
| 19 | [x] done | 39 | 65 |
| 20 | [x] done | 49 | 51 |
| 21 | [x] done | — | — (template stubs only) |
| 22 | [x] done | 17 | — (template stubs only) |

**Phase B complete.** All 22 chunks written to disk and validated. Next: Phase C.

---

## Phase C — build the graph (cheap, gated on Phase B)

- [x] **C1 — Merge all 22 chunk JSONs** into `.graphify_semantic.json`. Done: 1019 nodes, 1267 edges, 64
      hyperedges (pre-dedup).
- [x] **C2 — Merge semantic + AST → `.graphify_extract.json`** (AST is 0/0, passthrough). Done: 1008 unique
      nodes (1019 − 11 duplicate-ID collapses), 1267 edges.
- [x] **C3 — Build, cluster, analyze → `graph.json`, `GRAPH_REPORT.md`** (skill Step 4). Done: 1008 nodes,
      1250 edges, 76 communities.
- [x] **C4 — Graph health check** (skill Step 4.5, read-only). Warning fired (4 directed-collapsed,
      17 undirected-collapsed edges) but `post_build_edges` (1250) matches `graph.json` exactly — expected
      multigraph→simple-graph dedup, not data loss. No action needed.
- [x] **C5 — Label communities** (skill Step 5). Hand-labeled all 76 communities from their real highest-degree
      node content (not mechanically derived) — small enough corpus to do meaningfully. `.graphify_labels.json`
      written; `GRAPH_REPORT.md` and `graph.json` re-exported with `community_name` populated.
- [x] **C6 — HTML visualization** (skill Step 6). 1008 nodes, well under the 5,000-node threshold — full
      per-node rendering. `graphify-out/graph.html` written.
- [x] **C7 — Save manifest, cost tracker, final report** (skill Step 9, intermediates NOT deleted per
      no-delete policy). Done: `manifest.json` and `cost.json` written; all `.graphify_*` intermediates
      confirmed still present alongside `graph.json`, `GRAPH_REPORT.md`, `graph.html`. Token counts read 0/0
      (subagent usage was never backfilled into the merged extraction — known precision gap, not a bug).
      **Phase C complete — the knowledge graph build is done.**

**After C7:** paste God Nodes / Surprising Connections / Suggested Questions from `GRAPH_REPORT.md`, offer to
trace the most interesting question, then set up the InnerTepeniaGDD-style `CLAUDE.md` graphify section and
`.claude/settings.json` hook-guard in this repo.

---

## Log

| Date | Event |
|---|---|
| 2026-08-24 | Corpus detected (479 files), AST run (0/0, expected), cache checked (0/478 hit), 22 file-list chunks written. Dispatched all 22 subagents in one wave. Session limit hit partway through; 19 of 22 chunks (01-19, missing 20-22) confirmed to have written valid JSON to disk despite "failed" notifications — same false-failure pattern as InnerTepeniaGDD. This build plan written to track remaining work: chunks 20-22, then Phase C. |
| 2026-08-24 | Chunk 20 was a genuine failure (never wrote to disk, unlike 01-19's false-failure pattern) — re-dispatched fresh along with 21, 22 (never dispatched). All 3 completed cleanly. Phase B complete: 22/22 chunks on disk, ~1019 nodes / 1267 edges pre-dedup. Ran full Phase C: merged chunks → built graph (1008 nodes, 1250 edges, 76 communities) → health check (clean, expected dedup only) → hand-labeled all 76 communities from real content → HTML export (full per-node, well under 5,000-node threshold) → manifest/cost tracker saved, no intermediates deleted. **Build complete.** |
| 2026-08-24 | `/graphify .` re-invoked (bare-path form, not `--update`). Detect found 481 files (+2: this session's own new `CLAUDE.md` and `.claude/settings.json`, the latter code-type/0-node as expected). graphify's own semantic file-cache was empty (build session wrote merged chunk JSONs directly, never called `save_semantic_cache`) — populated it retroactively from the 22 existing chunk files instead of re-dispatching all 479 files: 429/479 hit immediately. Remaining 50 uncached were the genuinely-thin character Personal_Background stub files plus 2 real gaps (new `CLAUDE.md`, and `Signy.md` which chunk 22's original dispatch had missed). Dispatched 2 small gap-fill subagents (25+24 files) instead of a full 22-chunk rebuild — both completed cleanly, added 80 nodes/66 edges/6 hyperedges, all 50 files now cached (479/479 document files fully cached). Rebuilt graph: 1084 nodes, 1316 edges, 115 communities (up from 1008/1250/76 — new real character content, esp. Salagéa Aparast, Seica Cenilaithe, Elva, Miranda profiles, added real structure). Re-labeled all 115 communities by hand from content. Re-exported HTML (1084 nodes, still well under 5,000 threshold). Manifest/cost saved, no intermediates deleted except the temporary gap-fill chunk files. |
| 2026-09-08 | `graphify update .` run to add new character **Besifa** (`8E51CFAC-B2F0-4E16`, 7 files under `Worldspace/Characters/Dolls/`). `detect_incremental` found 35 changed files total (Besifa's 7 plus 28 files whose manifest hashes had drifted since the last run — likely from intervening edits elsewhere in the repo, not this session). First extraction pass (2 chunks, ~18 files each) produced only 138 nodes for those 35 files vs. 182 the old graph held for the 28 non-Besifa ones alone — the shrink-guard correctly refused to write (`net -112`). Root cause: bundling too many files per subagent caused thin/header-only sampling of large docs, confirmed explicitly by one subagent's own report. Re-dispatched the 28 non-Besifa files in 3 smaller, thoroughness-instructed chunks (9-10 files each) — recovered most of the gap but the single largest file, `Character_Development_Methodology_-_DRAFT_Ideas.md` (3,469 lines / 310KB, exceeds one Read call's cap), still only got 1 node vs. its old 18. Split that file into 2 offset-based Read passes (lines 1-1800, 1800-3469) dispatched as dedicated subagents — recovered 220 nodes from it alone (12x the original 18). Final merge: 1302 nodes, 1392 edges, 284 communities (up from 1084/1316/115) — a net gain despite the update only targeting 35 changed files, because the redo passes were significantly more thorough than the original full-build extraction for those particular files. Graph health clean. Given 92 non-singleton communities (too many for meaningful one-by-one hand-authorship on a routine update), labeled all communities from their real highest-degree node content — an honest, non-placeholder fallback, same approach InnerTepeniaGDD uses at its much larger scale. HTML re-exported (1302 nodes, still well under 5,000). **Lesson for future updates:** when `detect_incremental` flags an oversized file (near/over the Read tool's ~256KB cap) among changed files, split it into offset-based passes proactively rather than waiting for the shrink-guard to catch a thin single-pass extraction. |
