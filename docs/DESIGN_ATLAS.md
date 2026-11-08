# Design atlas

**Status:** OPEN coverage map, 2026-10-23. Aim: account for the whole game without choosing a campaign, audience or technology. The adopting owner marks each domain in scope, out of scope (with a reason) or OPEN, and names who owns it and which gate needs it.

## Player journey across a run

| Stage | Player decision | Design concern |
| --- | --- | --- |
| Character | Who do I play, and what does that let me try? | Real differences without one best pick (DG-10) |
| Arrival on a floor | What's here, what's dangerous, what do we lack? | Enough to read; not so much that exploring is gone |
| Explore | Which door, which room, together or split? | Rooms that offer choices, not corridors of walking |
| Encounter | Fight, sneak, talk, avoid, use the place? | More than one answer; the place itself is a tool (DG-11) |
| Unknown things | Test it, identify it, sell it, or leave it? | Checkable signs; no pure coin flips (DG-09) |
| Manage | Eat, rest, repair, light, heal? | Each chore creates a decision or is cut (DG-18) |
| Stay or go | Stairs now, or one more room? | Both choices credible (the core decision, DG-08) |
| Descent | Which way down, and in what state? | Different ways down with different costs |
| Deeper | What's new down here? | New interactions, not only bigger numbers (DG-19) |
| Death | What killed us, and was it fair? | Cause and last warning shown (DG-17) |
| Between runs | What do we keep, and do we want to go again? | Carry-over chosen on purpose (DG-06) |
| Win and after | What counts as winning; what's after that? | Ending, harder modes, mastery |

## Coverage

| Domain | Questions to answer | Owning document / needed by |
| --- | --- | --- |
| Audience and promise | Who enjoys which repeated decision? Why this over a traditional roguelike or a co-op action game? | Design brief / G0 |
| Tone | How dark, how funny, how serious? What is never shown? (DG-21) | Design brief + [content](CONTENT_AND_PRESENTATION.md) / G0 |
| Camera and perspective | First person, third person, top-down? (DG-02) | Design brief / G0 |
| Pacing | Real time, turns, turns that pass in real time? (DG-03) | [Core systems](CORE_SYSTEMS.md) / G0-G1 |
| Solo and co-op | Solo, co-op, both; how many players? (DG-04) | Core systems; [Multiplayer Adaptation](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/multiplayer-adaptation/PACKAGE.md) if co-op / S2 |
| Death and revival | Permanent death; revival in co-op; downed states (DG-05) | Core systems / G1 |
| Carry-over | Nothing, knowledge, unlocks, power (DG-06) | Core systems / G1-G2 |
| Floors and generation | Hand-made, generated, or generated with hand-made rooms; what generation may never do (DG-07) | Core systems + floor spec / G1-G2 |
| Descent pressure | Food, light, a hunter, wounds, none (DG-08) | Core systems + floor spec / G1 |
| Unknown things | Identification, curses, blessings, signs (DG-09) | Core systems + floor spec / G1 |
| Character | Classes, races, stats, skills that grow by use (DG-10) | Core systems / G1-G2 |
| Interacting systems | Fire, water, light, noise, doors, physics (DG-11) | Core systems / G1-G2 |
| Allies and followers | Recruiting, ordering, losing them (DG-12) | Core systems / G2 |
| Crafting | Salvage and building (DG-13) | Core systems / G2 |
| Shops and money | Buying, selling, stealing (DG-14) | Core systems / G2 |
| Friendly fire and co-op behaviour | Accidents, griefing, shared loot (DG-15) | Core systems + Multiplayer Adaptation / G2 |
| Onboarding | Can a new player learn without a wall of deaths? (DG-16) | Presentation plan / G0-G1 |
| Fair death | Tells, counters, causes shown (DG-17) | Core systems + floor spec / G0-G1 |
| Chores | Hunger, wear, identification, light: do they earn their place? (DG-18) | Core systems / G1 |
| Run structure | Floors, areas, bosses, run length (DG-19) | Run plan / G2 |
| Menus and inventory | Usable with a controller and a mouse; fast in a fight | [Game UI](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/game-ui/PACKAGE.md), [Control Mapping](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/control-mapping/PACKAGE.md) / G1-G3 |
| Presentation | Readable threats, items and exits in the dark, at the chosen camera | [Content and presentation](CONTENT_AND_PRESENTATION.md), Art Design / G3 |
| Accessibility and input | Motion sickness (first person), darkness, colour, audio-only cues | Control Mapping, Game UI / G1-G3 |
| Technical feasibility | Generation, lighting, physics, monster AI, networking if co-op | [Tech Choice](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/tech-choice/PACKAGE.md); tests / G2-G3 |
| Content production | Cost of a new room, monster, item or area; what multiplies | Content plan / G3 |
| Platforms and hardware | Target hardware, display size, performance | Platform matrix / G3-G4 |
| Operations | Saves (and save-scumming), crash recovery, settings, telemetry and consent | Reliability plan / G3-G4 |
| Business and distribution | Positioning, demand test, price, what's paid extra (DG-22) | Commercial plan / G4 |
| Production | Count, team, budget, schedule, release and support | Production plan / G4 and later |

## Missing before production

This scaffold has no audience study, market forecast, chosen engine, class list, item list, art bible, hardware results, budget or staffing plan, and the example fills none of these. Record them as OPEN and resolve them before the commitment that needs them.

## Change and cost review

When adding a system, name the decision it creates, which domain owns it, what it needs to be readable, how it fails, and what content it multiplies. A new item effect, for example, multiplies across every class, every monster, every system it can touch and every co-op combination. Include the cost of revising it, not just building it.

[Decisions](DECISIONS.md) · [Core systems](CORE_SYSTEMS.md) · [Gates](PRODUCTION_AND_GATES.md) · [Package home](../README.md)

---

Project Scaffold · created by Carter David Long (Bigfootcdl), with the Claude chat team working under their direction.
