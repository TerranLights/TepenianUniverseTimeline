# Design Principle — No Good Endings (Ending Distribution & Cost Calibration)

**What this is:** a generalized, portable version of an ending-distribution law one specific project used
across every character arc, district/region-scale story, expansion-scale story, and the main story itself —
confirmed to scale unchanged across all of those levels. Genuinely useful for any project telling multiple,
branching, or repeated character/story arcs where the developer wants meaningful stakes without becoming
uniformly grim.

---

## The Core Rule

Across a character's (or a region's, or a whole game's) full set of possible endings:

- **Negative endings are a minority** — one, or at most a handful, out of the full set offered. Never the
  majority, never even a even split.
- **Bittersweet or mixed endings are the largest category, by a real margin.** This is the default texture of
  "success" in this framework — a genuinely positive outcome that still cost something real.
- **Genuinely, cleanly positive endings are allowed to exist — but never costless.** A true win still requires
  real, mutual sacrifice from someone (the character, the player, or both) to be legitimate. A "good" ending
  with zero cost attached reads as unearned and should be corrected toward either a real cost or reclassified
  as bittersweet.

## Why This Scales Across Every Level

This isn't a character-specific rule bolted on separately at each scale — it's the same underlying principle
of "consequences should feel real without becoming uniformly punishing," applied consistently whether you're
looking at:
- **One character's personal arc** (a handful of branches, see `Dual_Outcome_Branching.md`)
- **A whole region, district, or chapter's worth of story** (dozens of possible resolutions across many
  characters and factions)
- **The full game or story's own main ending set**

At every scale, the same three-part shape holds: minority-negative, majority-bittersweet, costly-positive.

## Plan the Distribution First, Then Build Individual Endings

The practical order that keeps this from drifting: decide the *actual numeric distribution* for a given
character or story's full ending set explicitly, up front — how many endings total, how many negative, how
many bittersweet, how many costly-positive — before writing the specific content of any one ending. Building
individual endings first and hoping the distribution works out afterward is how a set quietly drifts toward
either too grim or too easy.

## Cross-Reference to the Ending-Shape Cross-Mapping Table

`../Pipeline/05_Beats_Paths_Results.md` has a full table mapping Arc Types (Positive Change, Flat,
Disillusionment, Fall, Corruption) and Ending Shapes onto this distribution's three categories. That table is
a *menu* for characterizing whichever arc types get chosen for a given character's branches — it is not itself
a distribution requirement. Don't read "two of five arc-type rows land in Negative" as "40% of endings should
be negative." Plan the actual distribution using this file's rule first; use that table only afterward, to
give the chosen shape its specific texture.

## A Real Mechanical Consequence Worth Adopting: The Double Gate

If your project has a companion/romance system layered on top of personal-arc resolutions, consider this
concrete pattern: a character's personal-arc ending resolving into the Negative category permanently
disqualifies her romance arc for the remainder of that playthrough, regardless of any other player build or
choice. This gives the "No Good Endings" principle real mechanical teeth beyond flavor text — a genuinely bad
outcome for a character should have a genuinely lasting consequence, not just a sadder scene.
