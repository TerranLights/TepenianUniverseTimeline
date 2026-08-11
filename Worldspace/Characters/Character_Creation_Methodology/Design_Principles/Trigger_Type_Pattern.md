# Design Principle — The Trigger-Type Design Pattern

**What this is:** a standing design rule for constructing a character's actual Inciting Event trigger pool —
distinct from the beat's own abstract definition in `../Pipeline/05_Beats_Paths_Results.md`. Directly
generalized from a real replacement design built after the mistake described in `Always_Present_Gating.md` was
caught and fixed. Most directly applicable to branching or non-linear media where a story's entry points can
vary by audience choice; a purely linear work still benefits from the underlying idea (variety and redundancy
in how a thread can plausibly begin) even without needing literal multiple triggers.

---

## The Rule

- **One consistent trigger *type* per character, thematically and functionally matched to her established
  background and personality** — not an arbitrary or generic action, and not a different kind of trigger for
  each individual instance. A character's trigger type should be directly load-bearing on something already
  established about her specifically, never copied wholesale from another character's own type just because it
  worked there.
- **A minimum of roughly 7 concrete triggers of that one type, ideally 12-16.** The point of the volume is
  explicit: the audience or protagonist should never be funneled into one single required path to begin a
  character's story, since that constrains how the larger story can unfold around her. Many thematically
  identical options, not one solitary gate.
- **Every character should have *some* triggers that aren't tied to a specific place, not just characters with
  an unusual structural need for it — but a small number, not a large dedicated pool.** The primary reason is
  flexibility, not edge-case coverage: situations where the character is already active in the protagonist's
  life and the two are somewhere not tied to any specific location. Edge-case coverage (a path through the
  story where every relevant location has become unreachable or hostile, for instance) turns out to need far
  less than it first seems — a single location-independent trigger can already suffice for that worst case,
  since a fully-blocked-everywhere state logically implies exactly one escape hatch is needed, not a large
  redundant pool. These location-independent triggers must stay characteristically consistent with the
  character — same single trigger type as her location-bound ones, just not anchored to a place. The exact
  split between location-bound and location-independent triggers within her total range is a per-character
  design decision, not a fixed ratio.

## Scaling Up for an Unusual Character

A character with genuinely unusual structural requirements (present from the very start of a story, for
instance, rather than introduced normally partway through) may legitimately need a scaled-up version of this
pattern — a much larger total count, split into two explicit tracks (location-bound and not), sized generously
rather than to the strict minimum. This is a real, justified special case, not the default template — most
characters, introduced normally and without that kind of edge case, should default to the more modest 7-16-
trigger range overall, with only a small subset of that total being location-independent.

## Where This Rule Actually Came From

A real character's story originally opened on an optional side-element (see `Always_Present_Gating.md`) — a
design mistake caught before shipping. The replacement used a genuinely different mechanism: a set of world-
state events thematically matched to her own established nature (in the specific case this pattern was
generalized from, events tied to restoring or forging connections, matching a character built around
communication), spread widely enough across the whole setting that no single optional element gated her story,
with a smaller, separate pool of location-independent triggers covering the worst-case scenario where the
usual paths are all closed off. This is the concrete, scaled-up worked example the general 7-16 rule above was
distilled from — the scaled-up numbers were her own special case; the general rule any other character should
default to is the more modest range.
