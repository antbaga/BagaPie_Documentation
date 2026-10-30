# How BagaPie works

## Select, press a key, pick a tool

<div class="video"><iframe src="https://www.youtube-nocookie.com/embed/-FqUbeQPQb4" title="BagaPie 11 - Introduction" loading="lazy" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; fullscreen" allowfullscreen></iframe></div>
<p class="video-caption">Video: <em>BagaPie 11 - Introduction</em>.</p>

BagaPie tools are launched from pie menus in the 3D Viewport.

1. **Select** the objects the tool needs. When a tool uses a target (a surface, a curve), select the target **last** so it becomes the active object.
2. Press **J** (Object Mode) or **D** (Edit Mode).
3. Click a tool. Grayed-out buttons mean the current selection does not match what the tool needs.

The selection depends on the tool:

| Tool needs | Examples |
| --- | --- |
| Nothing | Stair Spiral, Beam, Beam Wire: a new object is created at the 3D cursor |
| One object | Wall (mesh edges), Displace, Line Array, Proxy |
| Objects + a target selected last | Scatter, Snap Asset, Array Along Shape, Curve Deform |
| A curve, or nothing | Fence, Handrail: without a curve, BagaPie creates one and switches to Draw mode |
| Faces or edges in Edit Mode | Windows, Doors, Bool Through, Cable Creator |

The full list is in [Object Mode Pie](../object-mode/index.md) and [Edit Mode Pie](../edit-mode/index.md). It is also available in **Preferences > Pie Menu Tools**, with what each tool expects.

## The BagaPie panel

Open the 3D Viewport sidebar with **N** and select the **BagaPie** tab. Press **Ctrl + Alt + J** to open the same panel as a pop-up.

At the top, the **modifier stack** lists the BagaPie modifiers of the active object. Select one to display its settings below. Each line offers, depending on the modifier:

| Icon | Action |
| --- | --- |
| ✓ | **Apply**: convert the modifier result to real geometry. Use this button rather than Blender's Apply: BagaPie applies all the modifiers that belong together. |
| − | **Remove** the BagaPie modifier and its helper objects |
| Monitor / camera | Show or hide in the viewport / in renders |

Scatter layers, effectors and camera culling have extra icons in this list; see [Scattering](../object-mode/scatter.md).

When a [group](../group.md) is selected, the panel shows the group tools instead. Geometry Nodes modifiers prepared with [Node to Panel](../geopack/node-to-panel.md) are also displayed there.

The panel ends with links to the tutorial playlist and the documentation.

## Parametric and applied tools

- **Object Mode tools** add modifiers. Their settings stay editable in the BagaPie panel until you apply or remove them.
- **Edit Mode tools** run once on the selected faces or edges. You can tweak them in Blender's operator panel (bottom left) until you click elsewhere; then the result is permanent. **Windows and Doors** are the exception: they stay parametric.

## Collections created by BagaPie

BagaPie stores helper objects in a **BagaPie** collection, with sub-collections such as `BagaPie_Scatter`, `BagaPie_Boolean` or `BagaPie_Assets`. Avoid deleting them manually while the related modifiers are still in use; use the remove button in the BagaPie panel instead.

## Assets from the Asset Browser

Several tools have an **Asset Browser** button next to them (Scatter, Scatter Paint, Snap Asset, Draw array). It imports the assets selected in an open Asset Browser and runs the tool with them.

- Open an Asset Browser area and select one or more **Object** or **Collection** assets.
- Browse a specific library. The **All** library is not supported.
- In the viewport, select the target mesh, then click the **Asset Browser** button in the pie menu.

Imported assets are placed in the `BagaPie_Assets` collection.
