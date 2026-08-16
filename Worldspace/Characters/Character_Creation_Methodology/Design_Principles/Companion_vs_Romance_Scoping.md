# Design Principle — Companion vs. Romance Scoping

**What this is:** a generalized, portable rule for any project that layers an optional romantic-relationship
system on top of a full companion/personal-arc system for the same characters. Relevant only if your project
has both layers; skip entirely if romance (where it exists at all) is just a flag on an otherwise-ordinary
character rather than its own designed system.

**Where this came from:** surfaced while re-checking whether the Pipeline's full five-stage machinery should
be run twice per character — once for her Companion questline, once again for her Romance questline. Comparing
the Pipeline's own tools against a large body of already-built Romance content (one project's own
`Companion_System.md` — 15+ fully-designed romance sequences) showed the two were never actually being built
symmetrically in practice, even though nothing in the Pipeline said so explicitly. This file names that
asymmetry as a rule, so it stops being an implicit habit and starts being a checkable design law.

---

## The Core Claim

**Romance is not a second full pass through Stages 3–5. It is a narrow, targeted extraction from Companion
material already built, plus one small tool of its own.** Running the full pipeline twice — once per layer —
over-builds Romance (which, in every real instance checked, stays deliberately lightweight) and risks
duplicating or drifting from psychology that was already correctly established once, for the Companion arc.

---

## What Romance Draws From Stage 3 (Character Data) — a narrow slice, not a fresh pass

Romance does **not** get its own Ghost, Greatest Fear, Desire/Motive, Want, or Need/Truth. It inherits all of
that from the character's existing Companion-scoped Character Data wholesale. What it *does* draw out,
specifically:

- **Attraction Basis** — what draws her to a partner (physical presence, intelligence, courage, emotional
  depth, perceptiveness, capability — usually more than one), derived from her already-established personality
  and history, not invented in isolation. If a project gates romance behind a stat/trait threshold, this is
  what that threshold should be built from.
- **Dealbreaker** — a specific trait or behavior she wouldn't tolerate in a partner, distinct in kind from a
  threshold: a threshold is something a player can still grow into over a playthrough, a Dealbreaker is a
  permanent disqualifier that can't be worked around once triggered.
- **The Lie/Flaw Romance Sub-Case** — "I can't love him because ___" (see `../Pipeline/03_Character_Data.md`'s
  Lie/Flaw node) — a quick-fill variant scoped specifically to what blocks the internal conflict for a
  romanceable character. This is not a second, separate Lie from her Companion-arc Lie — it's the specific
  angle of the *same* Lie that bears on romantic vulnerability, and should read as obviously downstream of it.
- **Rejection Voice** — how she'd actually turn someone down, in her own voice, honestly, without cruelty — the
  one delivered line that closes the romantic door without closing the relationship.

## What Romance Does NOT Draw From Stage 4 (Story Material)

Explicitly out of scope for Romance, confirmed against real production practice (one project's own
`Companion_System.md` states this outright for the first item below):

- **The Player-Necessity Rule** and its whole apparatus (categorical-block sanity check, compounding-reasons
  technique, no-escort-quest constraint) — Companion-questline only. Romance is not a second problem the player
  solves for her.
- **Contagonist, Impact Character, Revenant, antagonist selection, Four-Corner Opposition** — Companion-
  questline only. Romance is a relationship layered onto a story that already has its own supporting cast and
  opposition; it doesn't need a second one.
- **MICE Quotient / Character Hierarchy** — already resolved once, for the character as a whole. Not re-run for
  the Romance layer specifically.

## What Romance Uses Instead of Stage 5 — The Courtship Sequence

**A new, lightweight tool, distinct from Stage 5's full arc machinery — not a smaller version of the 11-beat
skeleton, a genuinely different shape.**

