# Character Development Methodology — Stage 5: Beats, Paths & Results

**Pipeline position:** all the possible beats, paths, and results of a character's story arc, built
from the story material produced in Stage 4 (`04_Story_Material.md`).

**Status:** consolidated, with full worked examples validating it end-to-end — see `../Tepenia_Worked_Examples/`
for the complete run-throughs, kept separate so this Pipeline never depends on that specific setting to
function. The Midpoint Menu, the full canonical beat sequence with cross-source glossary, the Branching
Investigation-Route Structure, the Act 3 micro-sequence, arc-type beat-level implications, chiastic mirroring,
and the Ending-Shape Cross-Mapping Table are all in place. Two naming collisions were caught and resolved
along the way ("Point of No Return" and "False Victory," both colliding across independently-mined sources —
see the notes inline below). One worked example caught a real structural flaw (an early-draft Inciting Event
proposal that would have made a character's arc inaccessible to some playthroughs — see
`../Design_Principles/Always_Present_Gating.md`); another produced a second real-world confirmation of the
Ending-Shape table's Disillusionment straddle case (see below).

---

## Arc-Space Enumeration — Generating Every Plausible Arc Before Choosing One

**What this is, and why it comes first:** every other tool in this stage (the Midpoint Menu, the beat
sequence, the Arc-Type beat-level implications, the Ending-Shape table) assumes a single Arc Type has already
been chosen for a given character. This section is the step that comes *before* that choice. For a character
whose Stage 3 Character Data and Stage 4 Story Material are already finished, and who has a concrete
in-context Goal and an established World/Setting-Context to operate within, this tool generates the full space
of arcs she could theoretically go through, before anything gets narrowed down to one.

**Required inputs, all already fixed by this point:** a finished Character Data profile (Stage 3 — her Ghost,
Lie/Flaw, Need/Truth, Want, Desire/Motive, Greatest Fear), her Story Material casting (Stage 4 — MICE
classification, Character Hierarchy, Impact Character/Revenant/Contagonist, antagonist selection), a specific
in-context Goal, and the surrounding World/Setting-Context she's operating in. None of these should change
across the candidates generated below — the whole point is holding the character and her circumstances fixed
and varying only the shape of the arc she goes through.

**Also required: the Story-Format Gate's answer** (`00a_Initial_Input.md`) — linear or non-linear — since it
determines which of the two exit paths at the end of this process actually applies.

### Step 1 — Generate One Full Candidate Arc Per Arc Type

Run this stage's own machinery once per Arc Type (Positive Change, Flat, Disillusionment, Fall, Corruption —
see "The Three Arc Types — beat-level implications," below) against the same fixed inputs: select the Arc
Type's natural Midpoint Menu entry, build out the 11-beat skeleton using that Arc Type's specific beat-level
implications, and note its likely Ending-Shape Cross-Mapping Table row. The output of this step is five full
candidate arcs, not five one-line summaries — each one should be developed far enough to actually judge (a
real Ghost-to-Lie-to-Midpoint-to-Climax throughline), even though most of them won't survive to final content.

### Step 2 — The Plausibility Screen

Not every Arc Type is actually available to every character — a candidate gets disqualified here, not just
deprioritized, when it directly contradicts something already fixed about her:

- **A Flat Arc candidate requires she already holds the Truth at the story's start.** If her Stage 3 Lie/Flaw
  material establishes she does *not* yet hold the Truth, disqualify the Flat Arc candidate outright rather
  than forcing it to work.
- **A Fall or Corruption Arc candidate requires a real, plausible path to her consciously rejecting the Truth
  (Refused Redemption) given her established psychology.** If nothing about her Ghost, Coping/Defense
  Mechanism tier, or Reasons She Can't Quit makes that rejection remotely plausible, disqualify it rather than
  manufacturing an out-of-character turn.
- **Check consistency against her Stage 3 Life Arc archetype, if one was already assigned.** Life Arc
  archetype (Maiden/Hero/Queen/King/Crone/Mage, or whichever set is in use) and Arc Type are different axes,
  but they should cohere — a candidate that fights her already-established archetype's natural shape needs a
  real justification, not just inclusion for completeness.
