# C1-P02 — Example: Push, Not Pull
**Status:** draft
**Group:** chapter-01
**Position:** Critical path, step 2 (immediately after C1-P01).

> ⚠️ **EXAMPLE — DO NOT SHIP.** Placeholder content to demonstrate teaching order.

## Assumed knowledge
- **Walk**
- **Push** — taught in [C1-P01](C1-P01-do-not-ship.md). The player knows a block moves
  one tile when pushed.

## What this puzzle teaches
- Nothing new mechanically. It **tests** the *limit* of Push — that you cannot pull —
  by punishing a player who pushes a block into a dead end.

## Mechanics used
- Push
- Walk

## Setup
A 4×4 room. A block starts one tile from the north wall. The exit is west. A ledge
(drop) runs along the east wall.

## Intended solution
1. Walk to the east side of the block.
2. Push it one tile west, then continue around to reach the exit.

## Known alternate solutions
- Push the block east over the ledge; it falls and is destroyed, clearing the room.
  **Acceptable** — the goal is a clear path, and the registry says a block over a ledge
  is destroyed.

## Failure states
- Pushing the block **north** against the wall wedges it in a corner. Since the player
  cannot pull, the block is now stuck there permanently. This does **not** block the
  exit, so it is a wasted move, not a soft-lock. Waste of time, not a bug.

## Open questions
> **OPEN:** Does this puzzle actually test "no pull," or can the player brute-force
> their way out by shoving the block over the ledge every time without understanding
> the limit? (Placeholder — this is the kind of dominant-strategy concern to resolve.)
