# Character Development Methodology — 00a: Initial Input

**Purpose:** a minimal-field intake layer sitting in front of Stage 1 (`01_Input_Information.md`), built for
use at scale — the originating project needed this to register a cast in the thousands. Manually filling in
Stage 1's full field set (Section A's necessary categories plus Section B's optional ones) by hand, per
character, at any real scale isn't viable for one developer working alone. This file is the compression layer:
the smallest set of fields a developer actually has to provide, paired with a **Derivation Protocol**
describing exactly how the rest of Stage 1 — both necessary and optional fields — gets reconstructed from them.

**`00b_Clarification_Protocol.md`** sits alongside this file — it's the repeatable algorithm for resolving
whatever this Derivation Protocol leaves genuinely ambiguous for a specific character, without falling back
into a full manual review pass per character.

---

## The Story-Format Gate — Linear or Non-Linear, Decided Once

Not a per-character seed field — a project-level (or story-level) gate-check, answered once, before any
character intake begins, since it changes how Stage 5's Arc-Space Enumeration tool resolves its output for
every character processed afterward (see `05_Beats_Paths_Results.md`).

**The question:** is the finished work a given character is being built for a fixed, single telling (a novel,
a film, a closed short story, a linear campaign, or any other format where the audience experiences one
sequence of events with no branching) — or a non-linear/branching work (a game, an interactive story, any
format where the audience's own choices determine which version of events actually happens)?

- **Linear** → downstream, Stage 5's Arc-Space Enumeration tool collapses its full generated set of candidate
  arcs down to the single strongest fit before any content gets built out in detail.
- **Non-linear** → Stage 5's Arc-Space Enumeration tool keeps its surviving candidates as genuinely separate,
  mutually exclusive in-fiction branches (via `../Design_Principles/Dual_Outcome_Branching.md`), rather than
  collapsing to one.

**Default and override:** answered once per project, reused automatically for every character processed
afterward — the same one-time-cost pattern already established below for the writer's Memory Mining priming
answers. A specific character can still be flagged as an exception to the project's own default (a strictly
linear cutscene-only character inside an otherwise branching game, or vice versa) — note the override
explicitly on that one character's intake rather than re-asking the question generally.

**If genuinely unclear or mixed:** default to non-linear/no-collapse. Keeping more candidate arcs alive costs
nothing but a little extra design documentation, while collapsing prematurely on a project that turns out to
want branching content later means real, already-discarded design work has to be reconstructed. See
`00b_Clarification_Protocol.md` if this needs to be surfaced as an actual clarification question rather than
defaulted.

---

## Why the Full Stage 1 Field Set Doesn't Actually Need a Full Manual Answer Per Character

Three things make aggressive compression possible, found by re-checking every one of Stage 1's categories
against what's actually irreducible:

1. **Existing character-folder materials already answer most of the foundational-identity, biographical,
   mechanical-data, introduction-context, and relationship-web categories** for any character who already has
   a folder — reference art, any existing notes, any existing mechanical data. These don't need to be retyped
   into a form; they need a **pointer**, and this methodology (or whoever is applying it) reads them directly.
2. **The writer's own priming answers for the Memory Mining tool (Stage 2) are a one-time setup cost, not a
   per-character field.** The self-pass — happiest memory, saddest memory, a time of shame, a belief that
   creates conflict, a time of being hurt — is the *same* baseline used to prime every character's Memory
   Mining pass. It should be gathered once, ever, not re-asked for every character in a large cast. Not
   requested below; flagged as a one-time exercise to do separately, whenever convenient, outside this
   per-character intake.
3. **Several Stage 1 categories are genuinely not needed at initial registration.** Introduction-scene context,
   the full relationship web beyond what a folder already shows, and existing arc/ending concepts are
   Stage 4/5-territory that only matters once a *specific* character's full arc is actually being built — not
   while bulk-registering a whole cast. These stay deliberately deferred (marked TBD) at this stage, filled in
   properly later, per-character, when her actual development turn comes.

What's left, after removing all of the above, is a genuinely small irreducible core: facts that can only come
from the developer's own head, because no amount of reading existing files or applying setting canon could
produce them.

