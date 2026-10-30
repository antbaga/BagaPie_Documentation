# Node to Panel

Node to Panel turns the inputs of your own Geometry Nodes modifiers into a clean interface in the BagaPie panel. You organize inputs with prefixes. It is useful for complex node trees and for GeoPack tools, but works without GeoPack too.

<div class="video"><iframe src="https://www.youtube-nocookie.com/embed/9bV6AArrWeM" title="BagaPie V9 GeoPack - Nodes to Panel" loading="lazy" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; fullscreen" allowfullscreen></iframe></div>
<p class="video-caption">Video: <em>BagaPie V9 GeoPack - Nodes to Panel</em>.</p>

## Display a modifier

Add `BP_` at the beginning of the **node tree** name (not the modifier name). The modifier then appears in the BagaPie panel of the object.

In GeoPack, the tool is named after the node tree, without `BP_`.

## Prefixes

Add prefixes to the input names. A prefix ends with `_`, followed by the displayed name. Prefixes can also be written in the input description: right-click an input in the node group interface and use the **BagaPie Node to Panel** menu to add them.

| Prefix | Displays |
| --- | --- |
| `V_` | A value (any input type) |
| `L_` | A label |
| `P_` | A button (boolean input) |
| `P1_` … `P9_` | A button with an identifier from 0 to 9, which can show or hide other inputs |
| `1V_` … | An input controlled by button 1 (put the identifier first) |
| `C_` | The curve of a Float Curve or Color Ramp node: the input name must match the node name or label |
| `S_` | A separator; add the size after it |
| `URL_` | A button that opens a link. Use a String input and put the URL in its default value |
| `B_` / `B` | Create a new box / add to the previous box |
| `R_` / `R` | Create a new row / add to the previous row |
| `2_` (any integer) | Scale the input or button |

Prefixes combine. Examples:

| Input name | Result |
| --- | --- |
| `B_L_MyLabelName` | A new box with a label |
| `P_MyButtonName` | A switch button |
| `R_V_MyValueName A`, then `RV_MyValueName B` | Two values on one row |
| `P1_Hit me !`, `1V_MyValueName_A`, `1V_MyValueName_B` | A button that shows or hides two values |

Boxes and rows can be nested.

## Tips

- Inputs are displayed in order, from top to bottom.
- Float Curve and Color Ramp nodes appear at the position of their input, but their relative order is not controllable. If several nodes share the same name or label, they are all displayed. Rename a node with **F2**.
- Hide inputs that are only used for layout (labels, separators) in the modifier.
- Shader node groups using the same prefixes are displayed too, under the object's materials.
- At the bottom of the panel, **Save as GeoPack Modifier** adds the modifier to a pack, with its interface. See [Create a pack](create.md).

The prefix list is also in **Preferences > Nodes to Panel**, with examples.
