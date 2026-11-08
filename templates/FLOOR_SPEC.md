# Dungeon: floor spec

**Template status:** PROPOSED, 2026-10-23. The content unit is **one floor**. Fill what helps; prose is fine. In a game repo, one file per floor (or per room set, if floors are generated) in `docs/design/floors/<floor-id>.md`. See the [worked example](../examples/THE_SALT_CELLARS.md).

## What this floor tests

- **Floor ID / revision / author:**
- **Status:** PROPOSED; desk checks and play tests NOT RUN until recorded.
- **Question:** which decision does this floor test that an existing one doesn't?
- **Budget:** authoring time and reuse allowed.
- **Hand-made or generated:** if generated, which hand-made rooms and which generation rules.

## Situation

- Which floor of the run; what the party is expected to carry and lack on arrival.
- Setting in one or two lines (the project's own, not borrowed).
- Leading pressure and any second one.
- Death model used (DG-05) and anything never shown (DG-21).

## Rules used on this floor

Food, light, movement, death: whatever this floor relies on, stated so two people would trace it the same way.

## Map

| Room | Contains | Neighbours and move time |
| --- | --- | --- |
| | | |

## Clock and pressure

| Time or trigger | Event | Warning first |
| --- | --- | --- |
| | | |

## Threats

| Threat | Where | What it does; time to deal with it | Tell | Counter |
| --- | --- | --- | --- | --- |
| | | | | |

Every way to die needs a tell, a counter and a cause the game shows afterwards (DG-17).

## Things to find

| Thing | Where | What it is | How the party can learn | Sign in the world |
| --- | --- | --- | --- | --- |
| | | | | |

Every harmful unknown has a sign or a recoverable cost (DG-09).

## Ways down

| Way | Where | Cost |
| --- | --- | --- |
| | | |

## Plans and dominance policies

| Plan | Opening choices | What it gains | What it costs | What would disprove the intended tradeoff |
| --- | --- | --- | --- | --- |
| A | | | | |
| B | | | | |
| Dive for the stairs | | | | ends as well as the best plan |
| Clear every floor | | | | ends as well as the best plan |

Name the stay-or-go moment: when, what the party knows and lacks, what each choice risks.

## Traces and checks

Trace plans A and B, a weak start, an understandable death, and the two dominance policies, with times, positions, health and supplies. Then record checks separately:

- Desk trace and arithmetic: NOT RUN [date, finding].
- Bot or scripted policy runs: NOT RUN [policies, caps, results].
- Generation rule checks (if generated): NOT RUN [floors generated, rules checked, failures].
- Play tests: NOT RUN [link to validation report].
- Content cost: NOT RUN [actual hours and iterations].

## If co-op

Splitting up, sharing items, reviving, friendly fire, what a dead player does: requirements for [Multiplayer Adaptation](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/multiplayer-adaptation/PACKAGE.md), not decisions here.

## Decision after testing

Keep, revise, remove or defer; who decided; date; reason. A floor accepted for a test is not production content.

[Design brief](DESIGN_BRIEF.md) · [Validation report](VALIDATION_REPORT.md) · [Core systems](../docs/CORE_SYSTEMS.md)

---

Project Scaffold · created by Carter David Long (Bigfootcdl), with the Claude chat team working under their direction.
