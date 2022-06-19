# VS Code Layer

VS code is a code editor where I spend a good portion of my work hours. Being able to navigate between different files and the terminal improves my workflow greatly. Since there are so many VS code hotkeys, I actually have 2 vs code layers, the VS code editor layer and the VS code terminal layer.

### Editor Layer

The VS code editor layer takes place in the editor where content is edited. The editor layer belongs to an application layer, where all keys are hyper keys and karabiner-elements transforms the keys.

On the right-hand side, there are shortcuts to open, close and move between different editor groups and tabs. A group is when there are multiple windows open, like split vertically side by side. A tab is when there are multiple tabs open.

On the left-hand side, there are shortcuts to search and replace, add cursors and go to problems within the editor. Multi-cursor is when multiple cursors can be created at specific locations either by position or by specific text. Problems any problems an editor sees that may be a logic, syntax or an extension related tool like incorrect spelling.

![](<../../.gitbook/assets/Screen Shot 2022-06-19 at 3.37.53 AM.png>)

| Description                          | Key                   |
| ------------------------------------ | --------------------- |
| toggle to terminal                   | F4                    |
| toggle to editor                     | F4                    |
| quick open                           | F1                    |
| show commands                        | F2                    |
| focus left editor tab group          | u                     |
| focus right editor tab group         | o                     |
| move to left editor tab              | j                     |
| move to right editor tab             | l                     |
| move editor to left group            | h                     |
| move editor to right group           | ;                     |
| move editor left in group            | y                     |
| move editor right in group           | p                     |
| split editor                         | i                     |
| close editor                         | w                     |
| go to most recent editor group       | k                     |
| close active editor group            | q (registered as f12) |
| navigate to previous location        | m                     |
| navigate back in navigation location | n                     |

### Terminal Layer

The terminal layer takes place in the terminal where commands are ran. The terminal layer belongs to an application 2 layer since there are not enough hotkey spaces on the first application layer and also takes place in karabiner-elements.

Right now, only the right hand side is used. Shortcuts to open, close and move between different groups and tabs similar to the right hand side of the VS code editor layer. Multiple terminal instances can be created side by side or&#x20;

![](<../../.gitbook/assets/Screen Shot 2022-06-19 at 1.41.49 AM.png>)

| Description                      | Key |
| -------------------------------- | --- |
| show side bar visibility         | m   |
| show terminal                    | n   |
| terminal split                   | i   |
| new terminal                     | k   |
| terminal focus previous          | j   |
| terminal focus next              | l   |
| terminal go to previous instance | u   |
| terminal go to next instance     | o   |
| terminal kill                    | y   |
| resize terminal increase size    | p   |
| resize terminal decrease size    | /   |
| terminate(ctrl + c)              | h   |



All VS code shortcuts

