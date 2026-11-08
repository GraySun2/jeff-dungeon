# Framework method

**Status:** PROPOSED method, 2026-10-23. How to use this scaffold to design a whole game while adding commitment only when evidence supports it. A chat or a merged PR can't approve a design choice; the adopting owner does.

## Decision words

| State | Meaning |
| --- | --- |
| OPEN | A choice that matters hasn't been made |
| PROPOSED | A specific option or test is ready to look at |
| TESTING | An agreed test is running |
| LOCKED | The owner accepted it, for a stated scope, in their own words (quoted) |
| DEFERRED | Put off on purpose, with a trigger to revisit |
| REJECTED | Ruled out for a stated scope and reason |

For each choice that matters, record: the alternatives, what evidence there is, what it depends on, its cost, who owns it, which gate needs it, and what would make you reconsider. A few lines are enough. The register to start from is [docs/DECISIONS.md](docs/DECISIONS.md).

## The causal test

Give each part one job:

- **The floor** gives the party things to learn, take and avoid.
- **Pressure** (food, light, a hunter, wounds) makes staying on a floor costly.
- **Unknown things** make taking a risk a choice the player can reason about.
- **The descent** turns all of that into a decision: go down now, or stay for one more room.
- **Death** ends the run and teaches something the next run can use.

Ask the counterfactual for each part: if it were gone, which decision would change? If the answer is "nothing, there'd just be less to manage", it hasn't earned its cost yet. Hunger, item wear and identification must pass this test like any other system (DG-18).

Before anyone plays it, write four runs of one floor: a clean descent that still ends on a hard stay-or-go choice; a different plan that also works; a weak start that recovers; and an understandable death. Check their arithmetic. That checks consistency only, not fun.

## Evidence and commitment

Find the weakest assumption with [docs/START_HERE.md](docs/START_HERE.md) and the [atlas](docs/DESIGN_ATLAS.md). Pick the cheapest test that could prove it wrong: a paper floor with a timer, a greybox, or a build. Agree the pass/revise/stop criteria **before** looking at results. Keep every [gate](docs/PRODUCTION_AND_GATES.md) NOT RUN until a real review records a decision.

Keep these questions apart; a yes on one is not a yes on the others: can new players read a floor and understand a death; is the stay-or-go decision interesting; do players want another run after dying; is co-op better than solo, and is solo still good; is generation feasible and readable; what does a new floor type cost; is there demand.

## Composition

This scaffold owns the run: floors, the descent, unknown things, growth inside a run, death and what carries over. A secondary scaffold or a kit may consume those but not redefine them. Keep a small ownership table in the design brief. Co-op players are owned by [Multiplayer Adaptation](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/multiplayer-adaptation/PACKAGE.md): joining and dropping mid-run, revives, who gets which item, what a dead player does while the others play on.

## Adopting

Record the source commit and date. Rename the project, assign owners, replace the example with the project's own floor, and reset tests, thresholds and gates. No audience, setting, tech or approval transfers automatically from this scaffold or its reference games.

[Package home](README.md) · [Decisions](docs/DECISIONS.md) · [Gates](docs/PRODUCTION_AND_GATES.md)

---

Project Scaffold · created by Carter David Long (Bigfootcdl), with the Claude chat team working under their direction.
