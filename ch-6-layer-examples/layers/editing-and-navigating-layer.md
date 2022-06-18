# Editing & Navigating Layer

The Editing & Navigation layer is one of the most important layer that I use. I was using a much different version of this layer even before I had an ergonomic keyboard. The layer is broken up into a few different sections.

Starting with right-hand-side, the arrow keys are put in a comfortable j, i, k, l position in cyan. In red are ways to delete text with the Macro delete line on `p`. The ctrl+A and ctrl+e means go to the start line or end line even if the line is wrapped which is very useful in an editor or terminal. The thumb Hyper keys in white are actually VS code related because I am often in this layer when I context switch to a different terminal, file, or command.

On the left-hand-side, the light blue macros are select all, line and word. The orange macros are new line above and below. On the bottom light purple is the usual undo, cut, copy, paste. There is also a paste 2nd oldest history macro on the "b" key which comes in handy all the time.&#x20;

The section above in purple are modifiers. They are used in combination of keys on the right hand side. With the left thumb on a layer key and different modifiers held down an action on the right can be done such as an arrow key, delete key or page move key. A full chart of all the combinations are in the table below. I structured the modifier order as ctrl, option, command shift because it seemed the most comfortable because shift is the most situational key and can easily be lifted up and down.&#x20;

Another cool feature is that additional commands can be made using modifier combinations. For example, if I want to move left by 3 words or up by 3 lines, I can create a macro using karabiner-elements by mapping an unused combination, like cmd+option+letter to the macro.

This layer has gone through many iterations and actually used to be 2 layers. I was using this layer before I had an ergonomic keyboard because it was that useful and is what really got me into creating layers and macros. Typically, I do 4-5 actions in this layer and then go back to the default layer. I prefer having a press and hold functionality that is based on positional keys instead of modes with mnemonic like in vim.



![Editing & Navigating Layer](<../../.gitbook/assets/Screen Shot 2022-06-18 at 1.25.51 AM.png>)

| Description                      | Original Hotkey                              | Updated Hotkey     |
| -------------------------------- | -------------------------------------------- | ------------------ |
| left arrow                       | left\_arrow                                  | j                  |
| right arrow                      | right\_arrow                                 | l                  |
| up arrow                         | up\_arrow                                    | i                  |
| down arrow                       | down\_arrow                                  | k                  |
| page up                          | page\_up                                     | y                  |
| page down                        | page\_down                                   | n                  |
| back space                       | back\_space                                  | u                  |
| delete                           | del                                          | o                  |
| escape                           | esc                                          | q                  |
| undo                             | cmd+z                                        | z                  |
| cut                              | cmd+x                                        | x                  |
| copy                             | cmd+c                                        | c                  |
| paste                            | cmd+v                                        | v                  |
|                                  |                                              |                    |
| start of line                    | cmd+left\_arrow                              | cmd+j              |
| end of line                      | cmd+right\_arrow                             | cmd+j              |
| top of line                      | cmd+up\_arrow                                | cmd+i              |
| bottom of line                   | cmd+down\_arrow                              | cmd+k              |
| move left one word               | option+left\_arrow                           | option+j           |
| move right one word              | option+right\_arrow                          | option+l           |
|                                  |                                              |                    |
| backspace left one word          | option+backspace                             | option+u           |
| delete right one word            | option+del                                   | option+o           |
| backspace to start of line       | cmd+backspace                                | cmd+u              |
| delete to end of line            | karabiner-elements(ctrl+k)                   | cmd+o              |
|                                  |                                              |                    |
| select letter left               | shift+left\_arrow                            | shift+j            |
| select letter right              | shift+right\_arrow                           | shift+l            |
| select line above to cursor      | shift+up\_arrow                              | shift+i            |
| select line below to cursor      | shift+down\_arrow                            | shift+k            |
| select left one word             | option+shift+left\_arrow                     | option+shift+j     |
| select right one word            | option+shift+right\_arrow                    | option+shift+l     |
| select to start of line          | cmd+shift+left\_arrow                        | cmd+shift+j        |
| select to end of line            | cmd+shift+right\_arrow                       | cmd+shift+l,       |
| select to page up                | shift+page\_up                               | shift+y            |
| select to page down              | shift+page\_down                             | shift+n            |
|                                  |                                              |                    |
| move line up                     | vs code(option+up\_arrow)                    | option+i           |
| move line down                   | vs code(option+right\_arrow)                 | option+j           |
| copy line up                     | <p>vs code</p><p>(option+shift+up_arrow)</p> | option+shift+i     |
| copy line down                   | vs code (option+shift+down\_arrow)           | option+shift+k     |
|                                  |                                              |                    |
| left arrow x3                    | karabiner-elements                           | cmd+option+j       |
| right arrow x3                   | karabiner-elements                           | cmd+option+l       |
| up arrow x3                      | karabiner-elements                           | cmd+option+i       |
| down arrow x3                    | karabiner-elements                           | cmd+option+k       |
| left selection x3                | karabiner-elements                           | cmd+option+shift+j |
| right selection x3               | karabiner-elements                           | cmd+option+shift+l |
|                                  |                                              |                    |
| go to start of line w/ word wrap | ctrl+a                                       | m                  |
| go to end of line w/word wrap    | ctrl+e                                       | .                  |
| select word                      | macro                                        | r                  |
| select line                      | macro                                        | e                  |
| select all                       | cmd+a                                        | w                  |
| delete line                      | macro                                        | p                  |
| new line above cursor            | macro                                        | t                  |
| new line below cursor            | macro                                        | g                  |
| paste 2nd last item              | macro                                        | b                  |
| go to file                       | vs code(cmd+p)                               | F1                 |
| show all commands                | vs code(cmd+shift+p)                         | F4                 |
| terminal focus/unfocus           | vs code(custom)                              | F2                 |

