# Character Creation Methodology

**What this is:** a complete, self-contained system for developing any fictional character — from a first
loose idea through fully-built psychology, story role, and beat-by-beat arc — battle-tested across a real,
large-cast production and then deliberately generalized so it carries over cleanly to a different character,
a different cast, a different genre, a different medium, or a different fictional universe entirely. Nothing
in this folder requires the setting it was proven in. It works the same way for a linear story (a novel, a
film, a single closed narrative) as for a non-linear or branching one (a game, an interactive work, a story
with multiple paths), at any point along any timeline, in any setting — including ones with no connection to
where this system was built at all.

**Where this came from, briefly:** built and repeatedly stress-tested while developing characters for one
specific project's cast, then deliberately stripped of that project's own furniture — its terminology, its
specific mechanics, its named characters — so what's left is the underlying craft machinery, not a reskin of
one game's design. Two folders keep that origin material fully intact and available (`Source_Material/` and
`Tepenia_Worked_Examples/`), clearly separated from the portable core so the core never depends on them.

**How to use this folder as a "database-derivative algorithm" for building a character:** start at
`Pipeline/00_Overall_Process_Scaffold.md` — it's the map of the whole system and tells you where to go next
depending on how much you already know about the character. Everything else in this README is a guide to what
each folder is for and when you'd actually open it.

---

## The Seven Folders

### `Pipeline/` — the core, five-stage development process
The actual methodology, start to finish. Begin with a minimal seed of an idea (a name, an image, a single
sentence) and move through five stages that progressively build up a complete character: intake and
clarification (Stage 0 — including a one-time Story-Format Gate deciding whether the target work is linear or
non-linear), raw input gathering (Stage 1), psychological diagnostic tools (Stage 2), a consolidated
psychological data profile (Stage 3), story role and supporting-cast material (Stage 4), and finally the actual
beat-by-beat arc, branching structure, and ending design (Stage 5) — which opens with Arc-Space Enumeration,
generating every plausible arc a finished character could go through given a fixed goal and world-context,
before either collapsing to one (linear) or promoting the survivors into genuine parallel branches
(non-linear). This is the one folder every character-building pass will actually touch. Every file here is
written to be usable with zero knowledge of the project this system was built in.

### `Templates/` — blank worksheets
Two fill-in-the-blank documents for capturing a character in plain prose before any formal analysis begins: a
15-section general character worksheet, and a second, explicitly optional worksheet for characters whose story
involves an ongoing, deep relationship arc with the protagonist (only relevant if your own project has that
kind of character at all — skip it entirely otherwise).

### `Design_Principles/` — standing rules distilled from real production experience
Eight short, independent rules, each one born from a real design problem actually encountered and solved, not
invented in the abstract: how to keep a character's full arc reachable regardless of how someone experiences
the story (`Always_Present_Gating.md`), how to build a healthy pool of ways a character's arc can begin
(`Trigger_Type_Pattern.md`), how to keep a full cast internally consistent by separating what's privately known
from what's shown (`Mystery_Soft_Detail_Delivery.md`), how to track provisional names at scale
(`Placeholder_Naming_Convention.md`), how to make sure a rejected candidate — a hypothesis, a casting choice, a
full arc — never just disappears once something else is chosen instead (`Preserve_Unchosen_Material.md`), how
a secondary romance layer draws narrowly from a character's primary arc work instead of duplicating the full
pipeline (`Companion_vs_Romance_Scoping.md`), and
two related endings-design rules covering branching outcomes and distribution of good/bad/mixed endings across
a character's full outcome set (`Dual_Outcome_Branching.md`,
`No_Good_Endings.md`). Each file states plainly whether it's a universal caution or an optional add-on relevant
only to a specific kind of project.

### `Enneagram/` — a full real-world psychological typing system
A complete, independently-useful deep dive into the Enneagram of Personality (all nine types, each with core
psychology, subtypes, and a growth-path arc, plus foundational system files on triads, wings, instinctual
variants, and how to mine a type's real-world source material for usable character content). Feeds directly
into Stage 2/3 of the Pipeline as one of several diagnostic tools, but stands on its own as reference material
for understanding a real, well-documented framework of human psychology — nothing about it depends on fiction
or on any particular setting.

### `Rapid_Intake/` — a lighter alternative for a large supporting cast
A separate, deliberately lightweight intake process and folder template, for standing up a large number of
minor characters quickly rather than running every one of them through the full five-stage Pipeline. Meant for
exactly the situation where a project has a cast in the hundreds or thousands and most of them will never need
full psychological development — a fast, well-formed starting point instead.

### `Source_Material/` — the raw craft research everything else was built from
Two large source documents: a general character-development craft compilation and a villain/anti-hero-focused
companion volume, both drawn from a wide range of published writing-craft books (Weiland, Boutros, Corbett, St.
John, Card, Swain, Truby, and others). This is the ore the Pipeline was refined from — kept here in full,
unabridged, because the Pipeline's own distilled tools sometimes point back to this material for deeper context
or nuance a short summary can't carry. Not required reading to use the Pipeline; useful when a given tool's
short version leaves a real question unanswered.

### `Tepenia_Worked_Examples/` — real, concrete runs of the whole system
Two full run-throughs of the Pipeline applied to actual characters from the specific project this system was
originally proven in, including a real design mistake that got caught and fixed mid-process (the direct origin
of two of the Design Principles above). Kept in its own folder, entirely separate from the rest of this
resource, so nothing else here depends on it — and deliberately written to stay focused on the *story-craft*
findings (a character's Lie, her arc type, a structural mistake and its fix) rather than on the originating
project's own game-specific mechanics, which don't transfer to other settings or media and aren't included
here. Worth reading once, purely to see what actually running these tools looks like in practice, before
applying the Pipeline to a first character of your own.

---

## What Makes This Actually Portable

A few disciplines were applied consistently across every file in this folder, worth stating explicitly since
they're what makes the "any character, any setting, any medium" claim real rather than aspirational:

- **No fixed cast of beings.** Every reference to what a character fundamentally *is* — human, synthetic,
  something else entirely, or a setting with only one kind of being at all — is phrased as an open question the
  methodology asks about, never an assumption baked into the tools themselves.
- **No fixed medium.** "Story," "arc," and "beat" are used throughout instead of medium-specific words, and
  where a tool is genuinely medium-specific (an interactive-only branching mechanic, for instance), it's marked
  explicitly as optional rather than presented as a default.
- **No fixed mechanical system.** Where the source project's own systems (a particular stat layout, a
  particular long-term tracking mechanic) come up, they're either generalized into "whatever system, if any,
  your own project uses," or moved out of the portable core entirely and left in `Tepenia_Worked_Examples/` as
  historical color, not load-bearing content.
- **Nothing deleted, only relocated.** Every piece of context, background reasoning, and supporting detail this
  system was built from is still here somewhere — the split across these seven folders is about keeping the
  *portable core* (`Pipeline/`, `Templates/`, `Design_Principles/`, `Enneagram/`, `Rapid_Intake/`)
  free of setting-specific weight, not about trimming content down. `Source_Material/` and
  `Tepenia_Worked_Examples/` hold the rest, clearly labeled as optional, one hop away from anything that
  references them.
