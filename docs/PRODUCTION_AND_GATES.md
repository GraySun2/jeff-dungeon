# Production and gates

- **Status:** PROPOSED; every gate NOT RUN.
- **Date:** 2026-10-23.
- **Aim:** one gate ladder that tests whether floors, pressure, unknown things and the descent make each other better, and whether deaths feel fair, before content grows or production is committed.
- **Owner:** the adopting project names a test lead and a decision owner before testing. This scaffold assigns neither.

## Before any test

The project owner accepts or changes the thresholds **before** results are collected. Record the accepted version, audience, recruitment, facilitator, decision owner, help policy, session cap and cost in the [validation report](../templates/VALIDATION_REPORT.md). A threshold changed after seeing results is a new hypothesis, not a pass.

A designer tracing a floor, a bot running a policy, and a person playing answer different questions; report them separately. Count people as people: replays don't add participants. Every result has a numerator and a denominator, including help given and missing data.

Thresholds below are proposed starting points for small diagnostic tests, in the shape of Tactical Extractions' ladder. They are not benchmarks.

## Gate ladder

| Gate | Question | Planned evidence | MACRO_PLAN stage | Current |
| --- | --- | --- | --- | --- |
| **G0 Experience clarity** | Is the promise clear, can a new player read a floor, and is every death on it fair on paper? | Design brief with alternatives and exclusions; desk trace of one floor (four runs, two dominance policies, the threat-and-tell table); then a few first-time players | S2 Core design (exit) | NOT RUN |
| **G1 Descent loop value** | On one floor, is "go down now or stay" a choice players feel and can explain? Do they understand their deaths and want another run? | First played session (the S3 gate record), then more players on the same floor; two death-and-carry-over models compared | S3 First prototype (started) → S4 (passed) | NOT RUN |
| **G2 Repeat, dominance and co-op** | Does the decision survive several floors and the two dominance policies? Is solo good; does co-op give everyone something to do? | Returning players over a short run of floors; R8, R9, R12 policy tests; solo-versus-co-op comparison if both are in scope; feasibility spikes (generation, lighting, networking if co-op) | S4 After first play | NOT RUN |
| **G3 Run slice and content cost** | Can the team afford a second area with representative presentation? | A measured second area; representative art, audio, UI at the chosen camera; saves and recovery | S5 Slice and production | NOT RUN |
| **G4 Production decision** | Does the evidence justify a full game? | Owner reviews results, costs, risks, alternatives; complete offer, team, budget, schedule | S5 Slice and production (exit) | NOT RUN |
| **G5 Alpha** | Is the full run playable from start to win? | Alpha build | S6 Release and after | NOT RUN |
| **G6 Release** | Fairness, recovery, accessibility, performance, saves and operations ready? | Release checklist evidence | S6 | NOT RUN |
| **G7 Stewardship** | What does real use show about content, reliability and cost? | Post-launch review | S6 | NOT RUN |

A game that also uses Multiplayer Adaptation runs that package's own G0-G7 alongside; record both, don't merge them. Passing a gate permits the next experiment. It doesn't authorize production, a release or more content.

## G0: experience clarity

1. **Desk audit.** Trace one floor from the [floor spec](../templates/FLOOR_SPEC.md): four runs (clean descent with a hard choice, a different plan that works, weak start that recovers, understandable death) and the two dominance policies (dive, clear every floor). Fill the threat-and-tell table: every way to die has a tell, a counter and a shown cause. Record ambiguous rules instead of resolving them on the fly. This checks consistency only.
2. **First read.** With a few first-time players from the declared audience (six is a common small number), give the same short briefing, then ask before they start: what are you looking for, what's dangerous here, and how do you get down? Then let them play the first minutes. Don't coach.

Proposed acceptance (adjust before testing):

- Every blocking ambiguity found in the desk audit has an explicit rule and a rechecked trace.
- Every way to die on the floor has a tell, a counter and a shown cause.
- Neither dominance policy ends better than the best traced plan, or the brief says why that's acceptable for this floor.
- At least 5 of 6 players can name one danger and one way down without help.

## G1: descent loop value

The first played session, by anyone including the developer, written up in a validation report, is the S3 gate (D-011 (3)). G1 continues from there.

Use one floor. Compare two death-and-carry-over models (DG-05, DG-06) on the same layout. Log every descent (when, in what state, why, in the player's words), every unknown item tested and how, every death with its last warning, and minutes spent in menus.

Proposed acceptance:

- Most players can explain why they went down when they did, in terms of the floor (food, the hunter, health), not "it said to".
- Descent timing differs between players or runs for reasons they can name (R8, R9).
- Most players can explain their death and name the warning (R1).
- After a death, most players want another run and can say what they'd change (R2, R7).
- No chore system is named "pointless" by most players (R3).

## G2: repeat, dominance and co-op

- Returning players play a short run of floors, including one changed floor.
- Run R8 (dive), R9 (clear every floor) and R12 (one best build) as desk or bot policies, with fixed caps.
- If solo and co-op are both in scope: compare the same floors in each (R6).
- If co-op: run Multiplayer Adaptation's G1-G2 alongside; log decisions per player and dead-player waiting time (R5).
- Feasibility spikes chosen with Tech Choice: floor generation within its rules, lighting and darkness at target hardware, and networking if co-op (R14).

Proposed acceptance: no single policy ends best on every floor without reading it; deeper floors bring at least one new kind of decision; solo isn't clearly worse; each feasibility spike works on target hardware or the design is reduced.

## G3 to G7

G3 is a run slice, from character choice through several floors to a death or a win, with representative art at the chosen camera, plus the measured cost of a second area (see [content and presentation](CONTENT_AND_PRESENTATION.md)). G4 is the owner's production decision on the complete offer. G5-G7 are alpha, release and stewardship.

## Revision triggers

| Observation | Problem | Change |
| --- | --- | --- |
| Everyone dives | Floors give too little | Add a shortage only exploring fixes |
| Everyone clears every room | Nothing pushes on | Add a clock, a hunter or growing danger |
| Players can't explain deaths | Missing tells | Add tells and a cause screen before content |
| First-timers quit early | Learning wall | Gentler first area; teach in play |
| Players skip a system or call it busywork | Chore | Cut, automate or give it a decision |
| Players quit after a long run is lost | Death costs too much | Try another carry-over model or shorter runs |
| Dead co-op players wait | No role after death | Multiplayer Adaptation's revive or spectator rules |
| Late floors feel the same | No new decisions deeper | New interactions per area, not bigger numbers |

[Decisions](DECISIONS.md) · [Validation report](../templates/VALIDATION_REPORT.md) · [Package home](../README.md)

---

Project Scaffold · created by Carter David Long (Bigfootcdl), with the Claude chat team working under their direction.
