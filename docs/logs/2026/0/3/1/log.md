## 3089ea1

Merge pull request #2 from MCEngine/feature/implement-plugin-logic.

## 2b107cc

chore: normalize type names to lowercase for commands/provider/cache.

## cbc4581

fix: add missing Map import for crafting listener.

## 6877db7

fix: keep cursor items when taking crafting result; stack or add to inventory.

## 86a1776

fix: avoid NPE warning in RecipeCache grid comparison.

## f1c7c86

refactor: store ItemStack directly in RecipeCache instead of Base64; deserialize only at boundary.

## 4f7ba46

feat: add RecipeCache for in-memory fast access; refactor crafting view to empty GUI with dynamic recipe matching.

## 1d02c10

feat: add right-click crafting, block place/drop prevention, fix deprecations, add item display name.

## 0f5c38d

chore: remove deprecated inventory titles and update listeners.

## d6a1253

fix: replace deprecated serialization with Paper NBT API, use Paper PlayerProfile for skulls, support hand item.

## 7ca9f99

Merge pull request #1 from MCEngine/feature/mccraft-refactor.

## d3887a5

fix: accept HDB head base64 and block duplicate recipe ids.

## 6975772

refactor: separate type registration from recipe creation, add mccraft_type table.

## 8881d54

chore: add permissions for editor and get commands.

## 103467d

fix: centralize create permission check in handler metadata.

## 704c235

feat: Wire up MCCraftPlugin engine with full system (DB, commands, listeners, provider).

## ba583cb

feat: Add listener system (CraftingGUI, EditorListGUI, ItemDropProtection listeners).

## b04dc3b

feat: Add GUI system (CraftingGUI, EditorListGUI) and utility classes (ItemSerializer, GUIConstants).

## e2ea875

feat: Add command system (Manager, TabCompleter, Help, Create, Get, Editor handlers).

## a4679e3

feat: Add MCCraftProvider central API singleton.

## fe2eb6a

feat: Add database implementations (MCCraftSQLite, MCCraftMySQL).

## 97121e7

feat: Add API interfaces (IMCCraftDB, ICraftCommandHandle).