- **Structure:** a short, numbered sequence of **4 to 6 concrete, character-specific proof-points** — not a
  full arc with its own Ghost, Midpoint, and Climax. Each beat is a specific test, action, or moment ("a
  handful of concrete moments or tests," not time passing) that only makes sense given exactly who *she*
  specifically is.
- **Derivation:** seed every beat directly from the Stage 3 slice above (Attraction Basis + Dealbreaker + the
  Lie/Flaw Romance Sub-Case) — what would it actually take, given her specific wound and what she's drawn to,
  to earn her trust incrementally.
- **The Culminating Beat:** the sequence's last beat is its own small structural turning point — not a grand
  declaration, but a specific, small signal that she's moved from guarded to open. This is doing the functional
  job Stage 5's Midpoint does for a full arc, compressed into one beat inside a much smaller structure — worth
  naming explicitly for that reason, even though the Courtship Sequence never runs the actual Midpoint Menu.
  Convention worth keeping: **she is the one who makes the actual move**, not the player — the sequence builds
  toward her closing the distance, not the reverse.
- **Explicitly not used for a Courtship Sequence:** Arc-Space Enumeration across the five Arc Types, the full
  11-beat skeleton, the Midpoint Menu, the Ending-Shape Cross-Mapping Table, Chiastic Mirroring, the Act 3
  Micro-Sequence. All of that assumes a complete character arc; a Courtship Sequence is deliberately not one.
- **Access-gate logic sits outside the Sequence itself**, if a project has one — a stat/trait check (or
  whatever mechanism a given project uses to determine Romance eligibility at all) is the *unlock condition*
  for the Courtship Sequence as a whole, not part of any individual beat's content.
- **Individual beats may optionally carry their own mechanical check** — this is a genuinely different thing
  from the access gate above, and, where a project's own design laws require multiple ways to pass any given
  check (a "minimum solutions" rule, if your project has one — see the Core Design Law this pattern is built
  on top of in one project's own concrete elaboration, below), a single beat-level check should draw from
  *multiple, categorically distinct* qualifying routes rather than one stat threshold alone — the same
  discipline the rest of this methodology already applies to a Companion arc's own player-unique task, scoped
  down to one beat instead of a whole arc. **Worked example, real and binding in one project:** one project's
  own `Companion_System.md` codifies this as up to six category types per beat (skills, non-disqualifying
  traits, perks, non-disqualifying core stats, in-world knowledge gained by any means, and district reputation
  status), each with its own minimum/ideal route count, plus a standing rule that difficulty should escalate
  *noticeably but not brutally* from one beat to the next, culminating in the sequence's hardest check at its
  final, structurally-heaviest beat. Not every project needs this much mechanical weight per beat — a purely
  narrative Courtship Sequence (no checks at all) remains the lighter-weight default this tool was designed
  around — but where a project wants Romance beats to carry real mechanical stakes, this is a concrete,
  battle-tested shape for doing it without breaking the Sequence's own lightweight identity.

## The One Real Interdependency Stage 5 Doesn't Model on Its Own

If a project makes Romance's very availability conditional on the Companion arc's own resolution (e.g., a
negative Companion ending permanently disqualifying Romance regardless of an otherwise-eligible build), that's
a genuine cross-system dependency. Stage 5's Ending-Shape Cross-Mapping Table treats each character's arc
atomically and has no slot for this — it has to be tracked as an explicit, separate project-specific rule
layered on top, not forced into the table itself. Don't let the absence of a slot for it read as "this doesn't
need tracking" — it's a real design law, just one that lives outside Stage 5's own machinery.

## Correspondence to the Fill-In Template

`../Templates/Companion_and_Romance_Questline_Fill-In_Sheet_Template.md`'s Part B (B1–B5) is exactly the raw
intake for everything above: B1 → Attraction Basis, B2 → Dealbreaker, B3 → Rejection Voice, B4 → the Courtship
Sequence's own beats, B5 → any project-specific exception to the standard system. This Design Principle is, in
effect, the "how to turn Part B's answers into a finished Romance design" instructions the template itself
intentionally leaves implicit (per the template's own stated philosophy: it asks for raw material, not
finished conclusions).

## Summary Table

| | Companion Questline | Romance (Courtship Sequence) |
|---|---|---|
| Stage 3 draw | Full core cluster (Ghost, Fear, Lie, Desire, Want, Truth) | Narrow slice only (Attraction Basis, Dealbreaker, Lie sub-case, Rejection Voice) |
| Stage 4 tools | Full (Player-Necessity Rule, Contagonist, Impact Character/Revenant, antagonist, Four-Corner Opposition) | None — inherits the story already built |
| Stage 5 structure | Full 11-beat arc, Arc-Space Enumeration, Midpoint Menu, Ending-Shape table | The Courtship Sequence only (4-6 beats + one culminating turning-point beat) |
| Ending law | No Good Endings' full distribution, own Arc Type | No Good Endings still applies, but availability may be conditioned on the Companion arc's own resolution — track as a separate rule |
