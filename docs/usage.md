# Usage

PanelPilot has a single job: when a bound shortcut fires, switch the N-panel sidebar of the editor under the cursor to the target tab, and open the sidebar if it is currently hidden.

```{image} ./_static/images/panelpilot_preferences_default.png
:alt: PanelPilot preferences with the five factory-default shortcuts bound to Tool, View, Edit, Animation, and Mesh
:width: 100%
```

## Trigger a shortcut

1. Move the mouse over an editor that has a tabbed sidebar (3D Viewport, Image Editor, Node Editor, Sequencer, or Clip Editor).
2. Press one of the bound key combinations.
3. The sidebar opens if it was hidden, and the matching tab becomes active in that editor.

The operator does not steal focus, does not change selection, and does not change the active mode. It only changes the sidebar state of the area under the cursor.

## Which editors are supported

Shortcuts are registered in the keymaps of these editors:

- 3D Viewport
- Image Editor (and UV Editor)
- Node Editor (Shader, Geometry Nodes, Compositor)
- Video Sequencer
- Movie Clip Editor

The same shortcut can point to a tab that exists in several editors. If the target tab does not exist in the editor under the cursor, the operator reports a warning in the status bar and does nothing else.

## Choosing a tab

Each shortcut row has two ways to set the target tab:

- **Dropdown** - click the arrow button next to the tab field to open a list of all tabs available in the current session, grouped by editor. Pick one and its name is written into the field.
- **Text field** - type the tab name directly. Useful for tabs that belong to an addon that is currently disabled and therefore not in the dropdown.

The tab name is case-sensitive: `View` is not the same as `view`.

## Adding a new shortcut

1. Open **Edit > Preferences > Add-ons > PanelPilot**.
2. Click **Add Shortcut**.
3. A new row is added with the next free `Alt + NUMPAD_n` combination.
4. Click the key button and press the desired key combination.
5. Pick the target tab from the dropdown, or type its name.

The change is saved and the keymap is rebuilt automatically.

## Removing a shortcut

Click the **X** button on the right of any row. The change is immediate.

## Resetting a row

Click the circular refresh icon on the right of any row to restore it to its default values. The icon turns red when the row has been modified, so you always know which rows you have customized.

To restore the entire default set, click **Reset All to Defaults** under the list.
