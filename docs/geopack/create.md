# Create a pack

You can turn any Geometry Nodes modifier into a GeoPack tool, then share the pack as a `.geopack` file.

## 1. Create the pack

1. In **Preferences > GeoPack**, set the packs location if needed.
2. Click **Create New Pack** and fill in:
    - **Pack Name**, **Pack Author(s)**, **Description**, **Pack Version**, **Pack URL**
    - **Oldest Blender Version Compatible**
    - **Pack License**: Royalty Free, CC0, CC-BY, GPL or MIT
    - **Pack Location**
3. Click **Create !**.

## 2. Add a modifier to the pack

1. In the 3D Viewport, select the object (mesh or curve) that has your Geometry Nodes modifier.
2. In the modifier stack, click the modifier to save so it becomes active (blue outline).
3. Press **J** and choose **New GeoPack Modifier** (About section). With [Node to Panel](node-to-panel.md), the BagaPie panel also has a **Save as GeoPack Modifier** button.
4. In the dialog, choose the pack (**Add to pack**), fill in the information and define how the tool is set up (see below).
5. Click **OK**.

The tool now appears in the GeoPack pie menu (**V**).

The modifier name comes from its node tree name, without the `BP_` prefix if there is one. If the name is already used, BagaPie asks you to rename the node tree, or to **Override** the existing modifier.

### Information

**Modifier name**, **Author(s)**, **Description**, **Modifier Version**, **Minimal Blender version**, **Contact**, **URL**, **NodeTree License**.

### Usage: how the tool is set up

This defines what the user must select and what happens when they click the tool.

**Active Object Must Be**

| Option | Behavior |
| --- | --- |
| **Mesh**, **Curve**, **Mesh or Curve** | The tool is grayed out unless the active object has this type. The modifier is added to it |
| **None - Create new object** | Ignores the selection and creates a new object, mesh or curve |

Depending on the choice, extra options appear:

- **New mesh:** **Switch to Edit Mode and enable Add Cube tool**.
- **New curve:** **Switch to draw curve mode**, with **Curve Mode** (2D / 3D) and **Curve Projection** (Cursor / Surface).
- **Existing mesh:** **Switch to Weight Paint** (a new vertex group is created and assigned to an attribute input of your modifier), or **Add Hair Curves**.
- **Add Curve and switch to draw mode:** a new curve is created and plugged into an object input of the modifier.

**Use Selection**

Uses the other selected objects. Choose which object types are accepted (**Mesh**, **Curve**, **Camera**, **Empty**, **Text**, **Volume**, **Light**), the **Collection Name** and the **Collection Input** of the modifier that receives them. **Allow asset browser selection** adds an Asset Browser button to the tool.

The dialog summarizes the result under **How your modifier will work**. The same summary is shown to users in the pack details.

## 3. Icons

Each modifier can have an icon in the pie menu. In the pack details, use **Add Icon**, the remove button, or the refresh button. Icon size in the pie menu is set by **GeoPack Icon Scale** in the preferences.

## 4. Assets

A pack can include its own asset library:

1. In the pack details, open **Assets** and click **Create Asset Library**.
2. Click **Add blend file to Pack's Assets Library** to add `.blend` files.

The library is created automatically for users who install the pack.

## 5. Edit, export, delete

- **Edit:** the pencil icons edit the pack information or a modifier.
- **Export:** the export icon saves the pack as a `.geopack` file to share.
- **Delete:** deletes the pack or a modifier. Deleting a pack also deletes all assets linked to it, and cannot be undone. Keep a copy.

Save your preferences after creating or moving packs.
