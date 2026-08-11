# Design Principle — Always-Present Character Gating

**What this is:** a hard-won production rule, generalized from a real, caught-in-time design mistake. Relevant
to any character whose full arc needs to stay reachable regardless of how a given reader, viewer, or player
otherwise engages with the story — a genuinely medium-agnostic caution, not a game-specific one, though the
originating mistake happened to occur in an interactive project.

---

## The Rule

**For a character whose full arc needs to remain reachable by everyone who engages with her at all, none of
her structurally load-bearing beats can be tied to something entirely optional or skippable.**

Not just "don't gate her Inciting Event behind an introduction scene" — the stronger, more precise version:
never make a load-bearing beat contingent on a side-element she merely happens to also provide, even if that
element feels closely related to her. In a linear medium this means: don't anchor her arc's opening to a
subplot or chapter a reader could plausibly skip, abandon, or never reach. In an interactive medium it means
the same thing applied to optional mechanics and side-content.

## The Incident This Rule Came From

An early design draft proposed anchoring one character's entire personal-arc opening — her Inciting Event,
First Plot Point, and First Pinch Point — to an optional side-activity she happened to provide (in the
originating project's own implementation, a mechanic letting the protagonist revisit her to adjust an earlier
choice). The escalating sequence of visits to that side-activity looked like a clean structural spine to build
her early beats on.

**This was broken, and caught before shipping:** that side-activity is entirely optional and discretionary —
nothing guarantees any given engagement with the story touches it at all, let alone multiple times. Gating her
arc's start on it — and by extension any downstream material that requires her arc complete first — would have
made her full story permanently inaccessible to anyone who never touched the optional element, or who touched
it once and never returned.

## The Fix

The replacement design used a genuinely different trigger pool entirely: a set of world-state events
thematically matched to the character's own established nature, with enough triggers (and, in the specific
case this rule came from, both location-bound and location-independent tracks) that no single optional element
gates her story, and no single worst-case circumstance can lock someone out entirely either. See
`Trigger_Type_Pattern.md` for the generalized version of that replacement pattern.

## How to Apply This Check

Before finalizing which beat triggers a character's story, ask: **is this trigger something every reasonable
engagement with the story is actually guaranteed to encounter, or could someone genuinely skip it entirely
without doing anything unusual?** If the honest answer is "she could go untouched by this," the trigger doesn't
belong on a load-bearing beat — even if it feels thematically perfect, even if it's an element she herself
provides. Reach for something tied to broader, harder-to-avoid story or world state instead.
