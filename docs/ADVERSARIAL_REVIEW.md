# Adversarial review: Dungeon

- **Date:** 2026-10-23.
- **Status:** PROPOSED review and falsification plan; desk review only. No play sessions, prototype, balance trials or production approval are claimed.
- **Aim:** find the conditions under which a descent-and-permadeath dungeon game is frustrating, samey or a chore, using what players most often disliked about Barony and similar games as the starting list.
- **Evidence:** the contracts in [core systems](CORE_SYSTEMS.md), the [Salt Cellars fixture](../examples/THE_SALT_CELLARS.md), and the reference games in [sources](../research/SOURCES.md). The player complaints listed there are the writing chat's summary from general knowledge, not a verified review study.
- **Who does what:** the adopting project's design owner commissions these tests; a test lead records observations; the project owner decides at the [gates](PRODUCTION_AND_GATES.md). These are roles to assign, not people already assigned.

## The strongest objection

Permanent death plus hidden information can make a game where players lose an hour to something they couldn't see coming, then quit. The systems that make dungeon crawlers memorable (unknown potions, curses, traps, hunger, friendly fire) are the same ones players name when they say it was unfair or tedious. The opposite failure: smooth every edge and the run has no danger, so going down is never a decision. The scaffold earns its cost only when **the floor gives the party something it needs, staying costs something it can't spare, and every death has a cause the player saw and could have answered**.

## Findings from this desk review

From hand-tracing the [worked example](../examples/THE_SALT_CELLARS.md) on 2026-10-23. These are desk checks of a fixture, separate from the player tests below.

| Finding | Check and disposition | What's still unknown |
| --- | --- | --- |
| **D1. Diving is possible but not best; as intended for this fixture.** | The dive reaches floor 4 with health 4 (one character Hungry) against 11 for Plan A and 10 for Plan B. The counter-pressure is food: only exploring finds it. | Whether players feel the hunger cost, or forget it until floor 4. |
| **D2. Clearing every room is caught by the Warden; as intended.** | Even with a torch bought, a full clear is in the Pump Room at 10.5 with the golem still on the stairs; the Warden arrives at 11. The Chute is the escape one move away. | Whether players read the grinding at 8 as "leave soon" or as atmosphere. |
| **D3. The blue potion's sign is checkable, and its cost is time, not a life; checked.** | The dead adventurer shows an empty cloudy-blue flask and bandaged eyes. Drinking it costs 2 min of slow moves; the weak-start trace still leaves the floor with half a minute to spare. | Whether players look at the body at all. |
| **D4. Two clocks land together; OPEN.** | The torch runs out at 9 and the Warden wakes at 10. The torch matters only in the death trace. It may be a chore with no decision of its own (R3). | Whether one clock should be cut on this floor. |
| **D5. Plan B spends no gold; OPEN.** | The Shop helps Plan A and the death trace, but a party can ignore it and do as well. | Whether money needs a reason on every floor (DG-14). |
| **D6. The weak start recovers almost fully; OPEN.** | Blindness costs time, not health; the party still arrives with health 10 and 3 rations. The floor may be generous. | Tune after G1 observation, not before. |
| **D7. Co-op splitting isn't traced; OPEN.** | Two players splitting (Shop and Pump Room at once) might beat every traced plan. | A question for Multiplayer Adaptation and R5. |

## Attempts to break the proposal

Numbers in failure signals are proposed diagnostic thresholds for a small test, not benchmarks. Agree them before testing; log the denominator, any help given, and incomplete runs.