```
// Place your key bindings in this file to override the defaults
[
    // Toggle between terminal and editor focus
{ "key": "ctrl+shift+alt+cmd+f4", "command": "workbench.action.terminal.focus"},
{
    "key": "ctrl+shift+alt+cmd+f4",
    "command": "workbench.action.focusActiveEditorGroup",
    "when": "terminalFocus"
},
{
    "key": "alt+cmd+u",
    "command": "workbench.action.terminal.focusPreviousPane",
    "when": "terminalFocus && terminalProcessSupported"
},
{
    "key": "alt+left",
    "command": "-workbench.action.terminal.focusPreviousPane",
    "when": "terminalFocus && terminalProcessSupported"
},
{
    "key": "ctrl+shift+tab",
    "command": "-workbench.action.quickOpenLeastRecentlyUsedEditorInGroup"
},
{
    "key": "ctrl+shift+alt+cmd+l",
    "command": "workbench.action.nextEditor"
},
{
    "key": "ctrl+pagedown",
    "command": "-workbench.action.nextEditor"
},
{
    "key": "ctrl+shift+alt+cmd+j",
    "command": "workbench.action.previousEditor"
},
{
    "key": "ctrl+pageup",
    "command": "-workbench.action.previousEditor"
},
{
    "key": "alt+cmd+right",
    "command": "-workbench.action.nextEditor"
},
{
    "key": "alt+cmd+left",
    "command": "-workbench.action.previousEditor"
},
{
    "key": "alt+cmd+o",
    "command": "workbench.action.terminal.focusNextPane",
    "when": "terminalFocus && terminalProcessSupported"
},
{
    "key": "alt+cmd+down",
    "command": "-workbench.action.terminal.focusNextPane",
    "when": "terminalFocus && terminalProcessSupported"
},
{
    "key": "alt+cmd+up",
    "command": "-workbench.action.terminal.focusPreviousPane",
    "when": "terminalFocus && terminalProcessSupported"
},
{
    "key": "alt+cmd+l",
    "command": "workbench.action.terminal.focusNext",
    "when": "terminalFocus && terminalProcessSupported"
},
{
    "key": "cmd+6",
    "command": "-workbench.action.terminal.focusNext",
    "when": "terminalFocus && terminalProcessSupported"
},
{
    "key": "alt+cmd+j",
    "command": "workbench.action.terminal.focusPrevious",
    "when": "terminalFocus && terminalProcessSupported"
},
{
    "key": "cmd+5",
    "command": "-workbench.action.terminal.focusPrevious",
    "when": "terminalFocus && terminalProcessSupported"
},
{
    "key": "alt+cmd+/",
    "command": "workbench.action.terminal.resizePaneDown",
    "when": "terminalFocus && terminalProcessSupported"
},
{
    "key": "ctrl+cmd+down",
    "command": "-workbench.action.terminal.resizePaneDown",
    "when": "terminalFocus && terminalProcessSupported"
},
{
    "key": "alt+cmd+p",
    "command": "workbench.action.terminal.resizePaneUp",
    "when": "terminalFocus && terminalProcessSupported"
},
{
    "key": "ctrl+cmd+up",
    "command": "-workbench.action.terminal.resizePaneUp",
    "when": "terminalFocus && terminalProcessSupported"
},
{
    "key": "alt+cmd+i",
    "command": "workbench.action.terminal.split",
    "when": "terminalFocus && terminalProcessSupported"
},
{
    "key": "cmd+\\",
    "command": "-workbench.action.terminal.split",
    "when": "terminalFocus && terminalProcessSupported"
},
{
    "key": "alt+cmd+m",
    "command": "workbench.action.toggleSidebarVisibility"
},
{
    "key": "cmd+b",
    "command": "-workbench.action.toggleSidebarVisibility"
},
{
    "key": "alt+cmd+y",
    "command": "workbench.action.terminal.kill"
},
{
    "key": "alt+cmd+[KeyK]",
    "command": "workbench.action.terminal.newInActiveWorkspace"
},
{
    "key": "alt+z",
    "command": "workbench.action.quickOpenNavigateNextInFilePicker",
    "when": "inFilesPicker && inQuickOpen"
},
{
    "key": "cmd+p",
    "command": "-workbench.action.quickOpenNavigateNextInFilePicker",
    "when": "inFilesPicker && inQuickOpen"
},
{
    "key": "ctrl+shift+alt+cmd+f5",
    "command": "workbench.action.quickOpen"
},
{
    "key": "cmd+p",
    "command": "-workbench.action.quickOpen"
},
{
    "key": "shift+cmd+w",
    "command": "workbench.action.closeWindow"
},
{
    "key": "shift+cmd+w",
    "command": "-workbench.action.closeWindow"
},
{
    "key": "ctrl+shift+alt+cmd+c",
    "command": "actions.find",
    "when": "editorFocus || editorIsOpen"
},
{
    "key": "cmd+f",
    "command": "-actions.find",
    "when": "editorFocus || editorIsOpen"
},
{
    "key": "ctrl+shift+alt+cmd+v",
    "command": "editor.action.nextMatchFindAction",
    "when": "editorFocus"
},
{
    "key": "cmd+g",
    "command": "-editor.action.nextMatchFindAction",
    "when": "editorFocus"
},
{
    "key": "ctrl+shift+alt+cmd+x",
    "command": "editor.action.previousMatchFindAction",
    "when": "editorFocus"
},
{
    "key": "shift+cmd+g",
    "command": "-editor.action.previousMatchFindAction",
    "when": "editorFocus"
},
{
    "key": "ctrl+shift+alt+cmd+d",
    "command": "editor.action.startFindReplaceAction",
    "when": "editorFocus || editorIsOpen"
},
{
    "key": "alt+cmd+f",
    "command": "-editor.action.startFindReplaceAction",
    "when": "editorFocus || editorIsOpen"
},
{
    "key": "ctrl+shift+alt+cmd+a",
    "command": "editor.action.replaceAll",
    "when": "editorFocus && findWidgetVisible"
},
{
    "key": "alt+cmd+enter",
    "command": "-editor.action.replaceAll",
    "when": "editorFocus && findWidgetVisible"
},
{
    "key": "ctrl+shift+alt+cmd+t",
    "command": "editor.action.insertCursorAbove",
    "when": "editorTextFocus"
},
{
    "key": "alt+cmd+up",
    "command": "-editor.action.insertCursorAbove",
    "when": "editorTextFocus"
},
{
    "key": "ctrl+shift+alt+cmd+b",
    "command": "editor.action.insertCursorBelow",
    "when": "editorTextFocus"
},
{
    "key": "alt+cmd+down",
    "command": "-editor.action.insertCursorBelow",
    "when": "editorTextFocus"
},
{
    "key": "ctrl+shift+alt+cmd+g",
    "command": "cursorUndo",
    "when": "textInputFocus"
},
{
    "key": "cmd+u",
    "command": "-cursorUndo",
    "when": "textInputFocus"
},
{
    "key": "ctrl+shift+alt+cmd+e",
    "command": "editor.action.selectHighlights",
    "when": "editorFocus"
},
{
    "key": "shift+cmd+l",
    "command": "-editor.action.selectHighlights",
    "when": "editorFocus"
},
{
    "key": "ctrl+shift+alt+cmd+r",
    "command": "editor.action.addSelectionToNextFindMatch",
    "when": "editorFocus"
},
{
    "key": "cmd+d",
    "command": "-editor.action.addSelectionToNextFindMatch",
    "when": "editorFocus"
},
{
    "key": "ctrl+shift+alt+cmd+w",
    "command": "editor.action.moveSelectionToPreviousFindMatch"
},
{
    "key": "ctrl+shift+alt+cmd+f",
    "command": "editor.action.moveSelectionToNextFindMatch",
    "when": "editorFocus"
},
{
    "key": "cmd+k cmd+d",
    "command": "-editor.action.moveSelectionToNextFindMatch",
    "when": "editorFocus"
},
{
    "key": "ctrl+shift+alt+cmd+i",
    "command": "workbench.action.splitEditor"
},
{
    "key": "cmd+\\",
    "command": "-workbench.action.splitEditor"
},
{
    "key": "shift+cmd+]",
    "command": "-workbench.action.nextEditor"
},
{
    "key": "ctrl+shift+alt+cmd+o",
    "command": "workbench.action.focusNextGroup"
},
{
    "key": "ctrl+shift+alt+cmd+u",
    "command": "workbench.action.focusPreviousGroup"
},
{
    "key": "ctrl+shift+alt+cmd+;",
    "command": "workbench.action.moveEditorToRightGroup"
},
{
    "key": "ctrl+shift+alt+cmd+h",
    "command": "workbench.action.moveEditorToLeftGroup"
},
{
    "key": "ctrl+shift+alt+cmd+y",
    "command": "workbench.action.moveEditorLeftInGroup"
},
{
    "key": "cmd+k shift+cmd+left",
    "command": "-workbench.action.moveEditorLeftInGroup"
},
{
    "key": "ctrl+shift+alt+cmd+p",
    "command": "workbench.action.moveEditorRightInGroup"
},
{
    "key": "cmd+k shift+cmd+right",
    "command": "-workbench.action.moveEditorRightInGroup"
},
{
    "key": "ctrl+shift+alt+cmd+f9",
    "command": "editor.action.revealDefinition",
    "when": "editorHasDefinitionProvider && editorTextFocus && !isInEmbeddedEditor"
},
{
    "key": "f12",
    "command": "-editor.action.revealDefinition",
    "when": "editorHasDefinitionProvider && editorTextFocus && !isInEmbeddedEditor"
},
{
    "key": "ctrl+shift+alt+cmd+f10",
    "command": "editor.action.peekDefinition",
    "when": "editorHasDefinitionProvider && editorTextFocus && !inReferenceSearchEditor && !isInEmbeddedEditor"
},
{
    "key": "alt+f12",
    "command": "-editor.action.peekDefinition",
    "when": "editorHasDefinitionProvider && editorTextFocus && !inReferenceSearchEditor && !isInEmbeddedEditor"
},
{
    "key": "ctrl+shift+alt+cmd+f11",
    "command": "editor.action.commentLine"
},
{
    "key": "ctrl+shift+alt+cmd+a",
    "command": "editor.action.marker.prev",
    "when": "editorFocus"
},
{
    "key": "shift+alt+f8",
    "command": "-editor.action.marker.prev",
    "when": "editorFocus"
},
{
    "key": "ctrl+shift+alt+cmd+s",
    "command": "editor.action.marker.next",
    "when": "editorFocus"
},
{
    "key": "alt+f8",
    "command": "-editor.action.marker.next",
    "when": "editorFocus"
},
{
    "key": "alt+cmd+n",
    "command": "workbench.action.togglePanel"
},
{
    "key": "cmd+j",
    "command": "-workbench.action.togglePanel"
},
{
    "key": "ctrl+shift+alt+cmd+z",
    "command": "cSpell.addWordToUserDictionary"
},
{
    "key": "ctrl+shift+alt+cmd+k",
    "command": "workbench.action.quickOpenPreviousRecentlyUsedEditorInGroup"
},
{
    "key": "ctrl+tab",
    "command": "-workbench.action.quickOpenPreviousRecentlyUsedEditorInGroup"
},
{
    "key": "alt+cmd+,",
    "command": "workbench.action.terminal.openWebLink"
},
{
    "key": "ctrl+shift+alt+cmd+f8",
    "command": "workbench.action.showCommands"
},
{
    "key": "shift+cmd+p",
    "command": "-workbench.action.showCommands"
},
{
    "key": "ctrl+shift+alt+cmd+m",
    "command": "workbench.action.navigatePreviousInNavigationLocations"
},
{
    "key": "ctrl+shift+alt+cmd+n",
    "command": "workbench.action.navigateBackInNavigationLocations"
},
]
```
