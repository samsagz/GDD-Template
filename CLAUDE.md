# CLAUDE.md — TestGame Level Design List

## What this repo is
This repo defines the puzzles of **TestGame** — one file per puzzle, specified
precisely enough that a developer can build it without asking questions.

The **Game Design Document lives in a separate repository** at `TBD` *(no GDD
repository exists yet)*. **You cannot read it.** `MECHANICS-REGISTRY.md` is your
**only source of truth** for what mechanics exist. The two are not automatically
synchronized.

## Rules

### Reading
- **Always read `levels/INDEX.md` first.** Then read only the puzzle files relevant to
  the task. Do not bulk-read every puzzle.
- **Before designing any puzzle, read the puzzles that come before it on the critical
  path.** Difficulty and teaching order *are* the design. A puzzle judged in isolation
  is judged wrong.

### The template is law
- Every puzzle file follows `levels/PUZZLE-TEMPLATE.md` exactly. **No exceptions, no
  extra sections, no missing sections.**

### Mechanics
- A puzzle may **only** use mechanics listed in `MECHANICS-REGISTRY.md`.
- If the user describes a puzzle using a mechanic that is **not** in the registry,
  **STOP and tell them.** Either the mechanic is real (and both the GDD and the
  registry need updating) or the puzzle is wrong. **Do not silently accept it.**
- At the **start of a session**, if `MECHANICS-REGISTRY.md`'s
  `Last verified against the GDD` date is **more than a month old**, say so **once**,
  then move on.

### Keeping indexes in sync
- When a puzzle is **added or changed**, update `levels/INDEX.md` **and**
  `levels/MECHANIC-COVERAGE.md` in the **same change**.

### How to critique a puzzle
- **Do not tell the user a puzzle is "good."** Instead, tell them:
  - what its **dominant strategy** is,
  - whether it can be **brute-forced**,
  - whether it can **soft-lock** (soft-locks are bugs),
  - and whether it **teaches anything the player doesn't already know**.