- **A surviving candidate doesn't need to be good, only genuinely possible.** This screen exists to cut what's
  actually impossible given already-fixed facts, not to pre-judge quality — quality judgment happens at the
  exit-path step below, using different criteria depending on linear vs. non-linear.

What survives this step is the actual, honest answer to "every possible arc she could theoretically go
through" — usually somewhere between two and five candidates, occasionally all five, occasionally as few as
one.

### Step 3 — Exit Path, Determined by the Story-Format Gate

**If Linear (a fixed, single telling):** collapse to one — but the collapse itself is a developer decision,
not something this methodology (or whoever/whatever is applying it) should make unilaterally. **Whoever is
running this process proposes the single strongest surviving candidate** — by thematic fit with the
surrounding story, tone, and what the established Goal and World-Context actually call for — and states
plainly why that one over the others, but the developer is the one who actually confirms it before it gets
built out in full using the rest of this stage's tools.

**Don't discard the losing candidates — write them to that character's own Overflow file.** The fullest worked
instance of `../Design_Principles/Preserve_Unchosen_Material.md`'s general rule (unselected, character-specific
candidates get preserved at every stage of this Pipeline, not just here): a dedicated file (e.g. `[Character
Name]_Arc_Overflow.md`, kept alongside the rest of her character material) capturing every surviving-but-
unselected candidate from Step 2 at the same level of detail Step 1 produced, not compressed summaries — each
one is a genuinely complete alternate arc, not a scrapped idea. This is real, reusable material: a sequel, an
alternate-universe version of the same character, a different character built from a similar seed later, or
simply a reconsideration if the chosen arc turns out not to work once written. Nothing generated at Step 1 is
wasted work, whether or not it was the one selected.

**If Non-Linear (a branching or interactive work):** don't collapse. Promote the surviving candidates directly
into `../Design_Principles/Dual_Outcome_Branching.md`'s mutually-exclusive branch structure, and build each
one out in full as its own complete branch.

- **If the surviving candidate count is within Dual-Outcome Branching's 2-5 range**, promote all of them
  directly — this is the clean case the two tools were designed to hand off to each other.
- **If more than 5 candidates survive the Plausibility Screen**, the 5-branch cap is a real constraint that has
  to be actively reconciled, not silently ignored: either (a) apply Dual-Outcome Branching's own
  distinctiveness standard — a branch earns its slot only if it's a genuine trade-off, not a flavor variant of
  another surviving candidate — and merge or cut down to the strongest 5, or (b) if the character is major
  enough to justify it, treat exceeding 5 as the same kind of deliberate, explicitly-flagged special case
  `../Design_Principles/Trigger_Type_Pattern.md` already carves out for its own scaled-up character — never
  break the cap silently.
- **If fewer than 2 candidates survive**, Dual-Outcome Branching doesn't apply at all for this character —
  build whichever single candidate survived as her sole arc, the same as the Linear case above, and treat that
  as a real, informative finding about her rather than a failure of this process. Some characters, given their
  fixed psychology and circumstances, genuinely only have one honest story.

---

## The Midpoint Menu — a menu of interchangeable mechanics, not a single canonical beat

**Framing:** "the Midpoint" is not a literal 50%-of-runtime timestamp — it's whichever scene functions as this
structural slot in a given branch, wherever it actually lands in a specific telling. Different writing
scholars define what happens *in* that slot very differently, and rather than picking one as canonical, this
system includes every mechanic as a selectable option. For any one specific character's specific arc branch,
exactly one mechanic from this menu gets implemented — but the full menu stays available, and which one gets
picked depends entirely on that character's own context, not on a fixed project-wide default.

**Practical rule for branching arcs:** if a project uses Dual-Outcome branching (see
`../Design_Principles/Dual_Outcome_Branching.md`), each branch is its own complete arc, so each branch picks
its own mechanic from this menu independently. Two branches of the same character's arc can legitimately use
two different mechanics.

### Fully-sourced entries

1. **Moral Mirror Moment** — self-confrontation: who am I / what have I become / what must I become. Can run
   negative→positive (most common), positive→negative, or the tragic variant where change is genuinely offered
   and consciously declined.
