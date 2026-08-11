# Character Development Methodology — Overall Process Scaffold

**What this is:** a broad-scale architecture map of the whole methodology pipeline — the five numbered stages,
plus the intake layer in front of them. This file is the map, not the territory; full detail lives in each
stage's own file (`00a`, `00b`, `01` through `05`, all in this same `Pipeline/` folder).

**Portability note:** this whole system was built and battle-tested inside one specific fictional universe
(originally: a sci-fi CRPG's companion-character design), then deliberately generalized into this
self-contained form so it works for building *any* character, in *any* setting, at *any* point in a story —
linear or non-linear, any genre, any medium, with or without game mechanics attached. Nothing in this Pipeline
assumes a specific universe, species, technology level, or narrative format. Where a concrete, fully-worked
example would help, see the separate `Tepenia_Worked_Examples/` folder — it's genuinely optional, kept apart
on purpose so this Pipeline never depends on knowing anything about that specific setting to function.

**Why five stages, and what each one actually does:**

1. **Input Information** — everything that has to already exist, or be gathered, before any generative work
   starts on a given character.
2. **Information Processing** — the diagnostic toolkit: techniques for interrogating raw inputs to surface a
   genuine, specific psychology, rather than starting from a blank page or a generic trait list.
3. **Character Data** — the actual structured output of Stage 2, written down as reusable fields on a
   character's psychological profile (as distinct from a project's own surface/mechanical stat sheet, if it
   has one — see the `Templates/` folder for an example of that lighter layer, kept separate from this deep
   one).
4. **Story Material** — converting a finished Character Data profile into actual story scaffolding: her role,
   her supporting cast, her thematic shape, what kind of story she's even in.
5. **Beats, Paths & Results** — the full beat-by-beat structural machinery, branching into every possible arc
   type, path, and ending a given character's story material can resolve into.

Downstream stages consume upstream ones. Stage 5 can't be built without Stage 4's story material; Stage 4 can't
be built without Stage 3's character data; and so on.

---

## The Intake Layer — `00a` and `00b`

Not one of the five numbered stages — a compression layer sitting in front of Stage 1, built specifically for
scale: any project with a large cast (dozens, hundreds, or more) will find manually filling in Stage 1's full
field set per character unworkable one at a time.

- **`00a_Initial_Input.md`** — the minimal seed-field intake (name, a folder/file pointer if one already
  exists, a rough vision statement, core nature/type if the setting has more than one kind of being, a
  personality-typing axis if known, place/time of origin if known — the last few with an explicit "you decide"
  escape hatch) plus the full Derivation Protocol mapping those seed fields onto every one of Stage 1's
  categories, deferring what genuinely doesn't need to exist yet (introduction-scene context, the full
  relationship web, exact ending concepts) rather than front-loading everything. Also carries the **Story-
  Format Gate** — a one-time, project-level (not per-character) linear/non-linear decision that determines how
  Stage 5's Arc-Space Enumeration tool resolves its output for every character processed afterward.
- **`00b_Clarification_Protocol.md`** — the repeatable algorithm for resolving whatever `00a`'s derivation
  leaves genuinely ambiguous, per character. Confidence-tags every derived field (Sourced / Strong Inference /
  Weak Inference / Blocked), only ever surfaces a question for a Section A field at Weak-Inference-or-worse
  with no safe default, ranks surviving gaps by downstream leverage (personality-type assignment highest, then
  backstory wound, then core nature/type), and phrases whatever survives as closed-form multiple-choice with a
  "you decide" option.

---

## Cross-Cutting Constraints — apply at every stage, owned by none

These are the standing design disciplines this whole system was built under. The first three are genuinely
universal writing/game-design principles, worth adopting as defaults in any project. The rest are one
project's own specific implementation choices, kept here because they're a real, battle-tested example of how
a project can turn these principles into binding rules — adapt or discard them freely for a different project's
own needs.

- **This is a non-linear methodology.** Every beat below is defined by functional role, never by fixed
  percentage-of-runtime placement — nothing here assumes a particular story length, medium, or pacing.
- **Preserve Unchosen Material** (see `../Design_Principles/Preserve_Unchosen_Material.md`) — at every stage
  that produces more than one concrete, character-specific candidate (a psychological hypothesis, a casting
  choice, a full arc), the ones that don't get selected still get written down in full somewhere durable, not
  discarded. Whoever is applying this methodology proposes the strongest candidate at each fork; the developer
  confirms it.
- **No Good Endings / Ending Distribution law** (a genuinely portable principle, detailed in
  `../Design_Principles/No_Good_Endings.md`) — negative endings are a minority, bittersweet is the largest
  category, positive endings are real but never costless. Stage 5's Ending-Shape Cross-Mapping Table builds
  toward this distribution by default; discard it if a given project genuinely wants purer positive or purer
  tragic endings instead.
