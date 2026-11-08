# Worked example: The Salt Cellars

**Status:** PROPOSED fixture, 2026-10-23. Not a chosen game, setting, canon or implementation spec. **Owner:** the adopting project; assignment OPEN.
**Aim:** show one floor specified well enough that two people would trace it the same way, with plans that differ, a stay-or-go choice and a death the player can understand.
**Evidence:** an original paper exercise. The traces are hand-checked, not observations of play.

**Every number here is a fixture** (marked ⓕ where it first appears): invented for this paper test, not taken from Barony or any other game, and not a target for any project. The setting is invented too. Use with the [floor spec](../templates/FLOOR_SPEC.md), [core systems](../docs/CORE_SYSTEMS.md) and [adversarial review](../docs/ADVERSARIAL_REVIEW.md).

## The situation

Floor 3 ⓕ of a run, under an old salt mine. Two characters ⓕ arrive at the Landing at minute 0. They are hurt from floor 2: **14 of 20 health** ⓕ between them (tracked as one pool for this trace). They carry **1 ration** ⓕ, **30 gold** ⓕ and a torch with **9 minutes** ⓕ of light left.

Camera, pacing, input and player count are left OPEN. The trace works the same whether two people play or one player controls both characters. Time is in minutes of play; a real-time or turn-based version would convert it.

## Rules used on this floor ⓕ

- **Food.** On taking a way down, each character eats 1 ration. A character who can't eat arrives Hungry: −2 health on the next floor.
- **Light.** When the torch runs out, every move between rooms takes twice as long.
- **Moving.** Each move between neighbouring rooms takes 1 minute. The party moves together.
- **Death.** Permanent: if the party's health reaches 0, or the Warden catches it, the run ends.

## Map (rooms and moves)

| Room | Contains | Neighbours |
| --- | --- | --- |
| Landing | Arrival from floor 2 | Brine Hall |
| Brine Hall | Crawlers; a dead adventurer (two potions) | Landing, Shop, Shrine, Gallery, Stairs Hall |
| Shop | A trader | Brine Hall |
| Shrine | Free identification | Brine Hall |
| Gallery | Crawlers; **the Chute** (way down 2) | Brine Hall, Pump Room |
| Pump Room | Storeroom (food); the sluice | Gallery, Stairs Hall (by the channel) |
| Stairs Hall | The Salt Golem; **the stairs** (way down 1) | Brine Hall, Pump Room |

## Clock ⓕ

| Minute | Event | Warning first |
| --- | --- | --- |
| 8 | A grinding sound from below | — (this is the first warning) |
| 9 | Grinding again, louder; the torch runs out at 9 unless another was bought | Torch flickers at 8 |
| 10 | **The Warden wakes** (a roar) | Minutes 8 and 9 |
| 11 | **The Warden reaches the party, wherever it is.** It can't be beaten on this floor; if it reaches the party, the run ends | Minutes 8, 9 and 10 |

## Threats ⓕ

| Threat | Where | What it does; time to deal with it | Tell | Counter |
| --- | --- | --- | --- | --- |
| Crawlers | Brine Hall (blocks the way on) | Fight: 1 min, −2 health | Clicking heard from the Landing | None needed; small |
| Crawlers | Gallery | Fight: 1 min, −2 health | Clicking heard from Brine Hall | Avoid the Gallery |
| Salt Golem | Stairs Hall, on the stairs | Fight: 3 min, −6 health | Seen from the Brine Hall doorway; it doesn't move | Flood the hall from the Pump Room: the golem dissolves |
| The Warden | Anywhere, from minute 11 | Ends the run | Minutes 8, 9, 10 | Leave the floor by minute 11; the Chute is one move from the Pump Room |

## Things to find ⓕ

| Thing | Where | What it is | How the party can learn | Sign in the world |
| --- | --- | --- | --- | --- |
| Red potion (unknown) | Dead adventurer, Brine Hall | Healing: +5 health | Drink it; Shop identify (10 gold, 0.5 min); Shrine (free, 0.5 min, one item) | None |
| Cloudy blue potion (unknown) | Dead adventurer, Brine Hall | Blindness: for 2 min, moves take twice as long | As above | The adventurer clutches an empty cloudy-blue flask, with a bandage over the eyes |
| 2 rations | Pump Room storeroom | Food | Search: 0.5 min | — |
| Shop stock | Shop | Ration 10 gold; torch 10 gold (9 more minutes of light) | Buying takes no time | — |

Picking up the potions costs no time if the party has fought the Brine Hall crawlers.

## Ways down ⓕ

| Way | Where | Cost |
| --- | --- | --- |
| Stairs | Stairs Hall | Get past the golem: fight it (3 min, −6 health), or flood the hall (open the sluice in the Pump Room: 1 min; the water drains 3 min after opening, and then the stairs are clear) |
| Chute | Gallery | Instant; the fall costs −3 health per character (−6 total) |

