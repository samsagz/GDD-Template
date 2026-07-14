# C2-P01 — Example: Beat the Collapse
**Status:** draft
**Group:** chapter-02
**Position:** Critical path, step 3 (first puzzle of chapter 2).

> ⚠️ **EXAMPLE — DO NOT SHIP.** Placeholder content to demonstrate teaching order.

## Assumed knowledge
- **Walk**
- **Push** — from chapter 1.

## What this puzzle teaches
- **Run**: holding run lets the player cross a crumbling tile before it collapses;
  walking across it fails. This is the single new idea.

## Mechanics used
- Run
- Walk

## Setup
A straight corridor. The middle three tiles are crumbling tiles. The exit is on the
far side. There is no block and nothing to push here — the chapter deliberately drops
Push for one room to isolate Run.

## Intended solution
1. Stand at the near edge of the crumbling stretch.
2. Hold **Run** and cross all three crumbling tiles in one continuous dash to the exit.

## Known alternate solutions
- None intended. Walking onto a crumbling tile drops the player (see failure states).

## Failure states
- Walking (not running) onto a crumbling tile: it collapses and the player falls —
  a **lose**, resets to room start. Not a soft-lock: the room resets cleanly.
- Stopping mid-dash on a crumbling tile: same fall. Lose, clean reset. Fine.

## Open questions
> **OPEN:** Is a single dash enough to teach Run, or does the player need a second beat
> to internalize "hold to run"? (Placeholder.)
> **OPEN:** Does dropping Push entirely for this room hurt pacing? Check against the
> critical path.