- **No Demographic Stereotyping** — a character's origin, species, culture, or background should never be
  used as a shortcut for her personality. Applies most directly to Stage 3's Background Taxonomy and to any
  in-fiction regional-reputation shorthand.
- **No Level-Scaling** (a specific developer's own standing law across every one of their own game projects,
  included here as a real example of a project-wide constraint a character-creation pipeline has to respect,
  not because it's universally applicable) — enemies, loot, and encounters don't scale to match the player's
  level; the world has a fixed, designed difficulty. Not a character-psychology concern directly, but worth
  keeping in view for any project building a world around its characters.
- **The Dual-Outcome Branching law** (see `../Design_Principles/Dual_Outcome_Branching.md`) — 2-5 mutually
  exclusive resolution branches per character arc, genuine trade-offs on every branch. The mechanical skeleton
  Stage 5's branching content serves, if the target project wants branching character resolutions at all.
- **Two stat-check design laws**, included as a concrete example of project-specific mechanical rules that
  had to be reconciled with the story-structure layer: every skill/stat check reads the player's current,
  effective total including temporary buffs, with one exception carved out for a specific high-stakes gate
  type; and a Natural (unbuffed) maximum result in a stat-based approach grants a bonus that lets the player
  bypass a real number of subsequent checks within that same arc. Fully game-mechanic-specific — relevant only
  if the target project has its own stat/skill-check system to reconcile against character content; otherwise
  skip entirely.

---

## Stage 1 — Input Information

**What it contains:** foundational identity facts; the mandatory personality-typing assignment (this system
was built around the Enneagram — see the sibling `../Enneagram/` folder — but any well-grounded typology
system could substitute); intended story role/scope; existing biographical and historical material (typically
the single most input-hungry category, feeding Stage 3's Ghost/backstory-wound node directly); existing
mechanical/surface data if the target project has its own separate stat sheet; world-context reference access
(whatever the target setting's own established canon, lorebooks, or faction/culture material is); the
project's own standing design-law constraints; the writer's one-time baseline self-reflection answers (not a
per-character cost — see Stage 2's Memory Mining tool); existing narrative introduction context; existing
supporting cast; existing arc/ending concepts; and a memory/prior-notes check. A second, optional tier
covers soft-detail delivery material, speech/dialect notes, reputation, a pre-existing basic headline if one
exists, extended relationships, food/music preferences, found-family/"tribe" material, existing voice
specimens, concept art, secondary foils, cross-media appearances, prior playtesting, and the developer's own
unformalized instincts.

---

## Stage 2 — Information Processing

**What it contains:** four Governing Principles (Backstory Proportionality, the Consistency Caution, the
Mystery Caution — see `../Design_Principles/Mystery_Soft_Detail_Delivery.md` — and the "Character Is Not You"
caution); two consolidated diagnostic nodes (the Why Chain/Interrogation Technique; Self-to-Character Memory
Mining); and four standalone tools (the In-Voice Character Interview, Obstacle Brainstorm-and-Triage, the
Scenario Diagnostic Template — the single most fully-built tool in the whole methodology — and Compare-and-
Contrast Self-Image, plus Compelling Need and the Public/Private Values Gap). The personality-typing assignment
from Stage 1 stays the mandatory primary motivational axis throughout this stage; a secondary, optional
motivational lens can layer on top if useful, but shouldn't replace it.

---

## Stage 3 — Character Data

**What it contains:** a front-gate tier system (walk-on/minor/major, bridging a Drift-vs-Drive question with
Stage 4's Character Hierarchy); seven consolidated psychological nodes (Want, Need/Truth, Lie/Flaw, Ghost,
Desire/Motive, Greatest Fear, and a Background Taxonomy spanning Body/Environment/Experience/Ideas); eight
standalone fields (Strength, Reasons She Can't Quit, Dominant Attitude + Contradictory Exception, Character
Trait vs. Personality Trait, a four-tier Coping/Defense Mechanism, a Speech-Pattern Correlation Table, the
mandatory personality-type assignment, and an optional secondary Direction/motivation field); a diagnostic
test (Flaw vs. Personality Trait); a two-tier coverage-checklist system (a master Character Notebook checklist,
plus a separate delivery-channel audit — the different ways an audience actually comes to know a character);
and a small library of pre-built archetype content (this system used the Maiden/Hero/Queen/King/Crone/Mage Life
Arc set) that can seed the Lie/Truth pairing rather than requiring it be invented from nothing. A full per-
character fill-in worksheet (tier determination, construction order, cross-references back to Stage 2's tools)
sits on top of the vocabulary.

---

## Stage 4 — Story Material

**What it contains:** a three-step Front-Gate/Sequencing Trio (MICE Quotient → Character Hierarchy → Story
Problem vs. Character Problem); the Contagonist (a genuine merge of two overlapping source concepts); Impact
Character and Revenant kept deliberately separate, since collapsing them loses real information — a
non-Truth-aligned Revenant case routes toward villain/anti-hero material instead (see
`../Source_Material/Character_Development_Methodology_-_Villains_and_Antiheroes_-_DRAFT_Ideas.md`); standalone
tools (the Normal World, the Characteristic Moment, Antagonist vs. Antagonistic Force, the Twelve Archetypal
Antagonists, Four-Corner Opposition, the Four Elements of Relationship Sizzle, a functional-role catalogue for
supporting cast); composability notes between the various orthogonal systems above; two staging/sympathy
techniques (a general sympathy-lever catalogue, plus cat-save/delay-the-worst-act staging); and — as a
project-specific, fully optional add-on — the Player-Necessity Rule and its four supporting constraints, kept
here as a real example of what it looks like to adapt this methodology's story material into an actual
companion-character game system (see `../Design_Principles/` for the generalized versions of the constraints
worth carrying to a different project).

---

## Stage 5 — Beats, Paths & Results

**What it contains:**
- **Arc-Space Enumeration** — the entry point to this whole stage: holding a character's already-finished
  Stage 3/4 material, Goal, and World-Context fixed, generate one full candidate arc per Arc Type, screen out
  whichever are genuinely implausible given her established psychology, then either collapse to the single
  strongest candidate (linear projects, per the Story-Format Gate in `00a`) or promote the survivors into real,
  mutually exclusive branches via `../Design_Principles/Dual_Outcome_Branching.md` (non-linear projects) —
  including how to handle more or fewer surviving candidates than that rule's 2-5 branch range.
- **The Midpoint Menu** — twelve interchangeable Midpoint mechanics (not one canonical beat), spanning a
  two-type Mirror Moment, a Moment of Truth, a Negative Arc's Refused Redemption, a False Victory/False Defeat
  pairing, and broader craft-convention entries, plus three supplementary cross-references.
- **The full beat sequence** — an 11-beat canonical spine (Normal World → Inciting Event → First Plot Point →
  First Pinch Point → Midpoint → Second Pinch Point → The Later False Peak → Third Plot Point → Climax →
  Climactic Moment → Resolution), with every other naming convention for the same beats folded in as a
  glossary rather than treated as competing, plus the generalized Trigger-Type Design Pattern for Inciting
  Event construction (see `../Design_Principles/Trigger_Type_Pattern.md`).
- **The Branching Investigation-Route Structure** — a project-specific, fully optional add-on (kept here as a
  worked example, generalized further in `../Design_Principles/Dual_Outcome_Branching.md`): a minimum number
  of deterministic approaches to the same character-unique task, non-stat/world-state approaches as a
  supplementary path, a route-validity QA check, a menu of recommended non-stat route archetypes, and a
  multi-character non-overlap principle for projects with more than one character built this way.
- The Act 3 micro-sequence, the beat-level implications of several distinct Arc Types (Positive Change, Flat,
  Disillusionment, Fall, Corruption), chiastic mirroring as a cross-cutting structural principle, the
  Ending-Shape Cross-Mapping Table (mapping Arc Types × Ending Shapes × Ending-Distribution categories, with an
  explicitly-flagged edge case for reactive/Flat-Arc-adjacent characters that the table doesn't resolve
  cleanly), series-spanning arc models, common ending failure modes (deus ex machina, loose ends, "only a
  dream," the talkative villain), and QA tools.

---

## Cross-Stage Notes

- **Two genuinely different source types feed this methodology, worth keeping distinct in any project that
  adopts it.** Most of Stages 1-3 and much of 4-5 trace back to published writing-craft material (see
  `../Source_Material/` for the full raw mining this Pipeline was distilled from). A smaller portion — the
  Player-Necessity Rule, the Branching Investigation-Route Structure, and the two stat-check laws — comes from
  a different source entirely: one specific project's own already-mature, in-production game-design system.
  Both are legitimate, but they carry different evidentiary weight and different revision paths. Craft-derived
  material can be re-checked against its source books directly; project-specific material should be kept in
  sync with that project's own design docs, which are the actual source of truth for anything codified as
  that project's own canon.
- **The villain/anti-hero supplement material remains a parallel, not subordinate, resource** — feeds Stage 4
  (antagonist/villain story material) and Stage 3 (irredeemability thresholds), kept deliberately separate. See
  `../Source_Material/Character_Development_Methodology_-_Villains_and_Antiheroes_-_DRAFT_Ideas.md`.
- **This whole system was validated against real, fully-worked characters** before being generalized into this
  portable form — see `../Tepenia_Worked_Examples/` for the complete run-throughs, kept separate so this
  Pipeline never depends on that specific setting to function.

---

## What This File Is Not

Not the finished methodology in full — that's the seven files it maps (`00a`, `00b`, `01` through `05`). This
file is the navigational summary; if any stage file changes substantially, this scaffold should get a matching
pass rather than being left to drift stale.
