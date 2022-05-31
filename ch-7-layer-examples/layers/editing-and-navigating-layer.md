# Editing & Navigating Layer

This is one of the most important layer that I use. I constantly switch back in forth from the default layer to the editing & navigating layer using 1-5 commands. An editing and navigating layer is responsible for selecting, deleting, moving and copying/pasting text.

My first iterations actually had 2 edit/nav layers. One for single movement/selection using arrow keys. then another hyper edit/nav layer  that was activated with shift that would then make the single arrow/select movement become move by 1 word instead.&#x20;

Later, I revised the edit/nav layer into one layer by using modifiers on the left hand side and actions on the right. The learning curve is a little higher, but the speed gains is and comfort is well worth it in the long run. This method also allows for custom modifiers to be created as well.&#x20;

![Editing & Navigating layer](<../../.gitbook/assets/Screen Shot 2022-05-29 at 1.59.03 PM.png>)

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
