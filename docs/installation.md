# Installation

## Requirements

- Blender 4.2 or newer (the extension format requires it).
- No external Python packages.

```{image} ./_static/images/blender_logo.png
:alt: Blender
:width: 220px
:align: center
```

## Install the extension

1. Open Blender.
2. Go to **Edit > Preferences > Get Extensions**.
3. Click the dropdown next to the search bar and choose **Install from Disk**.
4. Select `PanelPilot_1.0.0.zip`.
5. PanelPilot appears in the extensions list and is enabled by default.

## Confirm it is active

When PanelPilot is enabled, the default shortcuts are bound to the 3D Viewport keymap immediately. Move the cursor over the 3D Viewport and press **Alt + Numpad 1**. The sidebar opens (if it was hidden) and switches to the **Tool** tab.

If you want to verify or change the bindings, open **Edit > Preferences > Add-ons**, search for `PanelPilot`, and expand the panel. See [Preferences](preferences.md) for the full UI walkthrough.

## Update the addon

To replace an older version:

1. Open **Edit > Preferences > Get Extensions**.
2. Find PanelPilot, click the gear icon, choose **Uninstall**.
3. Install the new `PanelPilot_x.y.z.zip` following the steps above.

User preferences (custom shortcuts) are kept across reinstalls because they live in Blender's user preferences file.
