# Sources and research pointers

- **Compiled:** 2026-10-23.
- **Status:** reference games with PROPOSED interpretations, and pointers to the research library. No player study, no market forecast, nothing copied in (D-012).
- **Owner / refresh:** the adopting project's research lead; refresh before an audience, competitor, platform or commercial decision.

## How the reference-game notes were made

The notes below are the writing chat's summary from its general knowledge, given to bigfootcdl in the build chat before this scaffold was written (A1 in [PROVENANCE.md](../PROVENANCE.md)). **No store page, review, interview or game was opened in this job**, so every row is unverified. Treat them as starting hypotheses to check, not facts. Details such as dates, player counts and add-on contents changed across updates.

## Barony: the main reference

A first-person 3D roguelike dungeon crawler by Turning Wheel (Steam, 2015; later on consoles), inspired by NetHack and Ultima Underworld, with solo play or co-op for up to 4 players online or on LAN, friendly fire on, and open-source code (the art and sound are not open).

**What players liked (to check):** co-op chaos and the stories it makes; deep interacting systems (hunger, unknown items, curses, light, allies, shops, traps, crafting); many classes and races that play differently; real danger; high replay value.

**What players disliked (to check), and where this scaffold answers it:**

| Complaint | Where it's answered here |
| --- | --- |
| Hard to learn; little teaching; deaths without understanding | DG-16, R2 |
| Clunky controls, menus and inventory, especially on controller or console | R4; Game UI and Control Mapping |
| Unfair deaths: cursed items, unknown potions, traps, out-of-depth monsters | DG-17, DG-09, R1 |
| Multiplayer connection problems, desync, bugs after updates | R14; Multiplayer Adaptation and Tech Choice |
| Dated look | Art Design; [content and presentation](../docs/CONTENT_AND_PRESENTATION.md) (readable over detailed) |
| Weaker solo than co-op | DG-04, R6 |
| Nothing carries over between runs; quitting after a long run lost | DG-06, R7 |
| Chores: hunger, item wear, identification; the timed hunter | DG-18, R3, R11 |
| Unbalanced classes and races | DG-10, R12 |
| Content split into paid add-ons | DG-22; [content and presentation](../docs/CONTENT_AND_PRESENTATION.md) "Scope to resist" |

## Similar games

Contrasts only: what each is known for and what it doesn't show. None of this says a mechanic sells, retains players or would work in a given game. All unverified in this job.

| Game | Kind | Worth studying for | Known complaints / limits |
| --- | --- | --- | --- |
| NetHack (1987) | Turn-based, text-based roguelike | Depth: almost anything you try does something; the source of hunger, unknown items, curses and shops | Very hard to learn; looks ancient |
| Ultima Underworld (1992) | First-person 3D dungeon game | A living underworld; more than one way to solve a problem | Old controls |
| Arx Fatalis (2002) | First-person dungeon RPG | Drawn spell symbols; cooking and crafting; atmosphere | Bugs; fiddly spell drawing |
| Legend of Grimrock 1 and 2 | Grid-based first-person party crawler | Hand-made puzzle floors; polish | No co-op; little replay value |
| Delver | First-person pixel roguelike | A simple, solo take on a Barony-like run | Runs out of depth |
| Ziggurat 1 and 2 | First-person shooter roguelite | Fast magic combat; unlocks across runs | Shallow |
| Underworld Ascendant (2018) | First-person dungeon game | A warning: big ambitions without polish | Bugs, weak AI, unclear goals |
| Dark and Darker | First-person multiplayer dungeon extraction | Tension; rival parties | Harsh for beginners; cheating and legal trouble |
| Dungeon Crawl Stone Soup | Turn-based roguelike | Cutting tedium on purpose (no hunger busywork, easy identification); fair difficulty | Traditional look |
| Brogue | Turn-based roguelike | Depth from simple controls; interacting terrain | Small scope |
| Caves of Qud | Turn-based sci-fi roguelike | Deep simulation and stories | Overwhelming for newcomers |
| Shattered Pixel Dungeon | Turn-based mobile roguelike | Short runs; clear menus on a phone | Small screen limits |
| Spelunky 2 | Platformer roguelike, co-op | Interacting systems; fair, readable deaths | Messy co-op; lag |
| Risk of Rain 2 | Co-op action roguelite | Unlocks across runs; co-op that scales | Gets chaotic late |
| Noita | Simulated-pixel roguelite | Surprising, memorable deaths; wand building | Very hard |

Selected precedents carry survivorship bias. They show these combinations have been made; they don't isolate what caused any success or show demand for this scaffold.

## Research library entries to read

In tool-bag's [library-scaffold](https://github.com/HeartwaveTheory/tool-bag/blob/main/library-scaffold/INDEX.md). Starting points; this scaffold doesn't inherit their concepts, settings, numbers or approvals.

| Entry | What it holds | How it's used here |
| --- | --- | --- |
| [Co-op design lessons](https://github.com/HeartwaveTheory/tool-bag/blob/main/library-scaffold/craft/design/2026-10-22-coop-design-lessons/README.md) | Downed-not-dead, threat split, two-layer pacing, partner verbs, splits (from web-search summaries) | DG-05 (downed states), DG-08 (pacing a pressure), R5, the example's D7 (splitting) |
| [Co-op networking for a small team](https://github.com/HeartwaveTheory/tool-bag/blob/main/library-scaffold/craft/tech/2026-10-22-coop-networking/README.md) | Netcode, relays and testing for small teams | R14; hand-off to Tech Choice and Multiplayer Adaptation |
| [Playtesting and player research](https://github.com/HeartwaveTheory/tool-bag/blob/main/library-scaffold/craft/design/2026-10-22-playtesting-and-player-research/README.md) | Running small playtests, consent, think-aloud, metrics | The gate procedures and the validation report |
| [Interface design for complex games](https://github.com/HeartwaveTheory/tool-bag/blob/main/library-scaffold/craft/interface/2026-10-20-interface-design/README.md) | UI guidance and an evaluation protocol | R4, the information hierarchy |
| [October 2026 roguelike market scan](https://github.com/HeartwaveTheory/tool-bag/blob/main/library-scaffold/archive/notes_pvt/main/research/2026-10-roguelike-market-scan.md) (archived) | Roguelite demand signals and design lessons (Rogue Legacy and others) | Background for DG-06 (carry-over); its market figures are not refreshed or relied on |

## Next research

What the research library should cover, filed by its own rules ([FILING.md](https://github.com/HeartwaveTheory/tool-bag/blob/main/library-scaffold/FILING.md)); no work done here:

1. **Verify the Barony notes:** official store page, the developer's update notes and add-on pages, and a sample of player reviews, as a dated library entry.
2. **Fair death in roguelikes:** developer talks and post-mortems on tells, identification and "unfair" deaths (NetHack, DCSS, Brogue, Spelunky).
3. **Carry-over between runs:** how roguelites choose between knowledge, unlocks and power, and what players say about each.
4. **First-person readability in the dark:** lighting, sound direction and accessibility settings in first-person dungeon games.
5. **Co-op roguelike design:** what dead players do, friendly fire, loot sharing, solo scaling.
6. **Procedural floors from hand-made rooms:** generation rules and testing in shipped games.
7. **Inventory and menus on controllers** in item-heavy games.

[Package home](../README.md)

---

Project Scaffold · created by Carter David Long (Bigfootcdl), with the Claude chat team working under their direction.
