# Effectors

Effectors are extra masks for a scatter layer. They appear in the pie menu only when the active object has a BagaPie scatter; otherwise the section shows **No Scatter available**.

Both effectors apply to **one layer**: select that layer in the modifier stack first. With several layers, repeat the operation for each layer.

## Point Effector

Removes instances around objects, for example to keep rocks away from a house.

1. In the BagaPie panel, select the scatter layer.
2. Select the effector object(s), then the scattered surface **last**.
3. Press **J** and choose **Point Effector**.

| Setting | Effect |
| --- | --- |
| **Effector Collection** | The objects used as effectors |
| **Distance Min / Max** | Distance range of the effect. Keep both close for a sharp edge. If Min is larger than Max, the mask is inverted |
| **Density** | Strength of the effect |

## Camera Culling

Removes instances outside the camera view, to lighten heavy scenes.

1. In the BagaPie panel, select the scatter layer.
2. Select the camera (or an empty), then the scattered surface **last**.
3. Press **J** and choose **Camera Culling**.

| Setting | Effect |
| --- | --- |
| **Camera** | The camera used |
| **X Ratio / Y Ratio** | Widen the kept area. Increase them if instances disappear at the frame edges |
| **Offset** | Extra margin |

Once a camera culling exists, the **Camera Culling** button in the layer tools, and the camera icon in the modifier stack, assign it to other layers.

Culling resolution depends on the surface resolution. Subdivide the surface if needed.
