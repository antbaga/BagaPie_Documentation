# Deformation

## Displace

<div class="video"><iframe src="https://www.youtube-nocookie.com/embed/EKUg_FvDrgk?start=575" title="BagaPie 11 - Parametric Tools" loading="lazy" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; fullscreen" allowfullscreen></iframe></div>
<p class="video-caption">Video: <em>BagaPie 11 - Parametric Tools</em>, from 9:35.</p>

Sets up a displacement in one click: a Subdivision modifier, a Displace modifier and a texture.

Select one mesh, press **J** and choose **Displace**.

| Setting | Effect |
| --- | --- |
| **Subdivision / Subdivision Render / Type** | Subdivision levels in the viewport and in renders |
| **Direction**, **Strength**, **Midlevel** | Displace modifier settings |
| **Texture** | Texture type. Detailed settings are in the Properties editor's Texture tab |
| **Mapping / Object** | Texture coordinates; use an object to move the pattern |
| **Scale**, **Brightness**, **Ramp Min / Max** | Pattern size and contrast |

## Instances Displace

Applies a noise displacement to instances only, for example the instances of a scatter or an array.

Select one object that carries instances (mesh or curve), press **J** and choose **Instances Displace**.

Settings: **Noise Texture**, **Scale**, **Noise**, **Intensity XYZ**, **Noise Position XYZ**.

## Deform

Blends and twists an object along an axis.

Select one mesh, press **J** and choose **Deform**. Settings: **Blend** and **Twist** per axis (X, Y, Z), with **Flip**.
