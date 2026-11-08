# Checklist: Dungeon

**Entry** lists what should exist before a chat starts design work with this scaffold. **Exit** is checked before the design stage is called done. Every Exit item is evidence the chat produces, not a promise. The Exit list is the S2 Core design gate ([MACRO_PLAN §1](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/docs/MACRO_PLAN.md#1-stages-and-gates)) plus this scaffold's own G0 desk evidence.

There is no package wrapper or agent brief yet (step 2); a PM briefing a chat for this scaffold writes the brief by hand from this list.

## Entry (warn, never block)

Nothing here locks anyone out (D-014). If an item is missing, the chat tells the developer once, in plain words, what's missing and what it may cost later, then carries on, and notes the warning in its final report.

- [ ] The game has passed the S1 gate in `PROJECT_STATE.md` (required GDD questions answered; scaffold list accepted). If not: "No GDD yet: the scaffold will pick your genre for you. Answer the GDD first."
- [ ] The scaffold list says whether Dungeon is the primary or a secondary. A free pick not on the list is a secondary unless the developer says it replaces the primary; ask once.
- [ ] GDD question 3 (how many human players) is answered. If more than one, Multiplayer Adaptation is on the list too, or the chat says once that co-op rules have no owner yet.
- [ ] GDD questions 2 (why come back), 4 (who it's for) and 9 (the first prototype's question) are answered. Open ones stay OPEN in the brief; ask, never guess.
- [ ] The scaffold folder is in the game repo at `scaffolds/dungeon/`, or the job includes copying it in.

## Exit (gate evidence the chat must produce)

- [ ] `docs/design/first-output.md` has the five parts of the [First output](docs/START_HERE.md#first-output): floor sketch, threat-and-tell table, the stay-or-go moment, four runs, dominance check.
- [ ] `docs/design/DESIGN_BRIEF.md` has every section of [templates/DESIGN_BRIEF.md](templates/DESIGN_BRIEF.md) filled or marked OPEN, with "Adopted revision: scaffold Dungeon @ `<commit>`" in its header.
- [ ] The brief states the run's promise and the stay-or-go decision in the developer's words, quoted.
- [ ] Camera (DG-02), pacing (DG-03), solo or co-op (DG-04), death (DG-05) and carry-over (DG-06) are each PROPOSED with an alternative, or OPEN with who decides and when. None LOCKED without a quote.
- [ ] Two pressure models and two death-and-carry-over models are compared, each with its cost and what would show it works.
- [ ] Every way to die on the first floor has a tell, a counter and a shown cause (DG-17), listed in the floor spec.
- [ ] Every chore system in scope (hunger, wear, identification, light) names the decision it creates, or is cut (DG-18).
- [ ] One floor in `docs/design/floors/` from [templates/FLOOR_SPEC.md](templates/FLOOR_SPEC.md), sized as the first prototype's fixture, with every number marked as a fixture.
- [ ] That floor's traces include the two dominance policies ("dive for the stairs", "clear every floor"), and neither ends better than the best plan, or the brief says why that's acceptable for this floor.
- [ ] `docs/design/status.md` has the game's decision register (from [docs/DECISIONS.md](docs/DECISIONS.md), DG- rows renumbered to the game's own IDs by the PM; none LOCKED without a quote), every [atlas](docs/DESIGN_ATLAS.md) domain marked in scope, out of scope with a reason, or OPEN, and the G0-G7 ledger with no gate marked passed.
- [ ] The weakest assumption and the one question the first prototype should answer are written, ready for the First Playtest prototype brief.
- [ ] Hand-offs listed, not decided: the action list for control-mapping; inventory and status needs for game-ui; what must be readable for art-design; engine needs (generation, lighting, physics, networking) for tech-choice; and, if players > 1, requirements for multiplayer-adaptation.

---

Project Scaffold · created by Carter David Long (Bigfootcdl), with the Claude chat team working under their direction.