| Threat | Procedure | Failure signal and response | Gate |
| --- | --- | --- | --- |
| **R1. Unfair death.** A trap, a curse, an unknown item or a monster kills without a tell or a counter (Barony's most common complaint). | After every death, ask: what killed you, what warned you, what could you have done? Desk-check that every way to die on a test floor has a tell, a counter and a shown cause (DG-17). | Most players can't name a warning after a death, or any death on the first floors comes from full health in one hit. Response: add the tell or the counter before adding content. | G0 desk, G1 |
| **R2. The learning wall.** New players die repeatedly without understanding why, and quit. | Watch first-time players' first three runs without coaching. Log each death's cause and whether they could explain it. | Most first-timers can't explain their first death, or most stop before a third run. Response: teach in play (DG-16): clearer tells, a gentler first area, a cause screen; not a long tutorial. | G0, G1 |
| **R3. Chores.** Hunger, wear, identification, light or weight become busywork. | Log menu actions per floor and time spent managing versus deciding. Ask which systems players would remove. | Managing takes more than about a quarter of floor time, or most players name the same system as "pointless". Response: cut or automate it, or give it a decision (DG-18). | G1 |
| **R4. Clunky menus and inventory.** Especially with a controller, or in a fight. | Time common actions (drink, swap weapon, drop junk, give an item to a friend) on each target input. | Common actions take noticeably longer on one input, or players die in menus. Response: Game UI and Control Mapping own the fix; this scaffold lists the actions and how often they happen. | G1, G3 |
| **R5. Co-op chaos turns sour.** One player carries; friendly fire becomes griefing; dead players sit waiting. (Only if co-op is chosen.) | Log decisions per player, friendly-fire incidents and their cause, and minutes each dead player spends with nothing to do. Use Multiplayer Adaptation's tests. | A dead player waits more than a few minutes with nothing to do, or friendly fire ends runs on purpose. Response: Multiplayer Adaptation's roles and revive rules; friendly-fire options (DG-15). | G2, with Multiplayer Adaptation |
| **R6. Solo is a worse game.** The fun depends on friends. (Only if both modes are chosen.) | Compare the same floors played solo and in co-op: enjoyment, deaths, run length, wish to play again. | Solo players rate it clearly lower or die much more for reasons co-op covers (no revive, no spare hands). Response: give solo its own tools (an ally, a revive item), scale threats; not just lower damage. | G2 |
| **R7. Death costs too much, or too little.** Players quit after losing a long run; or permanent power makes skill matter less. | Compare two carry-over models (DG-06). After a death, ask whether they'd start again now and why. | Most players won't start again after a long run is lost, or most say a death didn't matter. Response: change the carry-over or run length, not difficulty alone. | G1, G2 |
| **R8. Dive for the stairs.** Floors give little, so rushing down always wins. | Run a fixed "go straight to the nearest way down" policy on each test floor by desk trace (and bot if available). Compare the arrival state against the best plan. | The dive arrives as well off as any plan on most floors. Response: shortages only exploring fixes (DG-20). | G1 desk, G2 |
| **R9. Clear every floor.** Nothing pushes the party on, so clearing everything always wins and runs drag. | Run a fixed "visit every room before going down" policy. Compare as above, plus run length. | The full clear wins on most floors, or runs become long without new decisions. Response: a clock, a hunter or growing danger (DG-08, DG-20). | G1 desk, G2 |
| **R10. Samey floors and a repetitive late game.** Generated floors look and play alike; deeper floors only have bigger numbers. | Ask returning players to describe two floors from memory. Count decisions that are new on deeper floors. | Players can't tell floors apart, or the late game adds no new kind of decision. Response: hand-made rooms with distinct choices, new interactions per area (DG-07, DG-19). | G2, G3 |
| **R11. The pressure feels like punishment.** The hunter or clock arrives with no warning or escape. | Log every time the pressure catches a party: the last warning and whether an escape existed. | Players call it unfair, or most catches had no escape. Response: more warning, a visible escape, or a softer pressure. | G1 |
| **R12. One best build.** One class, race or item path is the answer key. | Compare two characters at equal power on the same floors. | One pick wins on every floor, or a floor can't be done without one pick. Response: change the floor or the picks, not just numbers. | G1, G2 |
| **R13. The view hides the floor.** Darkness, first person or busy effects hide threats and items. | Repeat key tasks at minimum display size, low brightness, colour removed, audio off. | A tell can't be read in one of those conditions. Response: fix the tell first. | G1, G3 |
| **R14. Co-op breaks technically.** Desync, lost items, lag deaths. (Only if co-op is chosen.) | Tech Choice and Multiplayer Adaptation feasibility spikes: two players, one floor, a disconnect mid-fight. | Any lost item or death players blame on the connection. Response: those packages own the fix; don't build more content first. | G2 |

## Out of the first proof

Leave out: a full class and race list, followers, crafting, many areas, bosses, a story, generated floors at scale, a meta-progression tree, online networking, and paid extra content. Each adds a second cause for what players do or a big running cost. None is needed to test whether one floor makes "go down now or stay" a real choice and its deaths feel fair.

## Missing before production

No evidence of demand, fair deaths, readable floors, a run length players want, second-floor intent, or achievable scope. No engine, measured generation or performance, content rate, art direction, accessibility check, team, schedule or budget. The [atlas](DESIGN_ATLAS.md) keeps these visible.

## Current desk-review conclusion

The proposal is specific enough for a paper test or greybox of one floor. The fixture shows diving as possible but not best, a full clear caught by a warned hunter, and an unknown item with a fair sign. Its two clocks may be one too many (D4), its shop is optional (D5), it may be generous (D6), and co-op splitting is untested (D7). All gates are NOT RUN.

[Core systems](CORE_SYSTEMS.md) · [Gates](PRODUCTION_AND_GATES.md) · [Package home](../README.md)

---

Project Scaffold · created by Carter David Long (Bigfootcdl), with the Claude chat team working under their direction.
