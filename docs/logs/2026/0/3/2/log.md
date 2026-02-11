## 10cd96d
Merge pull request #4 from MCEngine/fix/crafting-gui-drop-q. Brings the crafting drop-behavior fixes into main via PR.

## e22ac54
fix: Allow item drops outside crafting GUI, only block during crafting view. Restricts `ItemDropProtectionListener` to the crafting GUI and permits normal drops elsewhere, including the editor.

## 9f21a30
fix: allow Q craft drop only in crafting view. Prevents drop actions (Q/drag) from cancelling outside the crafting view, while keeping protections inside.

## b887e7a
Merged PR #3 (project iteration 2). Integrates the second iteration improvements into the codebase.
