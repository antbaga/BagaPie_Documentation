# GeoPack: install and use packs

GeoPack lets you install, create and share custom tools for BagaPie. A pack is a set of Geometry Nodes modifiers, with their usage rules, icons, and optionally an asset library and scatter presets. Packs are shared as `.geopack` files.

<div class="video"><iframe src="https://www.youtube-nocookie.com/embed/Dk8okiAreTM" title="BagaPie 11 - GeoPack First Steps" loading="lazy" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; fullscreen" allowfullscreen></iframe></div>
<p class="video-caption">Video: <em>BagaPie 11 - GeoPack First Steps</em>.</p>

Think of a pack as a small add-on built with Geometry Nodes, without code. Packs you create are yours: you can export, share or sell them, and anyone with BagaPie can install them.

## Set the pack location

The first time, choose where packs are stored on your computer.

1. Open **Edit > Preferences > Add-ons > BagaPie** and expand **GeoPack**.
2. Click **Set packs location** and pick a folder.

Packs already in that folder are detected and listed. You can move packs to another folder later: open **Storage**, set the new path, and click **Move all packs to new location**.

## Install a pack

1. In **Preferences > GeoPack**, click **Install Pack**.
2. Select the `.geopack` file and confirm.

If the pack includes assets, BagaPie creates an asset library for it automatically.

A free **Demo Pack** (`Demo Pack.geopack`) comes with the BagaPie download on SuperHive and Gumroad. The [Stone Column Generator for BagaPie](https://superhivemarket.com/products/stone-column-generator-for-bagapie) is another example of a pack, and [BagaPie Assets](../assets-library/bagapie-assets.md) Full includes 40 scatter presets as GeoPack tools.

## Pack details

Expand a pack in the preferences to see:

- **Info:** description, authors, version, license, minimum Blender version, link.
- **Modifier:** the tools of the pack, each with an icon, information and **how this modifier will work**: what to select and what happens. Read it before using a tool.
- **Assets:** the pack's asset library and its files.

The eye icons hide a pack, or one of its modifiers, from the pie menu.

## Use a pack

In Object Mode, press **V**. The GeoPack pie menu lists the installed packs. Pick a pack, then a tool.

Grayed-out tools mean the selection does not match what the tool needs. If the pack author used [Node to Panel](node-to-panel.md), the tool settings appear in the BagaPie panel.

If no pack is installed, the pie menu tells you to set a location or install a pack.

## Next

- [Create a pack](create.md)
- [Scatter presets](scatter-presets.md)
- [Node to Panel](node-to-panel.md)
