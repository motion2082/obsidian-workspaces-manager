# Workspaces Manager

Workspaces Manager is a plugin that expands the functionality of [workspaces](https://help.obsidian.md/Plugins/Workspaces) in [Obsidian](https://obsidian.md/).

> **Note:** This is an independent fork of [Workspaces Plus](https://github.com/nothingislost/obsidian-workspaces-plus) by [NothingIsLost](https://github.com/nothingislost) and [Johnny ✨](https://github.com/jsmorabito), maintained independently by [motion2082](https://github.com/motion2082).

## Features

### Workspace Indicator

- Current active workspace shown in status bar
- Click on workspace name in status bar to open workspace switcher
- `shift-click` status bar icon or workspace name to save the workspace

### Workspace Switcher

- Switch, delete, rename, and create new workspaces
- Save icon on the active workspace row for quick saving
- Open with assignable hotkey

### Hotkeys

- Open Workspaces Manager switcher modal
- Open specific workspace by name

### Plugin Options

- Toggle keyboard shortcuts on/off for the workspace switcher
- Toggle workspace delete confirmation on/off
- Auto save the active workspace on layout change

### Theming Options

- Workspaces Manager adds a data attribute to the HTML document body for workspace-specific styling
  - `body[data-workspace-name="My Workspace"]`
  - Updated whenever a new workspace is loaded

### Workspace Overrides

- Override pages loaded in a workspace using template variables

## How to use

After enabling the plugin, a workspace icon will appear in the status bar. If you are already using workspaces in Obsidian, the name of your current active workspace will be shown next to the icon.

> :warning: **Obsidian's core Workspaces plugin must be enabled for Workspaces Manager to work**

### Creating a Workspace

1. Type your new workspace name into the input field
2. Press `shift-enter` to create and save it

### Renaming a Workspace

Click the pencil icon next to any workspace name in the switcher.

### Deleting a Workspace

Click the trash icon next to a workspace, or press `shift-delete` while the workspace is selected.

### Opening a Workspace

1. Open the switcher via hotkey or by clicking the workspace icon/name in the status bar
2. Click a workspace or press `enter` after navigating with arrow keys

### Saving Workspaces

- Workspaces are not automatically saved when switching (unless the auto-save option is enabled)
- `shift-click` the workspace icon or name in the status bar
- In the switcher, click the save icon on the active workspace row, or use `shift-enter`
- Enable "Auto save on layout change" in settings to save automatically

### Overriding a Page in a Workspace

1. In settings, open the workspace you want to modify
2. Enter the file path in the override field, using template variables if needed
   - Example: `Journal/{{date:YYYY}}/{{date:YYYY-MM}}/{{date:YYYY-MM-DD}}.md`
3. The page will be loaded with the override applied when switching to that workspace

## Installation

Copy `main.js`, `styles.css`, and `manifest.json` to your vault at:
```
VaultFolder/.obsidian/plugins/workspaces-manager/
```

## Feedback & Issues

Report issues and ideas on [GitHub](https://github.com/motion2082/obsidian-workspaces-manager/issues).

## Credits

- Originally developed by [NothingIsLost](https://github.com/nothingislost) and [Johnny ✨](https://github.com/jsmorabito) as [Workspaces Plus](https://github.com/nothingislost/obsidian-workspaces-plus)
- Workspace Picker and Modal based on [Obsidian Theme Picker](https://github.com/kenset/obsidian-theme-picker) by [Kenset](https://github.com/kenset)

## Changelog

### 1.0.0
- Forked as Workspaces Manager, running independently
- Added save icon to active workspace row in the switcher
- Upgraded TypeScript to 5.x, added ESLint

### 0.3.3 and earlier
See the [original plugin](https://github.com/nothingislost/obsidian-workspaces-plus) for prior history.

## Screenshot
<img width="424" height="761" alt="image" src="https://github.com/user-attachments/assets/b090523e-ab99-43bf-8061-c3177f84eb5c" />

