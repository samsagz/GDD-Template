# P-000 — Example: The Locked Antechamber
**Status:** draft
**Group:** chapter-01
**Position:** Illustrative example only — NOT on the critical path. Do not ship.

> ⚠️ **This file exists to show the template in use. Every value below is obviously
> placeholder content. Delete this file before shipping.**

## Assumed knowledge
- **Walk** — the player already knows how to move around a room.

## What this puzzle teaches
- **Push**: that a block can be pushed one tile but never pulled. This is the one new
  idea. (Placeholder — a real teaching puzzle would isolate this idea cleanly.)

## Mechanics used
- Push
- Walk
- Point-and-click: examine/use

## Setup
A 5×5 stone room. A single pushable block sits in the center. A locked door is on the
north wall. A key lies on the floor in the southwest corner. A one-tile ledge (drop)
runs along the east wall.

## Intended solution
1. Walk to the southwest corner and click the key to pick it up.
2. Walk to the block and push it one tile north so it no longer blocks the path.
3. Walk to the north door and use the key on it to open it.
4. Exit north.

## Known alternate solutions
- Pushing the block east over the ledge destroys it and also clears the path.
  **Acceptable** — it clears the route without breaking anything.
- Reaching the door without moving the block at all, if pathing allows.
  **Bug** — if the block was never an obstacle, the push is untaught. Flag for redesign.

## Failure states
- Pushing the block north into the corner with a wall behind it: the push simply
  fails (per registry, cannot push against a wall). No loss, no soft-lock. Fine.
- Pushing the block so it seals the only path to the key before picking the key up:
  **SOFT-LOCK — this is a bug.** The room must not allow the key to become
  unreachable. Flag for redesign.

## Open questions
> **OPEN:** Should the key be required at all, or does it just pad the example? A real
> puzzle would cut anything that doesn't serve the one idea being taught.
> **OPEN:** Does destroying the block over the ledge leave the player unable to
> re-teach Push later? Check teaching order against the critical path.
