# Mesh tools

All tools on this page are applied: adjust them in the operator panel (bottom left) before clicking elsewhere.

<div class="video"><iframe src="https://www.youtube-nocookie.com/embed/NYiU-bJsxK0?start=185" title="BagaPie 11 - Edit Mode Tools" loading="lazy" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; fullscreen" allowfullscreen></iframe></div>
<p class="video-caption">Video: <em>BagaPie 11 - Edit Mode Tools</em>, from 3:05.</p>

## Cable Creator

Creates cables from selected **edges**.

1. Select edges.
2. Press **D** and choose **Cable Creator**.

The main setting is the deformation: increase its intensity and adjust the **frequency**. A higher frequency gives fewer deformations along the cable, a lower one a more chaotic cable. Change the **seed** for variations. The cable deforms according to the surface.

## Bool Through

Cuts a hole through the mesh from the selected faces.

1. Select the faces.
2. Press **D** and choose **Bool Through**.

The faces are projected onto the opposite side of the mesh, along their average normal. It also works on complex shapes, such as beveled faces. If the boolean looks unfinished, increase the **offset**.

## Tessellate

Replaces faces with an object of your choice.

1. Select the faces (quads only).
2. Press **D** and choose **Tessellate**.
3. In the operator panel, pick the mesh to use.

The object's origin determines where it is placed relative to each face.

## Insert Circle

Inserts a circle into any face: triangle, quad or n-gon.

Settings: rotation, number of sides, offset and radius. The radius is not set automatically; adjust it for small or large scales.

## Array Along Shape

Repeats part of a mesh along the closest surface of the same object, and deforms it.

1. Join the element to repeat and the surface into one object.
2. In Edit Mode, select only the faces to repeat.
3. Press **D** and choose **Array Along Shape**.

Enable **Snap Deform** to deform the repeated mesh along the surface. On curved surfaces, increase the precision. Unlock the axes to rotate the array axis.

A parametric version, working with separate objects, is in the [Object Mode pie](../object-mode/array.md#array-along-shape).

## Bolt Corner

Adds bolts or screws in the corners of the selected faces.

Settings: **Offset** to move them toward the face center, the bolt or screw type, and **Custom Object** to use your own asset.
