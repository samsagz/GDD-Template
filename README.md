# TestGame — Level Design List

This repository defines the **puzzles** of *TestGame*: one file per puzzle, each
specified precisely enough that a developer can build it without asking questions.

## What this repo is
- **`MECHANICS-REGISTRY.md`** — the local source of truth for what mechanics exist.
- **`levels/INDEX.md`** — the table of every puzzle. Start here.
- **`levels/PUZZLE-TEMPLATE.md`** — the canonical template every puzzle file copies.
- **`levels/MECHANIC-COVERAGE.md`** — reverse index: which puzzles use / introduce
  each mechanic.
- **`levels/<group>/`** — the puzzle files, grouped by chapter.
- **`levels/EXAMPLE-do-not-ship.md`** — a single example showing the template in use.
  Not a real puzzle; do not ship.

## The Game Design Document lives elsewhere
The GDD is a **separate repository**: `TBD` *(no GDD repository exists yet)*.

**The two repos are NOT automatically synchronized.** `MECHANICS-REGISTRY.md` is a
hand-copied mirror of the mechanics defined in the GDD. It will drift. It carries a
`Last verified against the GDD` date that must be updated by hand whenever it is
checked.

## Status
Scaffold only. No real puzzles exist yet — just the template, the indexes, and one
clearly-labelled example. Mechanic definitions in the registry are demo placeholders
authored by the assistant, not final design.
