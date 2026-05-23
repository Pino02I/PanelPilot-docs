# Changelog

## 1.0.0

First public release of PanelPilot.

### Features

- Switch the 3D Viewport sidebar to a specific N-panel tab via a custom keyboard shortcut.
- Auto-opens the sidebar if it is hidden when the shortcut fires.
- Default mapping: **Alt + Numpad 1-5** bound to Tool, View, Edit, Animation, and Mesh.
- Custom binding via a modal key-capture operator (click the key button, press the desired combination, ESC or mouse click to cancel).
- Per-row reset button that glows red when a row has been modified from its factory default.
- One-click **Reset All to Defaults** to restore the original mapping.
- Add new rows with auto-incrementing `Alt + NUMPAD_n` until the slots are exhausted.
- Auto-apply: every preference change rebuilds the addon keymap immediately, no Apply button.

### Packaging

- Distributed as a Blender Extension (`blender_manifest.toml`), compatible with Blender 4.2 and newer.
- Custom icon shown in the Get Extensions browser card.
- Ships with `README.md`, `CHANGELOG.md`, and full `LICENSE` (GPL v2.0+) at the package root.