2. **Death-Stakes Mirror Moment** — not moral at all: "I might not survive this." Produces a stasis→strength
   shift without requiring the character to change *who* she is. Best fit: Flat Arc characters, action-forward
   characters who don't need identity change, just to get tougher.
3. **Moment of Truth / Subconscious Turn** — the full psychological package: she doesn't consciously reject
   the Lie yet, but her actions start betraying the Truth she's secretly already accepted — the "caught
   between Lie and Truth" double-consciousness. The default, most versatile option for a standard Positive
   Change Arc.
4. **Refused Redemption** (a Negative Arc variant) — she sees the Truth clearly enough for a real chance to
   embrace it, and consciously rejects it for a worse Lie. Fall/Corruption Arc characters specifically.

### Entries with a genuine naming collision, resolved

5. **False Victory** — everything appears to be going great; she seems to have solved her problem or gotten
   what she wanted, but the win is built on the unaddressed Lie and will collapse later. Sets up a harder fall
   at the Third Plot Point; works well for a comedic or upbeat-toned first half.
   - **Naming-collision note:** the canonical 11-beat skeleton (see the full sequence below) also has a beat
     historically named "False Victory," but it sits *late*, immediately before the Third Plot Point, not at
     the Midpoint — an apparent win achieved through the wrong (Lie-aligned) methods, which curdles into a
     hollow victory that precipitates the real crisis. Same exact phrase, two different sources, two different
     structural positions. Resolved by keeping this Midpoint entry's paired terminology intact (False Victory
     / False Defeat is a matched pair worth not breaking) and renaming the later beat instead — see **"The
     Later False Peak"** in the full beat sequence below.
6. **False Defeat** — the inverse: an early gut-punch that feels terminal but isn't the true climax, setting
   up a recovery arc. Fits darker-toned or thriller-adjacent arcs. No naming collision found for this one.

### Broader craft-convention entries — flagged honestly as lower evidentiary weight than the fully-sourced entries above

7. **The External Commitment Event** (deliberately renamed from "Point of No Return" after a naming-collision
   check) — the Midpoint defined by an external, irreversible plot event rather than internal realization at
   all — she's now in it, whether emotionally ready or not. Good fit for Event-type MICE sub-threads (Stage 4)
   that don't warrant full internal-arc treatment but still need a structural midpoint marker.
   - **Naming-collision note:** this was originally called "The Point of No Return," but that exact phrase is
     already claimed elsewhere by two *different* beats in different sourcing — one placing a "Point of No
     Return" Energetic Marker at the Inciting Incident/First Plot Point, and another naming a "Doorway of No
     Return #2" specifically at the transition into Act 3 (the Third Plot Point), implying a "#1" earlier
     still. Both bookend the *middle* with this language rather than using it for the middle itself. The
     underlying mechanic here is still valid for the Midpoint slot — this entry is renamed specifically to
     avoid the collision.
8. **The Recontextualizing Reveal** (mystery/thriller convention) — new information recasts everything before
   it (the trusted figure is the traitor; the goal she thought she had wasn't the real one). The character's
   *response* to the reveal generates the arc from here, not an internal shift at the moment it lands. Strong
   fit for betrayal-centric arcs or conspiracy sub-threads.
9. **Death and Rebirth / The Symbolic Death** (Campbell/Vogler-adjacent) — a symbolic (or briefly literal)
   death of the old self, emerging changed. Strong fit for Crone/Mage-stage characters and for identity-
   fragmentation-themed characters specifically. **Not a separate menu item from #3 so much as a vivid instance
   of it** — the Six Life Arc content library's own pre-built Midpoints (a Maiden's Identities/Loyalties/Wants
   Conflict, a Hero's "Remembering Who He Is," a Queen's Leading the Charge, a King's Witnessing True
   Supernatural Nature, a Crone's Choosing to Seek Life, a Mage's Confronting Evil in the Heart of Man) are
   pre-populated instances of #3 or #9 — not something to pick *in addition to* one of the twelve entries in
   this menu, but the specific flavor this menu takes once a character is already assigned one of the Six
   Life Arcs (Stage 3).
10. **The Dark Mirror Encounter** — the protagonist meets or confronts a figure embodying what she could
    become if she fails. Extends the "antagonist drawn from the next arc-stage" technique (Stage 4) into a
    Midpoint-specific device. Best for a character teetering on the edge of a Fall/Corruption Arc.
