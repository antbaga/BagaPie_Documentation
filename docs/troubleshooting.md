# Troubleshooting

## Everything disappears when I apply a modifier

Apply BagaPie modifiers from the BagaPie panel (**N**): click **✓** in the modifier stack. BagaPie applies all the modifiers that belong together. Modifiers have an order: apply the ones above yours first.

## My scatter or ivy is not stable during an animation

Scatter and ivy positions are computed from the surface area of the target. If the object is animated or deformed, its area changes, and so does the distribution. There is currently no solution for this in BagaPie.

## My scatter or ivy is different in the render

- Check that the surface does not change at render time, for example a different Subdivision level for the render.
- Check **% Viewport Display**: the viewport can show fewer instances than the render.

## The pie menu does not open

- **J** works in Object Mode, **D** in Edit Mode on a mesh with something selected, **V** in Object Mode.
- Check that your BagaPie version is compatible with your Blender version. See [Installation](getting-started/installation.md#which-version-for-which-blender).
- Check the shortcuts in **Preferences > Preferences > Menu Shortcuts**.

## The Edit Mode pie shows "SETUP TOOL !" or "Restart Blender"

Click **SETUP TOOL !**, then restart Blender. This is needed once after installing or updating. See [Asset libraries](assets.md).

## A tool is grayed out

The selection does not match the tool. Check what to select in [Object Mode Pie](object-mode/index.md#what-to-select), or in **Preferences > Pie Menu Tools**. For targets, select the target **last**.

## The Asset Browser button does nothing or is grayed out

- An Asset Browser must be open, with assets selected.
- Select assets in a specific library, not in **All**.
- Only **Object** and **Collection** assets are imported.
- The active object in the viewport must be a mesh.

## "Save in GeoPack" is grayed out

1. Open **Preferences > GeoPack** and set the packs location if asked.
2. Select your object (mesh or curve).
3. In the modifier stack, click the Geometry Nodes modifier to save: it gets a blue outline.

## Windows: shutters are missing

Shutters only work on quad faces; they are disabled on n-gons. If a few shutters fail, tweak **Min Height**. See [Windows & Doors](edit-mode/windows-doors.md).

## The boolean of a window or door does not cut the whole wall

The default is set for a 20 cm wall. Increase the wall thickness in the operator panel, or **Boolean Thickness** in the BagaPie panel.

## The Group shortcut is lost after restarting Blender

Click **Add Group Shortcut**, then save your preferences.

## Still stuck?

Ask on [Discord](support.md). Include your Blender and BagaPie versions, and a screenshot of the BagaPie panel if possible.
