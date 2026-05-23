# FAQ

## Why Alt + Numpad and not Alt + 1, 2, 3?

The number row keys with the Alt modifier conflict with Blender's default keymap in some modes — for example, **Alt + 1** in Sculpt Mode is bound to `object.subdivision_set`. Alt + Numpad 1–9, on the other hand, is free across 3D View, Object Mode, Mesh, Curve, Armature, Sculpt and Pose. Using the numpad is the safest default.

## Can I rebind the shortcuts to non-numpad keys?

Yes. Click the key button on any row and press whatever combination you want (with optional Ctrl, Shift, or Alt). PanelPilot does not stop you from binding combinations that conflict with Blender or other addons, so test the new combo after binding it.

## Can I reorder the tabs in the sidebar?

No. Blender does not expose a public Python API to reorder N-panel tab categories. The visible order is decided by Blender's internal C code and cannot be controlled from an extension. PanelPilot does the next best thing: it lets you jump straight to any tab with a single keystroke regardless of where it sits in the strip.

## The shortcut fires but the tab does not change. Why?

The most common cause is a typo in the **Tab** field. The name must match exactly the visible tab title and is case-sensitive: `View` works, `view` and `VIEW` do not. Check the spelling in the preferences and try again. The operator also reports a warning in the status bar when the tab name is not registered.

## Does PanelPilot work in the Image Editor or Node Editor?

Not in this version. PanelPilot registers shortcuts only in the 3D Viewport keymap. Support for other editors is on the roadmap.

## Does it conflict with my other addons?

PanelPilot only registers `view3d.switch_sidebar_tab` keymap items under the 3D View keymap, using whatever key combinations you set. If two addons bind the same combination, Blender fires only one of them and which one is undefined. Pick combinations that are free in your setup if you want predictable behavior.

## Are my custom shortcuts saved across Blender sessions?

Yes. PanelPilot stores them in Blender's user preferences. They survive Blender restarts and addon reinstalls.

## Where is the source code?

PanelPilot is a small four-file Python package. Once installed, the source lives in your Blender extensions folder, typically:

`~/AppData/Roaming/Blender Foundation/Blender/<version>/extensions/user_default/panel_pilot/`
