# Snap Asset

Snap Asset places assets one by one on a surface, where you click.

<div class="video"><iframe src="https://www.youtube-nocookie.com/embed/EKUg_FvDrgk?start=16" title="BagaPie 11 - Parametric Tools" loading="lazy" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; fullscreen" allowfullscreen></iframe></div>
<p class="video-caption">Video: <em>BagaPie 11 - Parametric Tools</em>, from 0:16.</p>

## Place assets

1. Select the assets to place.
2. Select the target surface **last**.
3. Press **J** and choose **Snap Asset** (or its **Asset Browser** button to use assets selected in the Asset Browser).
4. Click on the surface to add instances.
5. Press **Esc** to stop.

Until you press **Esc**, every click adds an instance. To add more later, click **Add Instances** in the BagaPie panel.

## Settings

| Setting | Effect |
| --- | --- |
| **Add Instances** | Resume placing instances |
| **Offset Z** | Lift or sink the instances along the normal |
| **Align Normal** | Align instances to the surface |
| **Random Rotation** | Random rotation per instance |
| **Scale Min / Max** | Random scale range |
| **Target / Instances** | The surface and the assets used by the modifier |

## Edit the placement

Each instance is a vertex of the Snap Asset object. In Edit Mode you can move, delete or duplicate them like any vertex. In the sidebar **Item** tab, a vertex's **Bevel Weight** and **Vertex Crease** drive the rotation and scale of its instance.

Visibility and removal work as for other modifiers, from the modifier stack.
