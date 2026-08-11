# Seed → Profile Population Process

**What this is:** the deliberately minimal counterpart to `seed-template-init.txt`, in this same folder. This
is **not** a lighter version of the full five-stage character-development Pipeline (`../Pipeline/`) — it's a
different tool for a different job. That Pipeline exists to develop a small, curated set of characters into
full principal/companion-grade depth (psychology, arcs, romance if applicable). This process exists to
quickly stand up a presentable, well-formed character folder for a much larger roster — hundreds or thousands
of characters, most of whom will never need that level of development at all. If a character seeded here
later becomes a real principal character in a specific project, that project's own deeper methodology (the
Pipeline) takes over from there — this process doesn't try to anticipate or shortcut that.

**The whole process, three steps:**

1. **Copy `z-template/` to a new folder** named for the character.
2. **Fill in as much of `seed-template-init.txt` as you actually know.** Every field can stay `TBD` — that's
   a valid, expected answer, not a placeholder to feel obligated to resolve.
3. **Transfer each filled-in seed field directly into the matching profile blank**, per the mapping below. No
   inference, no expansion, no derivation — a field that says `TBD` in the seed stays `TBD` in the profile; a
   field that's filled in gets placed directly, with only the light reformatting needed to fit the profile's
   own prose/list style. Everything in the profile the seed doesn't cover stays exactly as blank as it is in
   `z-template/README.md` — this process does not attempt to fill those in.

## The Field Mapping

| Seed field (`seed-template-init.txt`) | Profile destination |
|---|---|
| `Name` | The header line: `## [Full Name] / "[Common Nickname / Callsign]"` |
| `Personality type: XwY (Z Subvariant) Self-Preservation / Social / Sexual` | Splits across two lines under **Core Identity**: `Type: XwY (Z Subvariant)` and `Instinctual Variant:` (the Self-Preservation/Social/Sexual part) |
| `Origin` | `Place of origin` |
| `Location (if different)` | `Primary Location(s) of Residence (if different)` |
| `Timeframe` | `Personal timeline/timeframe` |
| `Brief Personality Summary (abbreviated)` | Under **Personality & Voice**: `Brief Personality Summary (abbreviated)` |
| `Brief Character Backstory Summary (abbreviated)` | Under **Backstory Summary**: `Brief Backstory Summary (abbreviated)` |
| `Weakness (fundamental flaw)` | Under **Core Identity**: `Weakness (fundamental flaw)` |
| `Goal (broad-scale desire)` | Under **Core Identity**: `Goal (broad-scale desire)` |
| `Original design/model reference` | Header block: `Original Model:` |
| `Original creator/manufacturer` | Header block: `Original Manufacturer:` |
| `Original catalog/reference page` | Header block: `Original Catalog Page (if applicable):` |

## Deterministic From the Enneagram Type Alone — Also Filled, Not Left Blank

If using this Pipeline's default typing system (see `../Enneagram/`): Major Theme, Hornevian Group, and
Harmonic Group are not independent fields — each is a fixed function of the core Enneagram type number alone
(the wing never changes any of the three), per standard Enneagram theory. Whenever the seed's personality-type
field gives a type, fill these three profile lines from the lookup table below rather than leaving them blank:

| Type | Major Theme | Hornevian Group | Harmonic Group |
|---|---|---|---|
| 1 | Instinctive | Compliant | Competency |
| 2 | Feeling | Compliant | Positive Outlook |
| 3 | Feeling | Assertive | Competency |
| 4 | Feeling | Withdrawn | Reactive |
| 5 | Thinking | Withdrawn | Competency |
| 6 | Thinking | Compliant | Reactive |
| 7 | Thinking | Assertive | Positive Outlook |
| 8 | Instinctive | Assertive | Reactive |
| 9 | Instinctive | Withdrawn | Positive Outlook |

## What Stays Untouched

Everything else in `z-template/README.md` — Type, Role/Archetype, Affiliation(s), Strengths & Skills, Values &
Passions, Internal Conflict, the full Visual Description, every line under Personality & Voice beyond the one
Summary field, Role in Main Story/World, Canonical Appearances, and all of Design Notes & Open Questions — is
not covered by the seed (directly or by lookup) and stays exactly as blank/TBD as the template itself. That's
by design, not an oversight this process is meant to fix.
