# Core systems and ownership

**Status:** PROPOSED design contracts, 2026-10-23. Aim: make the floor, pressure, unknown things and the descent push on each other so the stay-or-go decision is real and deaths feel fair. **Owner:** the adopting designer. Every section below is a set of options to choose from, not a rule; the DG- IDs point to [decisions](DECISIONS.md). No example number is a requirement.

## Run circuit

| Stage | Player decision | What it feeds into next |
| --- | --- | --- |
| Character | Who to play; starting kit | What can be tried on the first floors |
| Arrive | Read the floor: what's visible, heard, known | Where to go first |
| Explore | Which door; together or split | What's found; time, light and food spent |
| Encounter | Fight, sneak, avoid, use the place | Health, noise, items, time |
| Unknown things | Test, identify, sell or leave | New options or new problems |
| Manage | Eat, heal, repair, light | What's short when the stay-or-go moment comes |
| Stay or go | Stairs now, or one more room | The state the party arrives in below |
| Descend | Which way down | Next floor's starting position and cost |
| Death or win | What ended it | What the next run keeps (§10) |

## 1. Camera and pacing (DG-02, DG-03)

| Model | What it gives | What it costs |
| --- | --- | --- |
| First person, real time (Barony) | Darkness and doors are scary; co-op chaos is vivid | Hard to read the room; motion sickness; reaction-speed deaths; menus fight with the action |
| Top-down or grid, turns (traditional roguelikes) | Everything readable; time to think; deep item interactions | Less immediate; co-op turns make players wait |
| Top-down, real time | Readable and fast; good for co-op | Less mystery in the dark; dodging becomes the skill |
| Turns that pass only when the player acts | Thinking time with movement that feels live | Odd in co-op; needs clear rules about what a "turn" is |