## Plan A: fight through, pay to know (Shop, golem)

Minute 0 Landing → 1 Brine Hall → fight crawlers, take the potions → **2** (health 12). → 3 Shop: buy a ration (20 gold left), pay to identify the red potion (10 gold left) → **3.5**. → 4.5 Brine Hall → 5.5 Stairs Hall → fight the golem → **8.5** (health 6). Drink the red potion: health 11. Take the stairs at **8.5**; both eat (2 rations).

**Arrives on floor 4:** health 11, 0 rations, 10 gold, the blue potion still unknown. The torch had 0.5 min left.

**The stay-or-go moment** comes at 8.5, just after the golem and with the grinding already heard at 8: the Pump Room storeroom (2 rations) is two moves away by the channel and back. Going there and back takes at least 2.5 min (more once the torch runs out at 9), so they'd be back no earlier than 11, when the Warden arrives. The party goes down with no food left for floor 4.

## Plan B: a different plan that also works (Gallery, flood)

0 Landing → 1 Brine Hall → fight, take the potions → **2** (health 12). → 3 Gallery → fight crawlers → **4** (health 10). → 5 Pump Room → search the storeroom → **5.5** (3 rations). → open the sluice → **6.5**. → 7.5 Stairs Hall by the channel; wait for the water to drain at **9.5** (6.5 + 3). The torch runs out at 9 while they wait; they don't move, so it costs nothing. Take the stairs at **9.5**; both eat.

**Arrives on floor 4:** health 10, 1 ration, 30 gold, both potions unknown.

**The stay-or-go moment** is the wait from 7.5 to 9.5: the grinding starts while they stand in the dark. They could drink the red potion to test it (no sign either way) or leave it unknown. The Shop is two moves away, too far with the torch out and the Warden at 11.

## Weak start that recovers

As Plan B, but at minute 2 one character drinks the cloudy blue potion without looking at the dead adventurer. The party is blind from 2 to 4: the move to the Gallery takes 2 min → **4**. Fight → **5** (health 10). → 6 Pump Room → search → **6.5** (3 rations) → open the sluice → **7.5** → 8.5 Stairs Hall (before the torch runs out at 9). The water drains at **10.5** (7.5 + 3). The Warden roars at 10; the party goes down at **10.5**, half a minute before it arrives.

**Arrives on floor 4:** health 10, 1 ration, 30 gold. A scare, a lesson about the sign, and no lasting cost.

## Understandable death

The party tries to see everything. 0 → 1 Brine Hall → fight → **2** (health 12). → 3 Shop: buy a ration, identify the red → **3.5** (10 gold left; no torch bought). → 4.5 Brine Hall → 5.5 Shrine: identify the blue for free → **6**. → 7 Brine Hall → 8 Gallery (grinding; the torch flickers) → fight → **9** (health 10; grinding again; the torch goes out). They head for the storeroom: with no light the move takes 2 min → **11** Pump Room. The Warden reaches them at 11. **The run ends.**

**What the game shows:** "Caught by the Warden. First warning: grinding at minute 8." **What they could have done:** at minute 9 in the Gallery, the Chute was right there: health 10 − 6 = 4 on floor 4, with 2 rations. Or they could have skipped the Shrine, or bought a torch.

## Dominance checks (desk)

| Policy | Trace | Result | Compared with the best plans |
| --- | --- | --- | --- |
| **Dive for the stairs** | 0 → 1 Brine Hall → fight → 2 (health 12) → 3 Stairs Hall → fight the golem → **6** (health 6). Down at 6; 1 ration, so one character arrives Hungry (−2) | Health **4** on floor 4, 0 rations, 30 gold, two unknown potions (drinking the red blind would bring it to 9) | Worse than A (11) and B (10). Diving is possible, not best. |
| **Clear every floor** | The death trace above, plus the golem. Even with a torch bought (0 gold left), the Gallery fight ends at 9, the Pump Room is reached at 10 and searched by 10.5, and the Warden arrives at 11 with the golem still on the stairs | **Caught**, unless the party breaks off to the Chute | Loses. The counter-pressure is the Warden, not more monsters. |

## Questions this fixture raises

- Is the Warden a fair clock, or does it feel like punishment (R11)? It has three warnings and an escape one move away; players may still feel rushed.
- The torch and the Warden both land at 9-10. Two clocks so close may be one too many (DG-18).
- Plan B spends no gold. Is the Shop worth having on this floor (DG-14)?
- The weak start recovers almost fully. The floor may be generous; tune after G1, not before.
- In co-op, could the two characters split (one to the Shop, one to the Pump Room) and beat both plans? Not traced; a question for Multiplayer Adaptation (R5).

[Floor spec](../templates/FLOOR_SPEC.md) · [Adversarial review](../docs/ADVERSARIAL_REVIEW.md) · [Package home](../README.md)

---

Project Scaffold · created by Carter David Long (Bigfootcdl), with the Claude chat team working under their direction.
