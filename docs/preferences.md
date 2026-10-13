# Preferences

PanelPilot exposes its full configuration directly inside the addon preferences. There are no extra menus or pies - every shortcut lives in one list.

Open it via **Edit > Preferences > Add-ons > PanelPilot**.

## The default state

When you install PanelPilot for the first time, the list is populated with five factory-default shortcuts bound to the most common 3D Viewport tabs.

```{image} ./_static/images/panelpilot_preferences_default.png
:alt: PanelPilot preferences in the default state, listing the five factory shortcuts bound to Tool, View, Edit, Animation, and Mesh
:width: 100%
```

## Shortcut list

Each row represents one keyboard shortcut bound to one sidebar tab.

| Column   | Meaning                                                                    |
| -------- | -------------------------------------------------------------------------- |
| Shortcut | The key combination assigned to this row. Click to rebind via capture.     |
| Tab      | The name of the sidebar tab to activate. Type it, or pick from the dropdown.|
| Dropdown | Opens the list of available tabs, grouped by editor.                       |
| Reset    | Restore this row to its default. Glows red when the row was modified.      |
| X        | Remove this row.                                                           |

## Picking a tab from the dropdown

Click the dropdown arrow next to the tab field. PanelPilot lists every tab available in the current session, grouped under a header for each editor (3D Viewport, Image Editor, Node Editor, Sequencer, Clip Editor, and so on). The factory-default tabs are always present under 3D Viewport even if the current mode does not register them.

Choosing an entry writes the plain tab name into the field. You can still edit the field by hand afterwards.

```{image} ./_static/images/panelpilot_dropdown_grouped.png
:alt: The tab dropdown open, listing tabs grouped under 3D Viewport, Image Editor, and Node Editor headers
:width: 100%
```

## Customized list and modified rows

Once you start renaming tabs, rebinding keys, or adding new shortcuts, the list grows and some rows light up in red on their reset icon. The red glow tells you which rows differ from their stored default.

```{image} ./_static/images/panelpilot_preferences_customized.png
:alt: PanelPilot preferences after customization, showing a row with a red reset icon, user-added shortcuts, and an empty row waiting for a binding
:width: 100%
```

## Rebinding a shortcut

1. Click the **Shortcut** button on a row.
2. The button label changes to **Press key...** and a hint appears in the area header.
3. Press the desired key combination (any key, optionally with Ctrl, Shift, or Alt).
4. The new combination is written into the row and applied immediately.

To cancel a capture, press **ESC** or click any mouse button. The row keeps its previous value.

## Adding and removing rows

- **Add Shortcut**: appends a new row. The first nine adds auto-assign the next free `Alt + NUMPAD_n`; beyond that, a blank row is created and you choose the key via capture.
- **X** on a row: removes that row from the list.
- **Reset All to Defaults**: clears the list and rebuilds the factory set.

## Auto-apply

Every change to the list (key, modifiers, tab name, additions, removals) triggers a full rebuild of the addon keymap. There is no Apply button.
