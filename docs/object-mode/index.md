# Object Mode Pie (J)

Press **J** in Object Mode. The pie menu groups the procedural tools by section.

| Position | Section | Tools |
| --- | --- | --- |
| Top | **Scattering** | Scatter, Scatter Paint, Snap Asset (each with an Asset Browser button), Ivy |
| Top left | **Deformation** | Displace, Instances Displace, Deform |
| Top right | **Effector** | Point Effector, Camera Culling (only when the active object has a scatter) |
| Left | **Array** | Line, Grid, Circle, Curve, Curve Deform, Draw (+ Asset Browser), Array Along Shape |
| Right | **Architecture** | Wall, Wall Brick, Window, Pipes, Column, Tiles, Beam Wire, Beam, Stair Linear, Stair Spiral, Floor, Handrail, Cable, Fence, Siding, Paving, Grid, Perforated Grid, Plank |
| Bottom | **Boolean** | Union, Difference |
| Bottom left | **Manage** | Create Group, To Instance, Ungroup, Group to Instance, Proxy, Save as Asset, Save Material |
| Bottom right | **About** | Tutorials, Documentation, New GeoPack Modifier |

You can hide tools you never use in **Preferences > Pie Menu Tools**. Save as Asset, Save Material and the old Window tool are hidden by default.

## What to select

| Tool | Select | Object type |
| --- | --- | --- |
| [Displace](deformation.md) | One object | Mesh |
| [Instances Displace](deformation.md) | One object with instances on it | Mesh or curve |
| [Deform](deformation.md) | One object | Mesh |
| [Line / Grid / Circle array](array.md) | One object | Mesh or curve |
| [Curve array](array.md) | Objects, then a curve as active object | Mesh and curve |
| [Curve Deform](array.md) | Objects, then a curve | Mesh and curve |
| [Draw array](array.md) | One or more objects | Mesh |
| [Array Along Shape](array.md) | Objects, then the surface to follow | Mesh |
| [Proxy](manage.md) | One or more objects | Mesh |
| [Group](../group.md) | One or more objects | Mesh or curve |
| [Scatter / Scatter Paint](scatter.md) | Assets, then the target surface | Mesh |
| [Snap Asset](snap-asset.md) | Assets, then the target surface | Mesh |
| [Ivy](ivy.md) | One or more target objects | Mesh |
| [Point Effector](effectors.md) | Effector object(s), then a surface with a scatter | Mesh |
| [Camera Culling](effectors.md) | A camera, then a surface with a scatter | Camera or empty |
| [Wall](architecture.md) | One object | Mesh (edges) |
| [Wall Brick](architecture.md) | One object | Mesh (edges) or curve |
| [Pipes](architecture.md), [Cable](architecture.md) | One or more target objects | Mesh |
| [Handrail](architecture.md), [Fence](architecture.md) | A curve, or nothing | Curve |
| [Siding](architecture.md) | One object | Mesh |
| [Paving, Grid, Perforated Grid, Plank](architecture.md) | One object | Mesh (faces) |
| [Column, Tiles, Beam, Beam Wire, Stairs, Floor](architecture.md) | Nothing; a new object is created at the 3D cursor | — |
| [Boolean](boolean.md) | One object | Mesh |

A grayed-out button means the active object does not match the tool. Most tools need an active mesh; some need a curve.
