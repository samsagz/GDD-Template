# Mechanic Coverage — TestGame

A **reverse index** of MECHANICS-REGISTRY.md: for each mechanic, which puzzle
*introduces* it (teaches it for the first time on the critical path) and which puzzles
*use* it thereafter.

> **This file must be regenerated whenever puzzles change.** It is derived data, not
> hand-authored design. When you add, change, or cut a puzzle, rebuild this table from
> the puzzle files' "Mechanics used" and "What this puzzle teaches" sections in the
> same change.
>
> Its whole purpose is to surface two failures a per-puzzle view hides:
> - **A mechanic in the registry that no puzzle ever uses** — designed and abandoned.
> - **A puzzle that teaches nothing** — introduces no mechanic the player didn't
>   already know. That puzzle is a candidate to cut.

> ⚠️ Data below is derived from the **EXAMPLE** puzzles only (`*-do-not-ship.md`). It
> exists to show the coverage map working, not to reflect real design.

---

## Coverage table

| Mechanic                        | Introduced by | Used by                        |
|---------------------------------|---------------|--------------------------------|
| Push                            | C1-P01        | C1-P01, C1-P02, P-000          |
| Walk                            | — (never taught) | C1-P01, C1-P02, C2-P01, C3-P01, P-000 |
| Run                             | C2-P01        | C2-P01                         |
| Point-and-click: examine/use    | C3-P01        | C3-P01, P-000                  |

## Flags
- **Walk is never *introduced* by any puzzle** — it's used everywhere but assumed as
  pre-existing knowledge. That's defensible for base locomotion, but the coverage map
  is doing its job by surfacing it: if Walk has any non-obvious rule, some puzzle
  should teach it.
- **C1-P02 teaches nothing new** (introduces no mechanic). It *tests* the "no pull"
  limit of Push. That's a legitimate role, but this is exactly the kind of row to
  scrutinize: a puzzle that neither teaches nor meaningfully tests would be a cut
  candidate.
- **Run is used by exactly one puzzle** (C2-P01) and never revisited. A mechanic taught
  once and never reused is a candidate for either more puzzles or cutting the mechanic.
- **No unused mechanics:** all four registry mechanics appear in at least one puzzle.