11. **The Reactive-to-Proactive Shift, stripped-down** — the purely structural version, deliberately without
    the full psychological apparatus attached: before this point things happen *to* her, after it she starts
    making things happen — full stop, no claim about subconscious Truth-acceptance required. Useful for a
    minor or Flat-Arc character who needs *some* Midpoint marker without the full Lie/Truth machinery.
12. **The Turn / Value-Polarity Flip** (Story Grid-adjacent) — the story's driving thematic value (life/death,
    freedom/slavery, love/hate) flips polarity at the Midpoint. Ties directly back to the "split the theme into
    oppositions" material captured in Stages 3/4. The **Public/Private Stakes Flip** (common in romance/rom-com
    beat-sheet convention — whatever was private about her struggle becomes public, or vice versa) nests under
    this as one specific, frequently-useful flavor rather than its own top-level entry.

### Supplementary cross-references — not competing menu items

- **Later-life crisis stages** (Generativity vs. Stagnation; Integrity vs. Despair) function the same way the
  Six Life Arc Midpoints already do above (see #9): pre-built *thematic content* for whichever mechanic from
  this menu gets chosen, specifically suited to flavoring a Queen/King-stage character's Midpoint (Generativity
  vs. Stagnation) or a Crone/Mage-stage one's (Integrity vs. Despair) — not a competing mechanic in its own
  right.
- **The Preparation → Pressure → Realization → Validation model** is a general drafting *process* for actually
  constructing whichever menu item gets picked, not itself a 13th named beat — useful as the how-to-write-it
  method once a mechanic above has been selected.
- **Chiastic mirroring** (see below) is a cross-cutting structural principle that applies to every entry in
  this menu equally, not a separate mechanic: whichever option is chosen, the Midpoint functions as the
  unpaired axis the rest of the beat structure pivots around and mirrors against.

---

## The Full Beat Sequence — canonical skeleton + cross-source glossary

An 11-beat skeleton stays canonical here, since it's the most structurally complete of the sourcing this
system was built from. Every other naming convention for the same beats folds in as a glossary entry rather
than competing:

1. **Normal World** — the opening world/circumstances, actively built to symbolically dramatize the Lie (Stage
   4).
2. **Inciting Event** — an outside force or discovery that starts things moving. **Refinement**: ensemble
   characters sharing a scene don't need the *same* Inciting Event — one character's triggering event can be a
   different, downstream event from another's, even when both share the larger story.

   **The Trigger-Type Design Pattern.** A standing design rule for constructing any character's actual
   Inciting Event trigger, distinct from the beat's abstract definition above — see
   `../Design_Principles/Trigger_Type_Pattern.md` for the full generalized rule and its origin story.
3. **First Plot Point** — an irreversible first step out of the Normal World; chiastically paired with the
   Third Plot Point (see Chiastic Mirroring, below).
4. **First Pinch Point** — an early complication or pressure point that escalates the opposition.
5. **The Midpoint** — see the full Midpoint Menu above; twelve interchangeable mechanics, pick one per branch.
6. **Second Pinch Point** — a later complication, chiastically paired with the First Pinch Point.
7. **The Later False Peak** (renamed from "False Victory" to resolve the naming collision with the Midpoint-
   positioned beat of the same name — see the Midpoint Menu above) — an apparent win achieved through the
   wrong, Lie-aligned methods; it curdles into a hollow victory that precipitates the real crisis. The Six Life
   Arc content library gives this consistent content across every arc type: a Hero's "wins against the Dragon,
   but only by compromising everything he's learned"; a Queen's "protects her children at the cost of their
   independence"; a King's "tries to stop the Cataclysm with kingly might"; a Crone's "seeks physical
   immortality."
8. **Third Plot Point** — see the Act 3 Micro-Sequence, immediately below; this is where more granular Act 3
   material actually lives.
9. **Climax**
10. **Climactic Moment** — chiastically paired with the Inciting Event.
11. **Resolution** — see the New Normal World's five flavors, folded into the Ending-Shape Cross-Mapping Table
    below; chiastically paired with the Hook.

---

## The Branching Investigation-Route Structure

