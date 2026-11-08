# Content, presentation and tone

**Status:** PROPOSED guidance, 2026-10-23. Aim: make floors readable, keep generated content in check, keep content cost under control, and let the project choose a tone for danger and death. **Owner:** the adopting designer with art, input and production owners. Basic cues are needed by G1; representative presentation and costs by G3.

## Floor grammar

A floor combines: rooms, at least two ways down, threats with tells, unknown things with signs, the leading pressure, and what the party lacks on arrival. Use the [floor spec](../templates/FLOOR_SPEC.md). Each addition should change a decision. Moving a potion from one room to another without changing what the party lacks, risks or must choose changes walking, not planning.

Variation that changes decisions:

- **What the party lacks on arrival** (food, light, health, a key).
- **Where help is relative to danger** (food behind the toughest fight; healing near the stairs).
- **The ways down** (one guarded, one hidden, one costly).
- **The leading pressure** (hunger, darkness, a hunter).
- **The unknown things** (one with a sign, one without; one helpful, one harmful).

Change one at a time when testing, so you can tell which change mattered.

## Generated content

If floors are generated (DG-07), build them from hand-made rooms, each holding a decision. Write the rules generation must never break (see [core systems](CORE_SYSTEMS.md) §3) and test them by generating many floors and checking each rule automatically. Keep a list of hand-made "set piece" rooms that make an area memorable. A generator that makes many floors that feel the same is worse than a few hand-made ones (R10).

## Information hierarchy

What the player must be able to read, most important first:

1. **Danger now:** what's about to hurt the party, and from where.
2. **The way down:** where the known ways down are and what they cost.
3. **What the party lacks:** health, food, light, the pressure clock.
4. **Unknown things:** what's been found, what's known, what the signs say.
5. **Party state:** who is hurt, hungry, cursed or blind; in co-op, where everyone is.

In first person most of this has to live in the world and in sound, not only the HUD. A top-down view can show more at once. The camera choice (DG-02) changes this list's costs; [Game UI](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/game-ui/PACKAGE.md) owns how it's shown.

## Readability rules

- Every threat has a tell before it lands: a sound with a direction, a shape, a mark on the floor, a wind-up.
- Every harmful unknown has a sign a careful player could notice, or a recoverable cost.
- The pressure clock is always visible or audible, with warnings before it bites.
- On every death, show the cause and the last warning.
- Darkness can hide treasure and set a mood; it must not hide the only tell of a deadly threat.
- Colour, sound or small detail must never be the only carrier of something a life depends on.

## Tone (DG-21): the project's choice

Dungeon games carry danger and death; many also carry dark comedy (Barony's co-op stories, NetHack's absurd deaths). No tone is chosen here. Options:

| Tone | A run feels like | A death feels like | Watch for |
| --- | --- | --- | --- |
| Grim and serious | A desperate descent | A real loss | Grim for its own sake; players quit |
| Darkly funny | Chaos and stories | A punchline you'll retell | Undercutting the danger |
| Heroic | A quest | A setback before the next attempt | Danger so soft the descent isn't a choice |
| Whimsical | An adventure | A pratfall | Too light to care |

Ways to keep death from being bitter or cheap, whatever the tone:

- **Make the cause clear.** A death the player understands is a lesson; one they don't is just bad.
- **Make the run count.** Show what the party achieved: floors reached, things learned, the best moment.
- **Get back in fast.** The time from death to the next run is part of the death's cost.
- **Decide what's never shown.** Write it in the brief.

## Art and audio

No style is chosen here. Keep silhouettes of monsters, players and items distinct in the dark and at the minimum display size. Sound tells need a direction and a visual equivalent for players who can't hear them. Use [Art Design](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/art-design/PACKAGE.md) to choose a style and check readability; a simple, readable style is better than a detailed, murky one.

## Input and accessibility

List the actions before mapping buttons, with how often each happens in a fight. Test drinking, swapping, dropping and giving items with each input during a fight (R4). First person brings motion-sickness costs: field-of-view and head-bob settings, a steady crosshair. Darkness brings brightness settings. Real time brings reaction-time costs: consider a slower mode or longer tells. Record these as design choices. [Control Mapping](https://github.com/bigfootcdl/nat-pod/blob/main/scaffold/packages/control-mapping/PACKAGE.md) owns bindings.

## Content cost

Build two areas before estimating a full run. For the second, record: room-building time, new monsters, new items and their interactions, new sounds, generation rules added, balance passes, and what broke in the first area. Item effects multiply across every class, monster, system and co-op combination; count them before adding more.

## Scope to resist

- More classes, races or items before the first ones each change a decision.
- More monster types to make a floor "harder" instead of changing what the party lacks or risks.
- Big generated floors where most time is walking.
- A meta-progression tree that hides a weak first floor.
- Selling core content as paid extras before the base run is complete (a common complaint about Barony's add-ons).
- Online co-op networking before one floor works (if co-op is chosen at all).

[Adversarial review](ADVERSARIAL_REVIEW.md) · [Gates](PRODUCTION_AND_GATES.md) · [Package home](../README.md)

---

Project Scaffold · created by Carter David Long (Bigfootcdl), with the Claude chat team working under their direction.
