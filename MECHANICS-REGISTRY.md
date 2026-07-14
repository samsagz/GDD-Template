# MECHANICS-REGISTRY.md — TestGame

> **This is a hand-copied mirror of the mechanics defined in the GDD repo at `TBD`.**
> No GDD repository exists yet, so there is currently nothing upstream to mirror and
> this file is acting as the source of truth by default. Once a GDD exists, this file
> becomes a *copy* of it and **WILL drift out of sync**. It is not automatically
> synchronized with anything.
>
> This file is the **local source of truth** for what mechanics exist. A puzzle may
> only use mechanics listed here.

**Last verified against the GDD:** 2026-07-13
_(No GDD exists yet; this date records when the registry was last authored/checked.
Update it — and this line — every time you verify the registry against the GDD.
If it is more than a month stale, that is a problem worth surfacing.)_

---

> ⚠️ **DEMO NOTE:** The definitions below were authored by the assistant to make the
> example coherent. They are **not** design decisions provided by the game owner.
> Replace them with real, GDD-backed definitions before this repo is used for actual
> level design.

## Mechanics

### Push
The player can push a single block one tile in the direction they are facing. Cannot
pull. Cannot push a block that has another block or a wall directly behind it. A block
pushed over a ledge falls and is destroyed.

### Walk
Default locomotion; one tile per step. Blocked by walls, blocks, and closed doors.

### Run
Hold to move at double speed. Lets the player cross a crumbling tile before it
collapses, which walking does not.

### Point-and-click: examine/use
Click a world object to interact: pick up loose items into an inventory, or use a
held item on a target object (e.g. use a key on a door).
