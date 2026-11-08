# First design session

**Status:** PROPOSED guide, 2026-10-23. Aim: end the session with a testable run promise and a clear boundary, not a locked engine, setting or campaign.

Start with: **When the party is a few floors down, hurt, short on food and carrying things it hasn't identified, what makes "take the stairs now" and "explore this floor a little more" both real choices, and what makes a death feel fair enough that players start again right away?**

## Steps

1. **Who is it for, and what are ten good minutes?** Name the audience and describe ten minutes they'd enjoy: opening a door into a dark room, a friend drinking an unknown potion, the moment someone says "we should go down now". Say what getting better at the game lets them do.
2. **Pick a camera and pacing for the next test only** (DG-02, DG-03). First person in real time, top-down in turns, or something between each change what players can see, how fights feel and how readable a trap is. Write what the choice excludes.
3. **Solo, co-op or both** (DG-04). Write what each player does in a quiet minute, and what a dead player does while the others play on. If co-op is in, Multiplayer Adaptation is in the job.
4. **Choose the leading pressure** (DG-08). Food, light, a hunter that comes if you stay too long, wounds that don't heal, or nothing but greed. Pick one to lead; add a second only when it changes a decision.
5. **Sketch one floor** with the [floor spec](../templates/FLOOR_SPEC.md): rooms, two ways down with different costs, the threats and their tells, two unknown items and their checkable signs, and what the party is short of on arrival.
6. **Write four runs of that floor** (from the [framework method](../FRAMEWORK_METHOD.md)): a clean descent that still ends on a hard stay-or-go choice; a different plan that also works; a weak start that recovers; and an understandable death.
7. **Try the two dominance plans on paper** ([adversarial review](ADVERSARIAL_REVIEW.md) R8, R9): "dive for the stairs" and "clear every floor". If either wins every time, change the floor before going further.
8. **Decide death and carry-over for the first test** (DG-05, DG-06). What ends a run, and what the next run keeps: nothing, knowledge, unlocks or power. Write what a new player keeps after their first death.
9. **Name the weakest assumption** and the one question the first prototype should answer. Pick a gate in [production and gates](PRODUCTION_AND_GATES.md) and agree its pass/revise/stop criteria before anyone plays.

The [design brief](../templates/DESIGN_BRIEF.md) collects all of this. Prose is fine.

## First output

One file in the game repo, `docs/design/first-output.md`, with these five parts. All numbers are provisional and marked so.

1. **Floor sketch.** A rough map of one floor: rooms, where the party arrives, every way down, threats, items, the pressure clock. A box-and-arrow drawing or a list is enough.
2. **Threat-and-tell table.** One row per thing on the floor that can hurt or kill:

   | Threat | What it does | Tell before it lands | Counter the party can have | What the game shows after a death |
   | --- | --- | --- | --- | --- |
   | (e.g. a trap) | (damage, a status) | (a sound, a mark, a shape) | (an item, a skill, a route) | (the cause, the last warning) |

3. **The stay-or-go moment.** The point on the floor where the party could go down now or stay. Say what they know, what they don't, what they're short of, and what each choice risks.
4. **Four runs.** One paragraph each: clean descent with a hard choice; a different plan that also works; weak start that recovers; understandable death. For the death, say what the player saw before it happened and what they'd do differently.
5. **Dominance check.** One line each on what happens if the party dives for the stairs, and if it clears every room. If either is clearly best, say what you'll change.

When this exists, fill the [design brief](../templates/DESIGN_BRIEF.md) into `docs/design/DESIGN_BRIEF.md` and write the floor into `docs/design/floors/<floor-id>.md`, then check the [Exit list](../CHECKLIST.md#exit-gate-evidence-the-chat-must-produce).

## What can wait

A full class and race list, many biomes, bosses, a story, a shop economy across floors, crafting, followers, procedural generation at scale, final art, voice and online networking can wait until a specific test needs them. The [atlas](DESIGN_ATLAS.md) keeps them visible so they don't disappear from the plan. One hand-made floor is enough to test the stay-or-go decision.

[Package home](../README.md) · [Decisions](DECISIONS.md) · [Example](../examples/THE_SALT_CELLARS.md)

---

Project Scaffold · created by Carter David Long (Bigfootcdl), with the Claude chat team working under their direction.