### ## Karabiner-element macros

```
{
    "global": {
        "check_for_updates_on_startup": true,
        "show_in_menu_bar": true,
        "show_profile_name_in_menu_bar": false
    },
    "profiles": [
        {
            "complex_modifications": {
                "parameters": {
                    "basic.simultaneous_threshold_milliseconds": 50,
                    "basic.to_delayed_action_delay_milliseconds": 500,
                    "basic.to_if_alone_timeout_milliseconds": 1000,
                    "basic.to_if_held_down_threshold_milliseconds": 500,
                    "mouse_motion_to_scroll.speed": 100
                },
                "rules": [
                    {
                        "manipulators": [
                            {
                                "description": "Global Navigation left left left",
                                "from": {
                                    "key_code": "left_arrow",
                                    "modifiers": {
                                        "mandatory": [
                                            "command",
                                            "option"
                                        ]
                                    }
                                },
                                "to": [
                                    {
                                        "key_code": "left_arrow",
                                        "modifiers": [
                                            "left_option"
                                        ]
                                    },
                                    {
                                        "key_code": "left_arrow",
                                        "modifiers": [
                                            "left_option"
                                        ]
                                    },
                                    {
                                        "key_code": "left_arrow",
                                        "modifiers": [
                                            "left_option"
                                        ]
                                    }
                                ],
                                "type": "basic"
                            }
                        ]
                    },
                    {
                        "manipulators": [
                            {
                                "description": "Global Navigation right right right",
                                "from": {
                                    "key_code": "right_arrow",
                                    "modifiers": {
                                        "mandatory": [
                                            "command",
                                            "option"
                                        ]
                                    }
                                },
                                "to": [
                                    {
                                        "key_code": "right_arrow",
                                        "modifiers": [
                                            "left_option"
                                        ]
                                    },
                                    {
                                        "key_code": "right_arrow",
                                        "modifiers": [
                                            "left_option"
                                        ]
                                    },
                                    {
                                        "key_code": "right_arrow",
                                        "modifiers": [
                                            "left_option"
                                        ]
                                    }
                                ],
                                "type": "basic"
                            }
                        ]
                    },
                    {
                        "manipulators": [
                            {
                                "description": "Global Selection right right right",
                                "from": {
                                    "key_code": "right_arrow",
                                    "modifiers": {
                                        "mandatory": [
                                            "command",
                                            "option",
                                            "shift"
                                        ]
                                    }
                                },
                                "to": [
                                    {
                                        "key_code": "right_arrow",
                                        "modifiers": [
                                            "left_option",
                                            "shift"
                                        ]
                                    },
                                    {
                                        "key_code": "right_arrow",
                                        "modifiers": [
                                            "left_option",
                                            "shift"
                                        ]
                                    },
                                    {
                                        "key_code": "right_arrow",
                                        "modifiers": [
                                            "left_option",
                                            "shift"
                                        ]
                                    }
                                ],
                                "type": "basic"
                            }
                        ]
                    },
                    {
                        "manipulators": [
                            {
                                "description": "Global Selection left left left",
                                "from": {
                                    "key_code": "left_arrow",
                                    "modifiers": {
                                        "mandatory": [
                                            "command",
                                            "option",
                                            "shift"
                                        ]
                                    }
                                },
                                "to": [
                                    {
                                        "key_code": "left_arrow",
                                        "modifiers": [
                                            "left_option",
                                            "shift"
                                        ]
                                    },
                                    {
                                        "key_code": "left_arrow",
                                        "modifiers": [
                                            "left_option",
                                            "shift"
                                        ]
                                    },
                                    {
                                        "key_code": "left_arrow",
                                        "modifiers": [
                                            "left_option",
                                            "shift"
                                        ]
                                    }
                                ],
                                "type": "basic"
                            }
                        ]
                    },
                    {
                        "manipulators": [
                            {
                                "description": "Global Navigation up up up",
                                "from": {
                                    "key_code": "up_arrow",
                                    "modifiers": {
                                        "mandatory": [
                                            "command",
                                            "option"
                                        ]
                                    }
                                },
                                "to": [
                                    {
                                        "key_code": "up_arrow"
                                    },
                                    {
                                        "key_code": "up_arrow"
                                    },
                                    {
                                        "key_code": "up_arrow"
                                    }
                                ],
                                "type": "basic"
                            }
                        ]
                    },
                    {
                        "manipulators": [
                            {
                                "description": "Global Navigation down down down",
                                "from": {
                                    "key_code": "down_arrow",
                                    "modifiers": {
                                        "mandatory": [
                                            "command",
                                            "option"
                                        ]
                                    }
                                },
                                "to": [
                                    {
                                        "key_code": "down_arrow"
                                    },
                                    {
                                        "key_code": "down_arrow"
                                    },
                                    {
                                        "key_code": "down_arrow"
                                    }
                                ],
                                "type": "basic"
                            }
                        ]
                    },
                    {
                        "manipulators": [
                            {
                                "description": "Global Forward Delete to end of line",
                                "from": {
                                    "key_code": "delete_forward",
                                    "modifiers": {
                                        "mandatory": [
                                            "command"
                                        ]
                                    }
                                },
                                "to": [
                                    {
                                        "key_code": "k",
                                        "modifiers": [
                                            "left_control"
                                        ]
                                    }
                                ],
                                "type": "basic"
                            }
                        ]
                    }
        }
   ]
}
                    
```

### Macros

A macro is a series of key strokes. Most keyboard software has a dedicated section for creating macros. Here are the macros I used in the editing / navigating layer.

select word

* option left\__arrow, shift+option+right\__arrow

select line

* cmd left\__arrow, shift+cmd+right\__arrow

delete line

* 1, ctrl+a, shift+cmd+right\_arrow, backspace, backspace
  * I add a 1 as an arbitrary value so that if the line is blank then the expected output is still produced and not deleting the last character on the above line.

new line above

* ctrl+a, enter

new line below

* ctrl+e, enter

### VS Code

To shift between the terminal and editor quickly, I use this script. hyper f4 can be changed to another variable, but I used it to avoid conflicts and to indicate its a thumb key on my keyboard. This can be added to your configuration by going to code -> preferences -> keyboard shortcuts -> select the open keyboard shortcuts (JSON) icon of a folder. Then paste the below code in.

```
{ "key": "ctrl+shift+alt+cmd+f4", "command": "workbench.action.terminal.focus"},
{
    "key": "ctrl+shift+alt+cmd+f4",
    "command": "workbench.action.focusActiveEditorGroup",
    "when": "terminalFocus"
},
```