**Fully optional — a real, concrete example of adapting Stage 5 into a stat/skill-driven game system**, kept
here because it's genuinely useful precedent for a project with its own such system, not because every
project needs it. A distinct mechanic from the Trigger-Type Design Pattern above: that pattern gates arc
*entry* (how many ways can the Inciting Event fire); this one gates the *middle* (how many ways can the player
actually execute the Player-Necessity Rule's unique task once the arc has started, if a project uses that rule
— see `04_Story_Material.md`). The two are complementary, not competing, and a single character's arc can
legitimately use both.

### The Route Counts

- **A minimum of 5 stat-based approaches**, deterministic (no randomness — a threshold is either met or it
  isn't), spread across different stats, and — critically — **each one a different way of executing the
  *same* player-unique task, not five different tasks.** A worked example (see
  `../Tepenia_Worked_Examples/`): one character's arc offered five approaches to the identical
  categorically-exclusive task, each keyed to a different stat (investigation/mapping, calculation/pattern-
  matching, raw force, persuasion, endurance) — one task, five distinct routes to succeeding at it.
- **Non-stat, world-state-based approaches at a floor of 3, target 7-12.** These exist specifically to prevent
  a soft-lock for a player who built entirely outside the covered stats, and — if the project's own romance or
  approval system requires a personal arc to complete before a separate relationship-check can even fire — to
  guarantee that gate and arc completion are never accidentally incompatible with each other.

### Two Standing Stat-Check Design Laws

A real, concrete example of project-specific mechanical rules that had to be reconciled with the story-
structure layer above — include only if your own project has a comparable stat/skill-check system to
reconcile against character content:

- **A "Mastery Dividend" for a perfect/maximum stat result, scoped to the current arc, not game-wide.** When
  one of the stat-based approaches offers a maximum-possible-value option in a given stat, choosing it should
  let the player bypass a real number of subsequent stat/skill checks within that same arc — not a standing,
  permanent effect.
  - **A permanent maximum vs. a temporarily-buffed maximum is a real and load-bearing distinction**, if your
    stat system allows temporary buffs at all. A permanent maximum is reached only through the game's own
    established permanent-stat-increase paths (character creation, training, permanent upgrades). A
    temporarily-buffed maximum merely reads at the ceiling *right now* because of a stacking bonus (a
    consumable, a temporary effect) on top of a lower permanent value. The Mastery Dividend is earned only by
    the permanent maximum, never the buffed one — a temporary buff can still clear the threshold for a single
    check, exactly as the Buffable-Stat-Check Law below requires, but it doesn't represent the genuine, rare
    mastery the Dividend exists to reward.
  - **Implementation:** a permanent-maximum option should appear as its own separate choice, distinct from an
    ordinary buffable stat check on the same stat, so the two are never conflated in the interface or the
    underlying check logic — e.g. a plain `[Stat Threshold]` option stays ordinarily buffable and only
    resolves the single check it's attached to, while a separate `[Permanent Maximum]` option is what actually
    gates the Dividend, selectable only by a genuinely permanent maximum stat.
- **The Buffable-Stat-Check Law, with one standing exception a project might choose to carve out.** Every
  stat/skill check in a game should generally evaluate the player's *current, effective* stat total —
  inclusive of temporary buffs — never the permanent, unadjusted base stat alone (a real precedent for this
  exists in Fallout: New Vegas, where a Strength check can be passed via a temporary food buff exactly as if
  the higher value were permanent). If a project wants one specific check-type to be exempt — say, a
  relationship-eligibility gate that should reflect who the character durably *is*, not a temporary buff —
  name that exception explicitly and only once, rather than leaving it as an isolated footnote that other
  systems might independently, and inconsistently, reinvent.

### The Route-Validity QA Check

A proposed non-stat route is invalid if the character's own already-established standing would already
trivially provide the same access on its own — the route has to bypass something *she* genuinely can't already
get, not just offer the player a redundant path to something she could hand over directly. See
`../Tepenia_Worked_Examples/` for two real, on-record corrections that used exactly this check to catch a
route that didn't actually hold up.

### A Menu of Recommended Non-Stat Route Archetypes

Reach for these where a character's own established world genuinely supports them — never invent the
underlying lore just to manufacture the route:

- **The faction-antagonism route** — where a character has an established negative or wary relationship with
  a specific faction or group, the player's own separate *positive* standing there opens a door she couldn't
  open herself, precisely because she's on the wrong side of that relationship.
- **The extreme-reputation route** — usable specifically by a player holding a rare, contradictory reputation
  state (beloved by one faction and reviled by another, simultaneously) — rare by design, and rewards that
  rare extreme playstyle with real character-content payoff rather than only its own dedicated endings.
  - **Flavor taxonomy, to avoid defaulting to the same mechanic every time:** bureaucratic/records-gap (an
    institution can't file the player, so individualized handling surfaces information as a side effect —
    flagged as overused if reached for reflexively), gossip/rumor (the player becomes unavoidable talk in an
    informal information economy), confessional/psychological (an institution built around sitting with
    irreconcilable truths engages with the player's own contradiction on its own terms), persuasion/leverage
    (someone gambles on the player specifically because their paradoxical reputation makes them worth the
    risk), fear/intimidation (refusing feels more dangerous than complying), and opportunism (someone tries to
    exploit the player's notoriety and the player can leverage that back). When designing a new route of this
    kind, ask what kind of reaction *this specific* faction or group would actually have to an unresolvable
    contradiction, rather than reaching for the bureaucratic default again.
- **The high-investment route** — where a character's own established psychology gives her a genuinely strong
  attachment mechanic (if the project tracks one), a route or full pathline reachable only by a player who has
  reached the deepest tier of that mechanic with her — content that can only exist because of that specific
  state, not a flavor variant reachable another way.

### Multi-Character Non-Overlap Principle

When two characters investigate the same underlying mystery from different angles, their arcs need genuinely
non-overlapping deliverables and mechanisms — completing one must never shortcut or complete the other. The
cleanest version of this splits the shared mystery into structurally distinct halves (one character
reconstructs destroyed content; the other verifies the cause and locates a surviving copy, for instance) rather
than having both characters converge on the identical deliverable through different routes.

---

## The Act 3 Micro-Sequence

More detailed, additive granularity for the space between The Later False Peak and the Climax, not a
competing beat sequence:

1. **Doorway of No Return #2** — the mechanical trigger into Act 3: a discovery, clue, or setback that makes
   the climax actually reachable, not just an emotional shift. (The "#2" implies a "#1" earlier, at the First
   Plot Point — consistent with the naming-collision note above; no separate "Doorway of No Return #1" needs
   naming, since that beat is already covered by the First Plot Point.)
2. **Mounting Forces** — the antagonist escalates specifically because the protagonist's commitment to the
   fight is now unmistakable.
3. **The Third Plot Point / Black Moment / Lights Out** — one beat, several names across different craft
   traditions. The sharpest content rule, worth using as the operative definition: the character's darkest
   fear comes to pass, and it must be engineered to match her specific, already-established Greatest Fear
   (Stage 3 node) precisely — not just "something bad happens." This beat is very often marked by an actual or
   symbolic death.
4. **The Q Factor** — a specific emotional jolt, arriving right around the Black Moment, that supplies the
   courage to go into the final confrontation. Its defining feature: it works by calling back to something
   specific established early in the story (an object, a line, a promise), not a fresh burst of resolve
   invented on the spot — a concrete instance of chiastic mirroring (below), applied to emotional payoff
   specifically.

---

## The Three Arc Types — beat-level implications

(The full taxonomy already lives in Stage 3's Life Arc content-library note; this section is Stage 5's
specific job: what changes at the *beat* level per arc type.)

- **Positive Change Arc** — the default assumption underlying the beat sequence above as written.
- **Flat Arc** — the Midpoint more naturally takes a Death-Stakes Mirror Moment or the stripped-down Reactive-
  to-Proactive Shift (Midpoint Menu #2 or #11) rather than the full Moment of Truth package, since a Flat Arc
  character already holds the Truth and isn't undergoing internal change.
- **Disillusionment Arc** — believes Lie → overcomes Lie → new Truth is tragic. Not morally negative; see the
  Ending-Shape Cross-Mapping Table below for why this variant is the one genuinely underdetermined case.
- **Fall Arc** — the Midpoint specifically takes the **Refused Redemption** mechanic (Midpoint Menu #4): she
  sees the Truth clearly enough for a real chance to embrace it, and consciously rejects it. The Third Plot
  Point/Black Moment for a Fall Arc should read as passive-denial curdling into open aggression.
- **Corruption Arc** — also takes Refused Redemption at the Midpoint. Its Third Plot Point is a precise
  inversion of the standard sequence: **an apparent *triumph* that is actually the true low point** — she
  achieves real, tangible external victory, but the win is hollow and costs her soul. Two foil techniques for
  staging this beat: populate it with a supporting character who shows the better road not taken, *and* a
  separate one showing their own descent as a direct consequence of the protagonist's corrupting influence.
  The Third Act for both Fall and Corruption Arcs reads as "inverted resurrection" — the character rages
  against the loss rather than rising strengthened, blocking the pain with self-justification ("it was worth
  the price").

---

## Chiastic Mirroring — cross-cutting structural principle

Every major beat has a deliberate mirror partner on the opposite side of the story, with the Midpoint standing
alone as the unpaired axis everything pivots around: **Hook ↔ Resolution, Inciting Event ↔ Climactic Moment,
First Plot Point ↔ Third Plot Point, First Pinch Point ↔ Second Pinch Point.**

- **The mirroring is about contrast, not sameness** ("comparative symmetry") — a paired beat should read as a
  deliberate reversal of its partner (the Lie's symbol becomes the Truth's symbol; a scene that once trapped
  the character now frees her), not a repeat.
- **Lighter-weight fallback**: when full plot-level mirroring isn't feasible, mirror or invert specific
  symbols, settings, colors, or which named characters are present at paired beats instead.
- **Workflow note**: figure out the ending first, then retrofit the beginning to set it up — easier than
  forcing an already-written beginning to resolve into a mirrored ending after the fact. Lock the Climax/
  Resolution's content before finalizing the Normal World/Characteristic Moment content, not after.

---

## The Ending-Shape Cross-Mapping Table

Three taxonomies operate at three genuinely different scopes, so this is a cross-mapping, not a merge: **Arc
Types** (whole-story arc shape), **Five Shapes of Endings** (climax outcome), and **the New Normal World's
five flavors** (resolution beat staging/texture: 1 — same place, she sees it differently; 2 — same place, she
actively improves it; 3 — same place, transformed by others' actions; 4 — contrast between her change and an
unchanged setting; 5 — a natural, permanent departure). Mapped directly onto a No-Good-Endings-style
distribution law's categories, if your project has one (see `../Design_Principles/No_Good_Endings.md`), so
Stage 5 builds toward that law rather than just gesturing at it:

| Arc Type | Ending Shape | New Normal World Flavor | Ending Distribution Category |
|---|---|---|---|
| Positive Change Arc | **Lead Sacrifices** (primary template — closest match to a mutual-sacrifice ending mechanic) | 2 or 5 | Costly-positive |
| Flat Arc | Lead Wins (she already has the Truth, uses it to fix the world around her) | 2 or 3 | Costly-positive or bittersweet, depending on what fixing the world costs her |
| Disillusionment Arc | **Genuinely underdetermined** — wins internally (overcomes the Lie) while the external Want may still be lost; can legitimately straddle Lead Wins and Lead Loses rather than picking one cleanly | 4 (the tragic contrast) | Bittersweet |
| Fall Arc | **Lead Loses** | 4, or a permanent negative departure | Negative |
| Corruption Arc | **Lead "Wins" But Really Loses** (already the same beat as the Third Plot Point inversion above, two names for one thing) | 4 | Negative |

- **Disillusionment's straddle is worth stating as a real nuance, not smoothing it over** — it's the one arc
  type where a character's ending may need to be built as two simultaneous, partially-contradictory reads (an
  internal win layered under an external loss) rather than resolved to one shape. This is confirmed by real,
  independent worked examples — see `../Tepenia_Worked_Examples/`.
- **The Open-Ended fifth shape deliberately has no row above** — worth a real caution for interactive media
  specifically: an audience that made active choices expects more definitive closure on a character's arc than
  a passive reader or viewer does. Use sparingly and deliberately, not as a default escape from committing to
  one of the other four shapes.
- **This table is a menu, not a per-character distribution requirement — read it against your own project's
  actual ending-distribution law (see `../Design_Principles/No_Good_Endings.md`), not in isolation.** Two of
  the five rows above land in the Negative category, which could be misread as "40% of a character's endings
  should be negative" if this table were applied mechanically. It shouldn't be: a well-built distribution law
  requires negative endings to be a minority of a *specific character's actual offered endings*, with
  bittersweet as the largest category by a real margin — this table is the lookup for *characterizing*
  whichever arc types get chosen for a given character's branches, not an instruction to draw evenly from all
  five rows. Plan the actual distribution per character first, then use this table to build out each chosen
  branch's specific shape.
- **If your project has a Double-Gate-style mechanical consequence** (a negative personal-arc ending
  permanently disqualifying a separate romance/relationship arc, for instance), the Fall/Corruption rows above
  are exactly where that consequence gets triggered — worth cross-referencing explicitly rather than treating
  as a separate, unrelated rule.

---

## Series-Spanning Arc Models

Relevant to any project with an episodic or expansion-based structure. Two models, not competing — pick
deliberately per recurring character:
1. **One overarching arc across the whole series** — the Lie introduced at the start isn't fully resolved
   until a much later installment; beats stretch proportionally across installments rather than compressing
   into one.
2. **A fresh arc per installment** — a returning character gets a new, self-contained Lie each installment,
   optionally building on Truths already secured earlier (the classic example: a character gets a Positive
   Change Arc in one installment, then a Flat Arc in the next, using her already-won Truth to change the world
   around her).
- **Bonus layering technique**: even within one overarching arc, each installment can carry its own smaller,
  self-contained "mini-Lie" contributing to the larger Lie's eventual resolution, rather than each installment
  being an unmarked slice of one continuous journey.

---

## Common Ending Failure Modes — standing pre-ship checklist

- **Deus ex machina** — any last-minute rescue or resolution must be set up by the protagonist's own prior
  actions, not arrive as unearned coincidence. Never let a character solve the climax using a capability the
  story hasn't established she has, and never let the climax's resolution arrive from outside what the
  protagonist herself set in motion.
- **Loose ends** — route minor-character-fate wrap-up through a single returning secondary character in one
  focused late scene, rather than a clumsy info-dump through the main plot itself.
- **"Only a dream"** (or any twist retroactively invalidating everything already experienced) — a hard caution
  against ever using this shape for a full character arc; the identical device can work in
  short-form content where the twist is baked into the format's own expectations from the start.
- **The talkative villain** — never let a villain's expository monologue be the mechanism that buys the
  protagonist time to escape or be rescued; deliver any necessary exposition either well before the moment of
  maximum urgency, or after the villain has already been dealt with.

---

## QA Tools

- **The "same event, beginning vs. end" consistency check** — if she had to face the Climax's events back at
  the story's beginning, would she react the same way she does at the end? If yes, the arc isn't doing its job
  regardless of how much has "happened" to her along the way.
- **Rewards and Punishments as the branching-consequence engine** — Lie-aligned choices trend worse, Truth-
  aligned choices trend better, the gap narrowing toward "yes, but..." partial outcomes as the arc progresses.
  This is the mechanical engine that should be producing an ending-distribution law's actual outcome spread
  (minority-negative, majority-bittersweet, costly-positive) at the level of individual dialogue/quest
  choices, not just at the level of the final ending selection.

---

## Worked Examples

Two full, real-world run-throughs of this entire stage — every tool above applied to real, specific
characters, checked against their actual established material rather than invented fresh — live in
`../Tepenia_Worked_Examples/`, kept separate so this Pipeline file itself never depends on knowing anything
about those characters or their setting. One of them caught and fixed a real structural accessibility flaw
before it shipped (see `../Design_Principles/Always_Present_Gating.md` for the generalized rule that came out
of it); the other independently confirmed the Disillusionment-straddle edge case in the Ending-Shape table
above, a second real-world data point for a genuine, still-open limitation of the table as built. Worth
reading once, purely as a demonstration of what "running the tools" actually looks like in practice — including
what it looks like when the methodology itself gets something wrong and has to be corrected — before applying
this stage to your own first character.
