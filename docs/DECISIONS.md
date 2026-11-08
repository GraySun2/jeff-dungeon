# Decision register

**Status:** every row PROPOSED, OPEN or DEFERRED, 2026-10-23. These are the scaffold's own IDs (DG-), for choices an adopting game makes. They are not Project Scaffold decisions (those are D- IDs in [docs/DECISIONS.md](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/docs/DECISIONS.md)), and a game repo gives its own D- IDs (D-017). Only the adopting owner's own words lock a row.

## Task authority

bigfootcdl asked for this scaffold (A1 to A5, quoted in [PROVENANCE.md](../PROVENANCE.md)). That authorizes writing it. It approves no game, prototype or design choice below.

## Choices to resolve

| ID | Choice and state | Alternatives | Evidence / gate / revisit |
| --- | --- | --- | --- |
| DG-01 | Core loop: PROPOSED | Explore a floor → encounter → test unknowns → manage → stay or go → descend, ending in a win or a death that teaches; compare a plain action game with floors if the stay-or-go choice adds little | Desk trace at G0; players at G1; revisit if the descent is never a decision (R8, R9) |
| DG-02 | Camera and perspective: OPEN | First person (Barony, Ultima Underworld); third person; top-down or grid (most traditional roguelikes) | Owner at G0; changes readability, motion sickness, co-op awareness |
| DG-03 | Pacing: OPEN | Real time; turns; turns that pass when the player acts; real time with pause | Compare on one floor at G0-G1; real time raises the fair-death bar (R1) |
| DG-04 | Solo, co-op or both: OPEN | Solo only; co-op only; both, with solo as a full mode | Owner in S2; if co-op, [Multiplayer Adaptation](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/multiplayer-adaptation/PACKAGE.md); revisit if solo is a worse version (R6) |
| DG-05 | Death model: OPEN | Permanent death; downed then dead; co-op revive at a cost; a ghost or spectator role; extra lives per run | Compare two at G1 (R7) |
| DG-06 | What carries over between runs: OPEN | Nothing; knowledge only (a bestiary, identified items); unlocks that add options (classes, starting kits); power (permanent stats) | Compare two at G1-G2; avoid power that hides a weak first floor (R7) |
| DG-07 | Floor generation: PROPOSED hand-made first | One hand-made floor for the first test; then generated layouts with hand-made rooms; fully generated; fully hand-made | G1 hand-made; generation feasibility at G2; revisit if floors feel the same (R10) |
| DG-08 | Descent pressure: OPEN | Food; light; a hunter that comes after a time; wounds; rising danger; greed only. One leads | G0-G1; revisit if the pressure feels like punishment (R11) |
| DG-09 | Unknown things: PROPOSED with signs | Use-to-learn; identify by a service or skill; signs in the world (price, a corpse, a note); knowledge kept across runs | G1 (R1, R3); every harmful unknown has a checkable sign or a recoverable cost |
| DG-10 | Character: OPEN | Classes; races; free stats; skills that grow by use; a mix | G1-G2 (R12) |
| DG-11 | Interacting systems: PROPOSED a small set | Fire, water, light, noise and doors first; physics, weather, factions later | G1-G2; each interaction must change a decision |
| DG-12 | Allies and followers: DEFERRED | None; hired; recruited by talking; summoned; built | After G1 |
| DG-13 | Crafting: DEFERRED | None; salvage and build gadgets; brewing; repair only | After G1 |
| DG-14 | Shops and money: OPEN | None; shops per floor; a hub between areas; stealing with consequences | G1-G2; revisit if money is ignorable (example D5) |
| DG-15 | Friendly fire and co-op behaviour: OPEN | On; off; reduced; on with protections against griefing | G2 with Multiplayer Adaptation (R5) |
| DG-16 | Teaching: PROPOSED in play | Learn by play with tells and shown causes; a tutorial floor; tips on death; an easier first area | G0-G1 (R2) |
| DG-17 | Fair death rules: PROPOSED | Every way to die has a tell, a counter and a shown cause; no unblockable death in one hit from full health early on | G0 desk, G1 (R1) |
| DG-18 | Chore budget: PROPOSED | Each of hunger, wear, identification and light must create a decision, or be cut or automated | G1 (R3) |
| DG-19 | Run structure: OPEN | Floor count; areas; bosses; run length in minutes; endless mode | G2; revisit if late floors are repetitive (R10) |
| DG-20 | Anti-dominance counter-pressures: PROPOSED | For "dive": shortages (food, light, keys) that only exploring fixes; better items deeper only if prepared. For "clear every floor": a hunter or clock; food that runs out | G1 desk, G2 (R8, R9) |
| DG-21 | Tone: OPEN | Grim; darkly funny; heroic; whimsical; plus a "never shown" list | Owner at G0; see [content and presentation](CONTENT_AND_PRESENTATION.md) |
| DG-22 | Engine, art, platform, business model: OPEN | Through Tech Choice, Art Design and later gates; whether any content is paid extra | Not chosen by this scaffold |
| DG-23 | Worked example: PROPOSED fixture | The Salt Cellars' rules and numbers | Desk consistency is not G0; replace on adoption |

## Adding a decision

Record: ID and date; the choice and its scope; alternatives; evidence and its limits; dependencies and cost; owner and needed-by gate; whose words authorize it; what would make you reconsider. Write LOCKED only with the owner's quote. Keep superseded rows and link the replacement.

[Framework method](../FRAMEWORK_METHOD.md) · [Gates](PRODUCTION_AND_GATES.md) · [Package home](../README.md)

---

Project Scaffold · created by Carter David Long (Bigfootcdl), with the Claude chat team working under their direction.
