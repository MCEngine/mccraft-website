# MCCraft progress (2026/0/3/1)

## Scope
Changes from commit `46d17a2a09db6b509168bda9ea7c30c3d023d245` to latest.

## Highlights
- Added command system with subcommand manager, tab completion, and help/create/get/editor handlers.
- Introduced GUI layer (crafting editor list, crafting grid GUI) plus listener system to drive interactions.
- Implemented MCCraftProvider singleton and async wrappers to unify DB access and cache updates.
- Added database implementations for SQLite and MySQL, including type and recipe tables.
- Introduced RecipeCache for in-memory matching and fast lookups; refactored to store ItemStacks directly.
- Enhanced crafting flow: right-click crafting entrypoint, drag/drop guards, cursor stacking, ingredient consumption, and head-item checks.
- Normalized type names to lowercase across commands/provider/cache; added permission checks and duplicate-id protection.
- Misc fixes: avoid NPEs in recipe comparisons, keep cursor items when crafting, add missing imports and deprecation cleanups.

## Components touched
- Commands: central manager dispatching to registered subcommands with permission enforcement.
- GUIs: crafting editor and viewer inventories with filler slots, serialized recipes, and dynamic result slot updates.
- Listeners: crafting GUI interactions, drop/place protections, inventory close/save flows, right-click activation.
- Persistence: SQLite/MySQL schemas (mccraft_item, mccraft_type) with upsert/delete/read operations; type head items stored.
- Cache: RecipeCache hydrated on startup; mirrors writes and performs recipe matching per station type.

## Notes
- Requires PaperMC 1.21+, Java 21+.
- Head items are required for non-default crafting types and are decremented on craft.
