# Edit Mode Pie (D)

In Edit Mode on a mesh, select faces or edges and press **D**. These tools are Geometry Nodes tools that only affect the selection.

| Position | Section | Tools | Select |
| --- | --- | --- | --- |
| Left | **Architecture** | Window Modern, Window Classic, Door Simple, Door Double, Cable Creator | Faces (Cable Creator: edges) |
| Top | **Generate** | Face to Grid, Face to Paving, Face to Perforated Grid, Face to Plank | Faces |
| Right | **Edit Mesh** | Bool Through, Tessellate, Insert Circle | Faces |
| Bottom | **Array** | Array Along Shape, Bolt Corner | Faces or edges / faces |

The pie menu only opens when something is selected.

## Applied tools

Except Windows and Doors, these tools are **applied**. Adjust them in Blender's operator panel at the bottom left of the viewport. Once you click elsewhere, the panel disappears and the result is permanent, like any Blender Edit Mode operator.

Windows and Doors create a separate, parametric object. See [Windows & Doors](windows-doors.md).

## First use: setup and restart

The tools are stored in the **BagaPie Modifier** asset library (the Parametric Library). The first time, or after an update, the pie menu may show **SETUP TOOL !** or **Tool File missing !**:

1. Click **SETUP TOOL !** (or **Update BagaPie Parametric Library**).
2. Restart Blender. Until then, the pie menu shows **Restart Blender**.

This is needed only once. See [Asset libraries](../assets.md).

## Pages

- [Windows & Doors](windows-doors.md)
- [Face To patterns](face-to.md)
- [Mesh tools](mesh-tools.md): Cable Creator, Bool Through, Tessellate, Insert Circle, Array Along Shape, Bolt Corner
