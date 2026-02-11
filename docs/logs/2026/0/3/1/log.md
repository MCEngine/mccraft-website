# MCCraft progress (2026/0/3/1)

## 97121e7

feat: Add API interfaces (IMCCraftDB, ICraftCommandHandle).

## fe2eb6a

feat: Add database implementations (MCCraftSQLite, MCCraftMySQL).

## a4679e3

feat: Add MCCraftProvider central API singleton.

## e2ea875

feat: Add command system (Manager, TabCompleter, Help, Create, Get, Editor handlers).

## b04dc3b

feat: Add GUI system (CraftingGUI, EditorListGUI) and utility classes (ItemSerializer, GUIConstants).

## ba583cb

feat: Add listener system (CraftingGUI, EditorListGUI, ItemDropProtection listeners).

## 704c235

feat: Wire up MCCraftPlugin engine with full system (DB, commands, listeners, provider).

## 103467d

fix: centralize create permission check in handler metadata.

## 8881d54

chore: add permissions for editor and get commands.

## 6975772

refactor: separate type registration from recipe creation, add mccraft_type table.

## d3887a5

fix: accept HDB head base64 and block duplicate recipe ids.

## 7ca9f99

Merge pull request #1 from MCEngine/feature/mccraft-refactor.

## d6a1253

fix: replace deprecated serialization with Paper NBT API, use Paper PlayerProfile for skulls, support hand item.

## 0f5c38d

chore: remove deprecated inventory titles and update listeners.

## 1d02c10

feat: add right-click crafting, block place/drop prevention, fix deprecations, add item display name.

## 4f7ba46

feat: add RecipeCache for in-memory fast access; refactor crafting view to empty GUI with dynamic recipe matching.

## f1c7c86

refactor: store ItemStack directly in RecipeCache instead of Base64; deserialize only at boundary.

## 86a1776

fix: avoid NPE warning in RecipeCache grid comparison.

## 6877db7

fix: keep cursor items when taking crafting result; stack or add to inventory.

## cbc4581

fix: add missing Map import for crafting listener.

## 2b107cc

chore: normalize type names to lowercase for commands/provider/cache.

## 3089ea1

Merge pull request #2 from MCEngine/feature/implement-plugin-logic.
