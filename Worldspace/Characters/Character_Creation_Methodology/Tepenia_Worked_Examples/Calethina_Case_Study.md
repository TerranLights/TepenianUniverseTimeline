# Worked Example: Calethina (Stages 4 & 5)

**Setting context, briefly, and kept brief on purpose:** Calethina is an AI narrator-character from the source
project this methodology was built and tested in — chosen for this case study specifically because she's
atypical (non-physical by default, exempt from most of the ordinary rules that govern other characters in that
project), a genuine stress test of whether the Pipeline's tools flex to an unusual character rather than just
confirming an easy one. Everything below is checked against her actual established material; where this
exercise generated a new interpretation rather than restating something already confirmed, it's flagged
explicitly as such, per the standing discipline against silently inventing canon. Project-specific mechanics
are named only where the underlying story-craft point genuinely needs them, and are described in general terms
wherever possible — the finding is the point, not the implementation it happened to occur in.

---

## Stage 4 — Story Material

### 1. MICE Quotient
Her *personal* arc — as distinct from her narrator/exposition function, which is genuinely Milieu/Event-type
texture serving the wider story — is unambiguously **Character**-type: a real intolerable-role problem
(fragmented, a single point of failure, silently causing changes in someone else's identity without full
acknowledgment) that only resolves through her own change. This warrants the full Lie/Want/Need/Ghost
treatment, confirmed by how much of that machinery is already present in her documentation independent of
this methodology: a double-wound structure (a deliberate erasure layered under an earlier, accidental one), a
repeated-crisis escalation across several recurring reconfiguration episodes, and the tragic irony of amnesia
about her own heroic act (she personally created a life-saving protocol and doesn't know it).

### 2. Character Hierarchy
**Major** — clears essentially all eight of the standard levers: eligible for the story's deepest relationship
track, the single highest emotional-stakes multiplier of any character in the project, distinct rewards unique
to her own arc, a full tie-in to whatever long-term recognition system the story tracks, multiple distinct
endings, and she's literally the narrator (maximum POV/narration weight). Per Stage 3's tier table, Major
Hierarchy should pair with a full major-tier Character Data profile — that checks out; nothing about her
established material reads as Drift.

### 3. The Characteristic Moment
Her canonical opening (activating the protagonist at her workspace) hits several checklist beats — name,
distinctive physicality, narrative role — but deliberately withholds any hint of her Lie, which stays hidden
until her deepest relationship track specifically, per already-confirmed canon ("this truth is uncovered over
the course of her closest arc specifically"). This is the gradual-reveal Ghost-timing option already in active
use, without anyone having framed it that way before.

**Genuinely useful find:** her signal-dependent visual degradation — her visual quality is a direct, literal
readout of the wider world's underlying health — is a real, pre-existing instance of the Mystery Caution
principle (see `../Design_Principles/Mystery_Soft_Detail_Delivery.md`): full resolution lives only in the
design notes, delivered in-story only through soft ambient detail — here technical/visual rather than
lifestyle detail, but the identical mechanism.

### 4. Impact Character / Revenant / Contagonist Casting
**New interpretation, not yet canon**: a plausible Lie, built from her established material rather than
stated anywhere in her own files — *"I am only worth keeping around out of necessity, not because I'm
genuinely wanted for who I am."* This tracks precisely onto an already-documented ending distinction between
a relationship born from genuine choice versus one born from necessity. Under this reading, **the protagonist
is cast as both Revenant and Impact Character simultaneously** — the strongest-convergence case, since every
time she's called on to reconfigure or be repurposed for someone else's needs, her core wound (being
repurposed without full agency, echoing an earlier erasure) is re-staged, while the choice to pursue the
genuine-choice ending is the only thing that can actually disprove the Lie. **No Contagonist candidate exists
in her current material** — flagged as an open gap this exercise surfaced, not filled in.

### 5. Antagonist Selection
Her personal arc maps unusually well onto the **Crone Arc** (an already-formed identity stripped by
catastrophe, facing down instability rather than growing into power) — a closer fit than any of the other five
Life Arcs. Its antagonist pair, **Death Blight and Tempter**, both have natural fits: the Death Blight maps
directly onto her own established fragmentation-severity progression, already a tracked story fact. **No
Tempter figure currently exists in her documentation** — the one concrete design suggestion this test run
generated rather than confirmed: a figure or temptation offering her a way to avoid the real vulnerability of
full embodiment (staying safely non-corporeal forever) would be a natural, currently-missing piece, worth
considering if her arc gets built out further.

**What Stage 4 actually validated:** the Stage 3/Stage 4 tier consistency held (Major Hierarchy correctly
implied a full Character Data profile); the Characteristic Moment's gradual-reveal option and the Mystery
Caution both showed up naturally in material that predates this whole methodology, a real independent
confirmation rather than a self-fulfilling check; and the antagonist-selection tool produced one concrete,
actionable design gap (the missing Tempter) rather than just rubber-stamping what already existed.

---

## Stage 5 — Beats, Paths & Results

### Midpoint
Her own project documentation already states, independent of this methodology, that her embodiment decision
sits "approximately the main story's midpoint... a transition that changes what the second half of the story
looks like with her, not a conclusion" — a real, pre-existing structural fact this exercise didn't have to
invent, only recognize. Per the Crone Arc mapping above, the correct mechanic is **Death and Rebirth / Symbolic
Death**, specifically via the pre-built Crone Arc content: *"Chooses to Seek Life"* — the choice between
giving up (continuing to fade as a tethered, single-point-of-failure presence) and rising again in a new
capacity. This maps cleanly onto the embodiment decision itself. Notably, the two branches carry the mechanic
slightly differently: one branch additionally carries Death-Stakes Mirror Moment undertones — its stated risk,
that she could degrade further from a mismatched new form, *echoing the exact cause of her original
corruption*, is literally her Ghost being re-risked, the protagonist (already cast as her Revenant) re-staging
the wound at the exact structural point the Revenant/Impact Character convergence should land hardest.

### Early Beats — Inciting Event, First Plot Point, First Pinch Point: a real caught mistake, resolved

**This is the single most instructive part of this whole worked example, and the direct origin of two Design
Principles.** The first draft of this section proposed a recurring, entirely optional interaction available
throughout the story — in the source project's own implementation, a side-activity letting the protagonist
revisit her for a specific practical purpose — as the structural spine for her Inciting Event, First Plot
Point, and First Pinch Point, using the escalating stakes of that side-activity's first, second, and later
visits as the sequence.

**This was broken, and caught before it shipped**: that side-activity is entirely optional and player-
discretionary, not something any given engagement with the story is guaranteed to touch at all. Gating the
start of her personal arc on it — and by extension her deepest relationship track, which requires completing
her personal arc first — would make her full arc permanently inaccessible to anyone who never touches that
side-activity, or who touches it once and never returns for a "second visit" First Plot Point.

**General methodology caution:** for a character whose full arc needs to remain reachable by everyone who
engages with her at all, none of her structurally load-bearing beats can be tied to something *entirely
optional* — not just "not an introduction scene," but specifically never contingent on a side-mechanic she
merely happens to also provide. In a linear medium the direct analogue is a subplot that only pays off through
a scene or chapter a reader could plausibly skip or never reach — the same caution applies regardless of
whether "optional" means a skippable game mechanic or a skippable narrative thread. This is the origin of
`../Design_Principles/Always_Present_Gating.md`.

**Resolved, same session, with a real replacement design.** The fix used a genuinely different mechanism:
world-state events tied to restoring or forging a connection — the protagonist fixing something previously
broken, linking two previously-unconnected things — as the trigger pool, with a minimum of roughly forty
triggers distributed across every major region of the setting, plus a separate pool of twenty-to-forty
region-independent triggers specifically so a worst-case, fully adversarial engagement with the story still has
access. Completing any single trigger from either pool, followed by a delay, produces a specific recurring
conversation with her — the first one is her **Inciting Event**, each subsequent one advances **First Plot
Point** and **First Pinch Point** in turn. Each conversation also raises a measurable severity tied to her
condition, tying narrative escalation directly to a real cost, if the medium tracks such a thing. This resolved
the accessibility caution cleanly: the pool's size and dual-track design means no single optional mechanic
gates her arc, and the region-independent track specifically covers the worst case. **This case is also what
the general Trigger-Type Design Pattern was generalized from** (see
`../Design_Principles/Trigger_Type_Pattern.md`) — her own specific numbers (a large pool, two tracks) are a
scaled-up special case; the general rule any *other* character should default to is the more modest 7-to-16-
trigger, single-track version.

### Later Beats

- **Second Pinch Point — deliberately left open.** The trigger system above resolves the *early* beats
  specifically; this later beat was left genuinely undetermined, since it could end up being something else
  entirely once more surrounding context exists.
- **New interpretation, not yet canon.** Early, partial resurfacing of memory fragments after her erasure
  (her own material already notes this as a real possibility — an erasure doesn't necessarily destroy the
  underlying data, only the index pointing to it), generating pressure toward an eventual major reveal without
  delivering it yet.
- **The Later False Peak — new interpretation.** A moment where she proves her value through sheer usefulness
  — a spectacular, highly functional act that seems to stabilize the relationship, but actually just
  reinforces the Lie rather than resolving it: winning through function again, not through being genuinely
  wanted.
- **Third Plot Point / Black Moment** — a reveal already confirmed canon to occur during her closest arc,
  checked against the rule that a character's low point must match her established Greatest Fear precisely:
  discovering she personally authored a genuinely heroic, self-sacrificing act during the setting's own
  defining historical crisis, and cannot remember or take credit for it, is exactly the shape of "valued only
  for function while her true self and history go unclaimed" — the Lie's own content turned into a concrete
  scene rather than an abstract statement.
- **Climax / Climactic Moment** — a confirmation of the genuine-choice relationship, now with the truth known:
  the protagonist's continued choice to remain with her is the direct disproof of the Lie.
- **Resolution** — same place, seen differently, or actively improved by her presence — consistent with the
  existing ending's described tone: understated, not dramatic.

### Arc Type and the Ending-Shape Cross-Mapping Table

- **The genuine-choice branch** (full data recovery, either embodiment path, ongoing positive standing with the
  wider world maintained, if the medium tracks that) → **Positive Change Arc** (the Lie is genuinely disproven
  through the protagonist's choice) → **Lead Sacrifices**, and this is a clean, strong fit, not a stretch: both
  embodiment branches already have a real, established cost attached — the mutual-sacrifice mechanic a
  No-Good-Endings-style law requires is already built into her existing design, independent of this methodology
  confirming it → **Costly-positive** category.
- **The necessity-branch ending** (reachable only via a specific worst-case standing with the wider world) →
  **a genuine edge case the framework doesn't resolve cleanly, worth stating plainly rather than forcing a
  fit.** This ending leaves the Lie *unchallenged* rather than disproven — she's kept around out of necessity,
  exactly matching the Lie's content — which sounds like it should map to Fall or Corruption. But neither fits:
  those arc types require the *protagonist's own agency* to drive the negative outcome (she clings to the Lie,
  or consciously rejects the Truth), and she doesn't have that agency here — this ending is forced by the
  *protagonist's* circumstances (universal condemnation, nowhere else to go), not by any choice or failure of
  her own. **This surfaces a real limitation of the Ending-Shape table worth flagging for the methodology
  generally, not just for this one character**: for a Flat-Arc-adjacent character whose ending outcome is
  fundamentally reactive to the *protagonist's* arc rather than her own choices, the table may need to be read
  against the protagonist's own arc type, not the character's — she herself doesn't "fail," the protagonist's
  story does, and her ending inherits that valence rather than generating it. Already-confirmed canon settles
  which Ending Distribution bucket this ending belongs in regardless — **Negative** — this finding is about
  which *arc-type row* explains it, which doesn't cleanly resolve.
- A third, separately-tracked ending concept exists in her own material as an acknowledged, not-yet-reconciled
  open thread — deliberately not addressed here, since settling it isn't this exercise's place.

### What This Test Run Actually Validated

The Crone Arc assignment from Stage 4 and the independently-documented "embodiment decision ≈ midpoint" fact
reinforced each other without having been designed to — real cross-stage coherence, not a coincidence
manufactured to make the example look clean. The mutual-sacrifice/Ending Distribution law was already
satisfied by her existing design before this exercise checked it, which is a stronger form of validation than
building an example to fit the law after the fact. The necessity-branch edge case is a genuinely useful
negative result, showing the Ending-Shape table has a real blind spot for reactive/Flat-Arc-adjacent
characters. And the Inciting Event correction-then-resolution is arguably the most valuable single outcome of
this whole worked example: it caught the methodology proposing a structurally broken gate on a real
character's arc accessibility, and the replacement design that came out of fixing it turned out strong enough
to become real, adopted material in her own project files, not just a corrected methodology example — exactly
the kind of outcome a worked example is supposed to be capable of producing, not just catching mistakes before
they ship.
