# PanelPilot

PanelPilot is a small, focused Blender extension that lets you jump between the tabs of the 3D Viewport sidebar (N-panel) with custom keyboard shortcuts.

It is built for users who spend a lot of time moving between Item, Tool, View, Edit, and addon-specific tabs and want a faster, mouse-free way to switch between them.

## What PanelPilot does

- Binds keyboard shortcuts to specific N-panel tabs in the 3D Viewport.
- Opens the sidebar automatically if it is hidden when a shortcut fires.
- Lets you rebind every shortcut directly from the addon preferences using a click-and-press capture.
- Resets any row to its factory default with a single click.
- Saves and applies every change instantly.

## Default shortcuts

| Shortcut         | Tab        |
| ---------------- | ---------- |
| Alt + NUMPAD_1   | Tool       |
| Alt + NUMPAD_2   | View       |
| Alt + NUMPAD_3   | Edit       |
| Alt + NUMPAD_4   | Animation  |
| Alt + NUMPAD_5   | Mesh       |

Alt + Numpad 1–9 was chosen because it has zero conflicts with Blender's default keymap across 3D View, Object Mode, Mesh, Curve, Armature, Sculpt and Pose.

## Documentation

```{toctree}
:maxdepth: 2
:caption: Contents

installation
usage
preferences
faq
changelog
```
