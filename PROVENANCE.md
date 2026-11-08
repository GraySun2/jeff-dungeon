# Where this scaffold came from

- **Name:** Dungeon
- **Source:** none standalone. This scaffold was **written fresh** in HeartwaveTheory/tool-bag, from research on Barony and similar games and by reading the scaffolds below. Nothing was copied unchanged; no research was copied (D-012).
- **Written on:** 2026-10-23, on branch `bigfootcdl/5-dungeon-scaffold` (tool-bag issue #5), from tool-bag `main` @ `f4f9e45`.
- **Asked for by:** bigfootcdl, directly, in a QC build chat (QC-dungeon); written by that chat.
- **Where it lives:** in tool-bag, at `scaffold/scaffolds/games/dungeon/`, with no standalone repo, like Tactical Extractions.
- **This copy:** copied into GraySun2/project-scaffold on 2026-10-23 from HeartwaveTheory/tool-bag `bigfootcdl/5-dungeon-scaffold` @ `e18329d` (tool-bag PR #6), on bigfootcdl's words "Let's put a copy into GraySun2/project-scaffold" (A6). Only links changed: links to this repo's own files are relative here instead of full tool-bag URLs; research library links still point at tool-bag's `library-scaffold/`. If the two copies drift, tool-bag's is the one the authority rows below were written for.
- **This repo's copy:** copied into GraySun2/jeff-dungeon on 2026-11-08 from bigfootcdl/nat-pod `scaffold/scaffolds/games/dungeon/` @ `7d4d734`, on Carter's words "Copy the dungeon scaffold from GraySun2/nat-pod into jeff-dungeon". The scaffold sits at this repo's root. Only links changed: links to files outside the scaffold folder now point at bigfootcdl/nat-pod on GitHub. `LICENSE` is the Scaffold's CC BY-NC 4.0 licence, copied unchanged.

## Authority

bigfootcdl's words in the build chat. These are not in [docs/DECISIONS.md](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/docs/DECISIONS.md), whose IDs only the chat Carter names assigns (D-063).

| ID | Date | bigfootcdl's words | Read as |
| --- | --- | --- | --- |
| A1 | 2026-10-23 | "we need to look into the game titled \"Barony.\" ... explain it to me in detail" and "what did people not like about barony? Tell me about the other titles in detail and even some other similar titles" | Research Barony, its weak points and similar games; this scaffold is built on that research. |
| A2 | 2026-10-23 | "Let's build this into a scaffold package / call it \"Dungeo\"", then "dungeon*" | A new scaffold from that research, named Dungeon. |
| A3 | 2026-10-23 | "put it into the HeartwaveTheory/tool-bag with the rest of the scaffolds there" | It lives in tool-bag's `scaffold/` folder. |
| A4 | 2026-10-23 | "you can read GraySun2/project-scaffold to see what i want you to do" | Follow the pattern the existing game scaffolds were made with (Tactical Extractions). |
| A5 | 2026-10-23 | "OK all" | All the chat's marked picks: level Advanced (draft); id `dungeon`; about 2 hours, stopping when this PR is open (step 1: the scaffold plus its plan, catalog, inventory and recommender rows; step 2, the package wrapper, after this merges); the chat opens the issue. |
| A6 | 2026-10-23 | "Let's put a copy into GraySun2/project-scaffold. It's getting a lot of new additions today" | Copy this scaffold, with its index rows, into GraySun2/project-scaffold through a pull request. |

## Sources

| Source | Repo @ commit | Used for |
| --- | --- | --- |
| [Tactical Extractions](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/scaffolds/games/tactical-extractions/README.md) (all files) | HeartwaveTheory/tool-bag `scaffold/scaffolds/games/tactical-extractions` @ `f4f9e45` | File layout; the adversarial review's shape (strongest objection, desk findings, R-numbered threats); two named dominance policies; the one G0-G7 gate ladder and its mapping; CHECKLIST and STOP_RULES shapes; the template shapes |
| [Extraction and Expeditions](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/extraction-expeditions/README.md) | GraySun2/scaffold-Extraction-Expeditions @ `1c53c7e` (original, not available), as packaged in tool-bag | Push your luck; one leading pressure before combining; loss models compared in pairs; three journeys; G0-G7 gates |
| [Multiplayer Adaptation PACKAGE.md](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/multiplayer-adaptation/PACKAGE.md) | GraySun2/scaffold-multiplayer-adaptation @ `c312083` (original, not available), as packaged in tool-bag | Only the ownership line, so this scaffold points to it instead of repeating it |
| [docs/MACRO_PLAN.md](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/docs/MACRO_PLAN.md) §1-§3; [docs/DECISIONS.md](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/docs/DECISIONS.md) D-011 to D-015, D-039 (7), D-055 (3); the GDD [CATALOG](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/scaffolds/gdd/docs/CATALOG.md) and [RECOMMENDATIONS](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/scaffolds/gdd/docs/RECOMMENDATIONS.md) | tool-bag @ `f4f9e45` | Stages S0-S6; Advanced level; `docs/design/` for game design files; how a new GDD question 1 answer is added |
| Reference games (Barony and others) and research library entries, listed in [research/SOURCES.md](research/SOURCES.md) | Reference games: the writing chat's general knowledge, not opened in this job. Library: tool-bag `library-scaffold/` @ `f4f9e45` | Pointers and interpretations only, not copied |

## What is new (not in any source scaffold)

The descent decision; fair-death rules; unknown things with checkable signs; systems that interact; the chore budget; carry-over between runs as a deliberate choice; generated floors with hand-made rooms and generation limits; solo and co-op both good; the "dive" and "clear every floor" dominance checks; an adversarial review built from Barony's player complaints; the Salt Cellars example (original setting and fixture numbers); DG- decision IDs.

## Re-checking

There is no copy to diff. To check the borrowing, open each source at the commit above and compare with the rows here. If a source changes, this scaffold doesn't update by itself.

---

Project Scaffold · created by Carter David Long (Bigfootcdl), with the Claude chat team working under their direction.
