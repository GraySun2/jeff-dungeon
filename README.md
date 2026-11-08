# Dungeon

**Status:** PROPOSED scaffold, 2026-10-23. Documentation only: no prototype, no play sessions, no gate passed. **Level:** Advanced (draft). **Decision owner:** the adopting project's owner.

**Opening question:** When the party is a few floors down, hurt, short on food and carrying things it hasn't identified, what makes "take the stairs now" and "explore this floor a little more" both real choices, and what makes a death feel fair enough that players start again right away?

Use this scaffold for games where one player or a small co-op group **goes down through a dangerous dungeon, floor by floor, learning how its systems work, until they win or die and start over**. The driving case is the first-person co-op roguelike crawler (Barony is the nearest reference), but the scaffold doesn't choose the camera: first person, third person, top-down, real time or turns are the adopting project's choice ([DG-02, DG-03](docs/DECISIONS.md)).

The loop it helps design: **pick a character → enter a floor → explore and read the floor → fight, sneak or avoid → find and test unknown things → manage food, light and health → choose when and how to go down → win, or die, learn and start a new run.**

This is a general scaffold, not any one game, and not a copy of Barony. No setting, audience, engine, numbers or player count is chosen here.

## Start here

1. Read [project status](PROJECT_STATUS.md) and the [framework method](FRAMEWORK_METHOD.md).
2. Work through [docs/START_HERE.md](docs/START_HERE.md) and produce its **First output**.
3. Fill in the [design brief](templates/DESIGN_BRIEF.md) and one [floor spec](templates/FLOOR_SPEC.md). The [worked example: The Salt Cellars](examples/THE_SALT_CELLARS.md) shows the level of detail.
4. Read [core systems](docs/CORE_SYSTEMS.md), then try to break the design with the [adversarial review](docs/ADVERSARIAL_REVIEW.md).
5. Pick the first gate in [production and gates](docs/PRODUCTION_AND_GATES.md) and record results in the [validation report](templates/VALIDATION_REPORT.md).
6. Check the [checklist](CHECKLIST.md) Exit list before calling the design stage done. [Stop rules](STOP_RULES.md) say when to stop and ask.

The [design atlas](docs/DESIGN_ATLAS.md) covers the whole game. [Content and presentation](docs/CONTENT_AND_PRESENTATION.md) covers readable floors, generated content, tone and content cost. [Decisions](docs/DECISIONS.md) lists every open choice (DG-01 onward). [Sources](research/SOURCES.md) lists the reference games and points at the research library.

## What it takes from each source

Built by reading the games below and two scaffolds in this repo, not copying them. Details and commits are in [PROVENANCE.md](PROVENANCE.md).

| From | What this scaffold takes | How it changes here |
| --- | --- | --- |
| Barony and its roots (NetHack, Ultima Underworld), as reference games | Descent floor by floor; permanent death; unknown items that can help or hurt; systems that interact (hunger, light, curses, allies, shops, traps); co-op where things go wrong in funny ways; something that hunts you if you stay too long | Each of these is an option with alternatives, not a rule. Barony's most common complaints (unfair deaths, a learning wall, chores, clunky menus, nothing carried between runs, weak solo play) become checks the design must pass ([adversarial review](docs/ADVERSARIAL_REVIEW.md)). |
| [Extraction and Expeditions](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/extraction-expeditions/README.md) | Push your luck; one leading pressure before combining several; loss models compared in pairs; three journeys (strong, weak that recovers, failed); G0-G7 gates | There is no trip home: the "return decision" becomes "go down now or keep exploring", and the loss is the whole run. |
| [Tactical Extractions](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/scaffolds/games/tactical-extractions/README.md) | The file layout; the adversarial review's shape; two named dominance policies; "agree thresholds before you look"; the one gate ladder | Search for people becomes reading a floor and testing unknown things; the two dominance policies become "dive for the stairs" and "clear every floor". |

## What is new here

Each of these is an open design choice with alternatives, not a rule. See [core systems](docs/CORE_SYSTEMS.md) and [decisions](docs/DECISIONS.md).

- **The descent decision:** stairs now, or more of this floor, with what the party knows, carries and lacks (DG-08).
- **Fair death:** every way to die has a tell, a counter and a cause the game shows afterwards (DG-17).
- **Unknown things:** potions, scrolls and gear that must be tested or identified, with checkable signs, so experimenting is a choice and not a coin flip (DG-09).
- **Systems that talk to each other:** fire, water, light, noise, hunger and allies affect each other, so players invent plans (DG-11).
- **Chores on a budget:** hunger, wear and identification each have to earn their place, or they go (DG-18).
- **What carries over between runs:** nothing, knowledge, unlocks or power, chosen on purpose (DG-06).
- **Generated floors that stay readable:** hand-made rooms inside generated layouts, and rules for what generation may never do (DG-07).
- **Solo and co-op both good:** co-op chaos without griefing or waiting; solo that isn't a worse version (DG-04, DG-15).

## Compose deliberately

This scaffold owns the run: floors, the descent, unknown things, character growth inside a run, death and what carries over. Other packages own their own parts, and this scaffold writes requirements for them instead of deciding them: [Multiplayer Adaptation](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/multiplayer-adaptation/PACKAGE.md) (co-op players: joining, dropping, revives, shared loot), [Control Mapping](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/control-mapping/PACKAGE.md) (buttons), [Game UI](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/game-ui/PACKAGE.md) (inventory, map, status screens), [Art Design](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/art-design/PACKAGE.md) (how a threat or an item reads), [Tech Choice](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/tech-choice/PACKAGE.md) (engine). Extraction and Expeditions can be a secondary for borrowing; one owning document per rule.

## Adopt

Copy the folder into the game repo, record the commit you copied, reset every decision to the game's own and every gate to NOT RUN. Write the game's design files under `docs/design/` (D-039 (7)). The example's setting and numbers are fixtures; replace them.

---

Project Scaffold · created by Carter David Long (Bigfootcdl), with the Claude chat team working under their direction.
