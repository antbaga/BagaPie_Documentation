# Setup & installation

BagaPie uses two kinds of asset libraries. Both are set up from **Preferences > Assets**.

## BagaPie Parametric Library (free, CC0)

Click **Setup BagaPie's Parametric Library CC-0**. BagaPie adds a library named **BagaPie Modifier** to the Asset Browser, filled with BagaPie presets.

This library also contains the Geometry Nodes tools of the [Edit Mode pie](../edit-mode/index.md). After the first setup, **restart Blender**: the tools are only available after a restart.

If the Edit Mode pie shows **Tool File missing !** after an update, click **Update BagaPie Parametric Library**, then restart Blender.

## BagaPie Assets packs

[BagaPie Assets](bagapie-assets.md) is the optional asset library that funds BagaPie: up to 750 assets and 40 scatter presets. Every BagaPie tool also works with your own assets.

### Install the packs

Packs are `.baga` files.

1. In **Preferences > Assets**, click **Set BagaPie Assets Packs Storage Location** and choose a folder.
2. Click **Install BagaPie Asset Pack (.baga files)** and select a pack.
3. Repeat for each pack. Packs are installed one by one, and each installation can take several seconds.

The preferences list the packs (Lite, Essential and full volumes) and show the installed ones in green. **Edit Library Location** changes the storage folder; the folder icon opens it.

After updating BagaPie, if no packs are found, use **Set library location** to point BagaPie to the folder where your packs are already installed.

### Material panels

Some BagaPie Assets materials (grass, plants, rocks, trees, stumps) have their own settings in the BagaPie panel when the asset is selected: tint, brightness, saturation and their random variations, ambient occlusion, translucency, specular, roughness, and a **Season** slider for vegetation.

Season values above 0.9 add transparency, which can increase render time. Lower **Season** or **Random Season** if renders slow down.
