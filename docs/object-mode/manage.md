# Manage & Proxy

The Manage section of the **J** pie menu gathers scene management tools.

| Button | Action |
| --- | --- |
| **Create Group** | Group the selected objects. See [Group](../group.md) |
| **To Instance** | Group the selection and turn the group into an instance in one step |
| **Ungroup**, **Group to Instance** | Shown when a group is selected. See [Group](../group.md) |
| **Proxy** | Add or remove a viewport proxy |
| **Save as Asset** | Save the selected object as an asset (hidden by default) |
| **Save Material** | Save the active material of the selected object as an asset (hidden by default) |
| **Add Group Key** | Shown when the BagaPie group shortcut is not set: activates **Ctrl + G** |

## Proxy

A proxy replaces an object in the viewport with its **convex hull**. It is automatically disabled at render time. Use it to keep heavy scenes responsive.

- Select one or more objects, press **J** and choose **Proxy**.
- If the selection already has proxies, **Proxy** offers to remove them. You can select everything, proxies included, and remove all proxies at once, or put everything under proxy.

The proxy has no settings. In a scatter layer, you can toggle proxies per asset or for the whole layer from the [layer tools](scatter.md#tools).

## Save as Asset and Save Material

Both tools are hidden by default. Show them in **Preferences > Pie Menu Tools**. They save the selected object, or its active material, to an asset library. Preview generation may fail; you can replace the preview in the Asset Browser.