---

## The Minimal Seed Fields

**The first three fields are the ones that actually matter. The rest have an explicit "you decide" escape
hatch — the developer is not required to answer them if there's no strong existing preference.**

1. **Name (or character-folder identifier).** If she already has a named folder, this is just confirming which
   one.
2. **Character-folder path or pointer to existing materials, if any exist.** This single field is doing the
   most compression work in the whole intake — if a folder exists, its reference art, any existing notes, any
   partially-filled surface/mechanical spec sheet (see `../Templates/`), and any prior design fragments all
   become directly readable, covering large parts of Stage 1 without the developer restating any of it.
3. **A vision statement — whatever's already in your head about her, in whatever form it's already in.** One
   line, one paragraph, a mood, a single defining trait, a "she's basically X but Y" comparison — doesn't need
   to be complete, organized, or even fully coherent. **This is the single highest-leverage field in this
   entire intake.** A short, rough description reliably implies a great deal of downstream material (a
   personality shape, a plausible personality-type cluster, a likely relationship to whatever this setting's
   own defining historical event is, a likely emotional register) that the Derivation Protocol below expands
   outward from, the same way Stage 2's Why Chain tool expands a stated Want into its underlying Desire. Give
   as much or as little as actually exists — "she's a bitter ex-soldier who never talks about her old unit" is
   already enough to seed several Stage 1 categories at once.
4. **Core nature or type, if the setting has more than one kind of being** (human, robot, alien, spirit,
   whatever ontology the target setting actually uses) **and it isn't already obvious from the folder.**
   Skippable entirely if the setting only has one kind of being, or if field 2 already makes this clear.
5. **A personality-typing assignment, if already decided.** This system was built around the Enneagram (see
   the sibling `../Enneagram/` folder for the full reference material) — any well-grounded typology could
   substitute, but the rest of this Pipeline assumes something in that shape. Explicit permission to say "you
   decide" — if so, one gets proposed from field 3 and any reference art, flagged clearly as a proposal, not
   asserted as settled.
6. **Place and time of origin, if already decided.** Deliberately worded as broadly as the target setting
   needs — a single-city game needs only a neighborhood; a setting spanning multiple eras, planets, or even
   fictional universes needs whatever placement logic actually applies to each one. Same explicit permission
   to say "you decide" or "TBD." If left open, a placement gets proposed using whichever distribution logic
   actually applies to her setting and era — see `../Tepenia_Worked_Examples/` for a concrete example of what
   that distribution logic looked like in one real, fully-worked setting. Always flagged as a proposal, never
   asserted as settled.

**In the absolute minimal case — an existing folder with reference art but no prior notes — the first three
fields alone are enough to start.** Everything else either gets read from the folder or derived per the
protocol below.

---

## The Derivation Protocol

How each of Stage 1's categories gets populated from the seed fields above, existing setting canon, and
reasonable inference — mapped one by one so nothing is derived by unstated magic.

### Section A — Necessary Fields

- **Foundational Identity Facts.** Name from seed 1. Core nature/type from seed 4 or the folder (seed 2).
  Generational/origin-cohort identity, age, and current residence: inferred from her assigned place and time
  of origin (seed 6) and whatever demographic patterns are established for that setting/era, or defaulted to a
  plausible unremarkable value if nothing in seed 3 suggests otherwise, flagged as inferred, not asserted as
  confirmed. Physical appearance and reference art: read directly from the folder (seed 2) if one exists; if
  not, deferred until concept art exists. Occupation/social role: pulled from seed 3 if stated there, otherwise
  inferred from her assigned setting's established economy and culture.
- **Personality-Type Assignment.** From seed 5 directly if given. If "you decide": proposed from seed 3's
  vision statement plus any reference art, cross-checked against the typing system's own reference material
  (`../Enneagram/`, if using this Pipeline's default system), presented as a proposal for approval — never
  silently asserted as locked.
- **Intended Story Role and Scope.** Defaults to "fully-developed principal/recruitable character, base
  story" unless seed 2 or seed 3 indicates otherwise (a romanceable-but-not-recruitable fixture, a background
  named figure, a walk-on). Any expansion/sequel placement and recurrence: TBD unless seed 2 or 3 already
  implies it.
