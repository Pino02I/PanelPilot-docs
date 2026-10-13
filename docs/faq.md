# FAQ

## Why Alt + Numpad and not Alt + 1, 2, 3?

The number row keys with the Alt modifier conflict with Blender's default keymap in some modes - for example, **Alt + 1** in Sculpt Mode is bound to `object.subdivision_set`. Alt + Numpad 1-9, on the other hand, is free across 3D View, Object Mode, Mesh, Curve, Armature, Sculpt and Pose. Using the numpad is the safest default.

## Can I rebind the shortcuts to non-numpad keys?

Yes. Click the key button on any row and press whatever combination you want (with optional Ctrl, Shift, or Alt). PanelPilot does not stop you from binding combinations that conflict with Blender or other addons, so test the new combo after binding it.

## Does PanelPilot work in the Image Editor or Node Editor?

Yes, since version 1.1.0. Shortcuts are registered in the 3D Viewport, Image Editor, Node Editor, Sequencer, and Clip Editor. The shortcut acts on whichever editor is under the cursor when you press it.

## Some tabs are missing from the dropdown. Why?

The dropdown lists the tabs that are registered in the current Blender session, grouped by editor. Tabs that belong to an addon that is disabled, or that only appear in a specific mode, may not be listed. The factory-default tabs (Tool, View, Edit, Animation, Mesh) are always shown, and any tab already used by one of your rows is shown too. For anything else, type the tab name directly into the field.

## Can I reorder the tabs in the sidebar?

No. Blender does not expose a public Python API to reorder N-panel tab categories. The visible order is decided by Blender's internal C code and cannot be controlled from an extension. PanelPilot does the next best thing: it lets you jump straight to any tab with a single keystroke regardless of where it sits in the strip.

## The shortcut fires but the tab does not change. Why?

The most common cause is a typo in the **Tab** field. The name must match exactly the visible tab title and is case-sensitive: `View` works, `view` and `VIEW` do not. It can also mean the tab does not exist in the editor under the cursor - for example a 3D-only tab while the mouse is over the Node Editor. The operator reports a warning in the status bar when the tab name is not found.

## Does it conflict with my other addons?

PanelPilot only registers `panelpilot.switch_sidebar_tab` keymap items in the supported editors, using whatever key combinations you set. If two addons bind the same combination, Blender fires only one of them and which one is undefined. Pick combinations that are free in your setup if you want predictable behavior.

## Are my custom shortcuts saved across Blender sessions?

Yes. PanelPilot stores them in Blender's user preferences. They survive Blender restarts and addon reinstalls.

## Where is the source code?

PanelPilot is a small four-file Python package. Once installed, the source lives in your Blender extensions folder, typically:

`~/AppData/Roaming/Blender Foundation/Blender/<version>/extensions/user_default/panel_pilot/`