Whatever is chosen, state: what advances time; what the player sees of danger before it lands; how long they have to react; and whether opening a menu pauses the game (in co-op it usually can't). Real time raises the bar for fair death (§7).

## 2. Solo, co-op or both (DG-04)

| Option | What it changes here |
| --- | --- |
| Solo only | Everything must be fun without friends to laugh with; pacing and difficulty tuned for one |
| Co-op only | Chaos and shared stories carry the game; a player who can't find a group can't play |
| Both | Solo must be a full mode, not a worse co-op: scale threats, give solo players a tool co-op gets from friends (an ally, a revive item) |

For any co-op option, use [Multiplayer Adaptation](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/multiplayer-adaptation/PACKAGE.md). It owns joining and leaving mid-run, who owns which item, revives, what a dead or disconnected player does, and host authority. This scaffold writes the requirements (for example "a player who dies has something to do within a minute", "an item in a disconnected player's pack is not lost") and lets that package decide how.

## 3. The floor (DG-07)

A floor is a set of rooms, at least two ways down, the threats, the items, and what the party lacks on arrival.

- **Rooms that offer choices.** Each room should hold a decision: a fight to take or avoid, an item to test, a shortcut with a cost. A room that's only walking is a cost with no choice.
- **More than one way down.** For example: the main stairs (guarded), a hidden way (needs a key or a search), a fall (fast, costs health). Different costs make the descent a decision.
- **Generation (DG-07).** Proposed order: one hand-made floor for the first test; then generated layouts built from hand-made rooms; full generation only when its rules are tested. Rules generation must never break: a way down is always reachable; no unwinnable fight blocks the only way on; a deadly threat never spawns next to the arrival point; the floor's pressure is always visible.

## 4. Descent pressure (DG-08)

What makes staying costly. Extraction's rule holds: pick one to lead, then add.

| Pressure | How it presses exploring | Risk |
| --- | --- | --- |
| Food | Every room costs food; finding food is a reason to explore | Chore if food is plentiful or the counter is fiddly (R3) |
| Light | Torches burn; darkness slows or blinds | Frustrating if darkness hides threats unfairly (R13) |
| A hunter that comes after a time | A clock with teeth; staying is a gamble | Feels like punishment if there's no warning or escape (R11) |
| Wounds that don't heal | Every fight is spent from a limited pool | Death spirals with no recovery |
| Rising danger | The floor gets worse the longer you stay | Hard to read |
| Greed only | No push; the player decides when they've had enough | "Clear every floor" wins (R9) |

The pull to design: **exploring gives what the party lacks, and staying costs what the party needs.** If one side always wins, see §11.

## 5. Unknown things (DG-09)

Potions, scrolls, rings and gear the party doesn't recognise. They make experimenting a decision. Barony and NetHack show this can make great stories; they also show it can make deaths that feel like a coin flip.

**Ways to learn what something is:**

| Way | Example | Design question |
| --- | --- | --- |
| Use it | Drink, read, wear | Is the worst outcome survivable on its own? |
| A service | A shrine, a shopkeeper, a scroll | What does it cost, and is it always available? |
| A skill | Appraisal that grows by use | Does it make one class mandatory? |
| A sign in the world | The price, a body with an empty flask, a note, a smell | Can a careful player have suspected it? |
| Knowledge between runs | Once known, known in later runs | Does it empty the mystery too fast? |

**Rules for fairness:** every harmful unknown has at least one checkable sign or a cost the party can recover from; testing should be a choice with odds the player can reason about, not a blind gamble; a cursed item that can't be removed needs a counter on the same floor or the next.

## 6. Character (DG-10)

Options: classes; races; free stats; skills that grow by use (Barony's swords, stealth, trading and more). Rules: every pick opens a way to play, not just more numbers; no class or race is the answer key (R12); a new player's first pick should be forgiving. Name for each pick one floor where it's weaker than another.

## 7. Fair death (DG-17)

The most important contract in this scaffold. Barony's most common complaint is deaths that come from nowhere.

- **A tell.** Every way to die shows itself first: a sound, a shape, a mark, a smell, a wind-up, a warning message.
- **A counter.** The party could have done something: an item, a skill, a route, running away.
- **A cause shown afterwards.** On death the game says what killed you and what the last warning was.
- **No early one-hit deaths.** On the first floors, nothing kills from full health in one hit without a tell the player had time to react to.
- **Bad luck stays small.** Random outcomes can hurt, but the worst outcome of one roll shouldn't end a healthy run alone.

## 8. Systems that interact (DG-11)

Start small: fire, water, light, noise and doors. Each interaction must change a decision (fire burns a door instead of picking the lock; water puts out fire and a torch; noise brings monsters from the next room). Add physics, weather or factions only when the first set is readable. These interactions are where co-op stories come from; they're also where unfair deaths hide, so each one needs a tell (§7).

## 9. The chore budget (DG-18)

Hunger, item wear, identification, light, weight. Each must earn its place:

| System | The decision it should create | If it doesn't |
| --- | --- | --- |
| Hunger | Explore for food, or go down hungry | Cut it, or make food a reward, not a tax |
| Item wear | Repair, replace, or risk it | Automate repair, or make wear rare and readable |
| Identification | Test, pay, or leave it | Give signs; keep knowledge between runs |
| Light | Spend light to explore, or move on | Make light plentiful and use darkness only as a mood |
| Weight | What to carry out of a room | Generous limits; a quick drop-the-junk action |

Count the menu actions each chore needs per floor. If players spend more time managing than deciding, cut.

## 10. Death and what carries over (DG-05, DG-06)

| Model | Next run keeps | Feels like | Risk |
| --- | --- | --- | --- |
| Nothing carries over (Barony) | Only what the player learned | Pure skill; every run equal | Players quit after a long run lost (R7) |
| Knowledge carries over | A bestiary, identified items, notes | Learning is visible | Mystery gone fast |
| Unlocks carry over | New classes, starting kits, areas | New things to try | Grind to unlock the fun |
| Power carries over | Permanent stats | Progress even when failing | Hides a weak first floor; skill matters less |

In co-op, decide what a dead player does: wait, watch, play a ghost with a small job, or come back at a cost. Multiplayer Adaptation owns the mechanics; this scaffold names the requirement: a dead player has something to do within a minute, or the run ends soon after.

Whatever is chosen, show the cause (§7). Consider the player who dies early many times in a row: they must still want another run.

## 11. Dominance (DG-20)

Two policies to check on every floor:

- **Dive for the stairs.** If floors give little and pressure is high, rushing down always wins. Counter-pressures to choose from: shortages (food, light, keys) that only exploring fixes; deeper floors that need gear found above.
- **Clear every floor.** If floors are safe once cleared and there's no clock, clearing everything always wins and runs become slow. Counter-pressures: a hunter or clock; food that runs out; danger that grows.

A plan that works on one floor is fine. The problem is a plan that works on every floor without reading it. Test both in the [adversarial review](ADVERSARIAL_REVIEW.md).

## Ownership

| Rule | Owned here | Others may add |
| --- | --- | --- |
| The run: floors, descent, unknowns, death, carry-over | This scaffold + floor spec | |
| Co-op players: joining, dropping, revives, loot | [Multiplayer Adaptation](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/multiplayer-adaptation/PACKAGE.md) | This scaffold names requirements |
| Buttons | [Control Mapping](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/control-mapping/PACKAGE.md) | This scaffold names the actions |
| Inventory, map, status screens | [Game UI](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/game-ui/PACKAGE.md) | This scaffold names what must be read |
| How threats and items look | [Art Design](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/art-design/PACKAGE.md) | This scaffold names what must be readable |
| Engine, generation, lighting, networking tech | [Tech Choice](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/tech-choice/PACKAGE.md) | This scaffold names what's needed |

If two documents disagree, settle the owner and fix the other.

[Adversarial review](ADVERSARIAL_REVIEW.md) · [Gates](PRODUCTION_AND_GATES.md) · [Package home](../README.md)

---

Project Scaffold · created by Carter David Long (Bigfootcdl), with the Claude chat team working under their direction.