- **Existing Biographical and Historical Material.** The primary expansion target of seed 3. A vision
  statement's implications get traced outward using the same Why Chain logic already established for Stage 2:
  a stated trait or circumstance gets asked "why" repeatedly against her assigned setting's own established
  history and timeline position, until a plausible, specific Ghost-adjacent history emerges. Proposed, not
  asserted, and always checked against anything already in the folder (seed 2) first so nothing invented
  contradicts something already established.
- **Existing Mechanical and Surface Data.** Read directly from the folder (seed 2) if a surface/mechanical
  spec sheet or game-stat baseline already exists there. If not: deferred, marked not-yet-assigned — this
  methodology does not invent mechanical stats, only remains consistent with them once they exist.
- **World-Context Reference Access.** Not a per-character field at all — handled automatically once the
  foundational identity facts establish a place and time of origin; whichever reference canon actually applies
  for that setting/era gets consulted as needed, without requiring the developer to name it.
- **Standing Design-Law Constraints.** Not per-character — already known and applied automatically to every
  character processed through this methodology, per whatever that project's own standing rules are (see
  `00_Overall_Process_Scaffold.md`'s Cross-Cutting Constraints section for a real, worked example set).
- **The Writer's Own Priming Answers.** **Not requested per-character, per the one-time-cost finding above.**
  Gathered once, separately, whenever convenient — flagged here as an outstanding one-time task, not part of
  this intake.
- **Existing Narrative Introduction Context.** **Deferred (TBD) by default at initial registration.** Only
  built out when this specific character's actual arc development begins, not during bulk intake — unless
  seed 2's folder already has something on record, in which case it's read directly.
- **Existing Supporting Cast and Relationship Web.** Read directly from the folder (seed 2) if it exists.
  Otherwise, whatever seed 3's vision statement implies (a mentioned mentor, a mentioned rival) gets captured;
  the full web is **deferred (TBD)** beyond that until her actual arc development begins.
- **Existing Arc and Ending Concepts.** **Deferred (TBD) by default** — Stage 5 territory, not needed
  until her actual arc is being built, unless seed 2's folder already has drafted concepts on record.
- **Existing Memory and Prior Design Notes.** Not a developer-provided field — checked automatically against
  any existing project record before any processing begins.

### Section B — Optional, Enriching Fields

None of these are requested directly in this intake. All are either pulled from the folder (seed 2) if
present, inferred from seed 3 and setting canon where a reasonable inference exists, or left genuinely blank —
since by definition nothing downstream requires them, an unfilled optional field never blocks anything.

- **Soft-Detail Delivery Material, Speech/Dialect Notes, Food/Music/Sensory Preferences, Found-Family/"Tribe"
  material:** inferred from her assigned setting's established culture plus anything seed 3 already implies
  about her personality, proposed lightly rather than invented in detail — these are meant to be filled in
  properly later, closer to when she's actually being written, not exhaustively front-loaded now.
- **Reputation/Rumor Material, a Basic Headline, an Extended Family Tree, Existing Humor/Voice Lines, Concept
  Art Beyond Reference Images, Secondary Foils, Cross-Media Appearances, Prior Playtesting:** left blank unless
  the folder (seed 2) already has something on record. None of these are ever inferred from nothing.
- **The Developer's Own Unformalized Instincts.** This is functionally the same field as seed 3 — the vision
  statement *is* this category, just asked earlier and given more weight. Nothing separate to gather.

---

## What Happens After the Seeds Are Given

The methodology (or whoever is applying it) produces a full derived Stage 1 sheet from the above, with every
inferred (as opposed to directly-sourced-from-the-folder) field clearly marked as a proposal. This is not meant
to be a silent, one-shot output trusted blindly at scale — the review burden this creates, and how it's kept
small rather than becoming a second full manual pass, is handled by **`00b_Clarification_Protocol.md`**: a
confidence-tagging and minimal-question-surfacing algorithm that resolves only whatever this Derivation
Protocol left genuinely ambiguous for a given character, not a blanket re-review of everything derived here.
