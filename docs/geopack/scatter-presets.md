# Scatter presets

A complete scatter setup can be saved in a GeoPack and reused in one click, in any file. Applying a preset replaces the current scatter of the surface.

<div class="video"><iframe src="https://www.youtube-nocookie.com/embed/SbOvA8Yzdrw" title="BagaPie 11 - Scatter Presets" loading="lazy" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; fullscreen" allowfullscreen></iframe></div>
<p class="video-caption">Video: <em>BagaPie 11 - Scatter Presets</em>.</p>

## Save a preset

1. Set up the scatter on a surface. See [Scattering](../object-mode/scatter.md).
2. Make sure you have a pack to save it in. See [Create a pack](create.md).
3. Frame the surface in the 3D view: the preview is rendered from the current view.
4. At the bottom of the scatter settings, open **Save in GeoPack**:
    - **Generate Preview Icon** (on by default)
    - **Lighting: Use Current World** to light the preview with your world
5. Click **Save Scatter in GeoPack**, choose the pack, and **name the preset** (required). Keep **Preview Generation** checked. The other information is optional and can be edited later.
6. In **Usage**, keep **Active Object** set to **Mesh**, the default, and click **OK**.

Saving takes a few seconds: BagaPie renders the preview and copies the assets into the pack.

### What is saved

- All scatter layers of the surface.
- The assets, stored inside the pack.
- A preview, generated from the current view and the active object.

Camera culling, effectors and weight paint are **not** saved: they belong to the scene, not to the scatter system.

Preview settings (resolution, samples, exposure, sun, focal length) are in **Preferences > Preferences > GeoPack Scatter Icon Generator Settings**.

## Use a preset

Select a surface, press **V**, choose the pack, then the preset.

If the surface already has a scatter, BagaPie warns you that the new scatter will replace it, and that its camera culling and effectors will be lost.

## Share

The preset is a modifier of the pack: you can change its preview or information in **Preferences > GeoPack**. Export the pack as a `.geopack` file to share it.

The [BagaPie Assets](../assets-library/bagapie-assets.md) Full edition includes 40 ready-made scatter presets.
