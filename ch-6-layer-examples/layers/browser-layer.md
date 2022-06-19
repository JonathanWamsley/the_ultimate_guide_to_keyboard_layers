# Browser Layer

The browser layer is an application layer that uses browser shortcuts such as creating, removing and navigating through tabs and windows. For a browser, I use chrome but most other browsers have similar shortcuts.

{% embed url="https://support.google.com/chrome/answer/157179?co=GENIE.Platform=Desktop&hl=en" %}

### Vimium Extension

{% embed url="https://cheatography.com/l1qu1d/cheat-sheets/vimium/" %}

Vimium is a browser extension that allows links to be clicked on easily without a mouse. This is done by vimuim highlighting 2 letters showing available links and then the user types the 2 letters next to the link to open in a tab or new tab.

There are also some other nice features such as being able to searching through tabs or easily going to last tab.

One think I dislike about vimuim is that it is alway active and sometimes has weird interactions with text input fields. For this reason, I like to place vimium on a layer and add to other chrome shortcuts. I do this by creating a custom key map in the Vimium extension in the vimium help section, activated by "?" by default. I unmap all shortcuts then add the ones I use. the \<c-letter> stands for control + letter which I do to avoid conflicts such as youtube's hotkeys that have no modifiers and cannot be easily changed.\


![](<../../.gitbook/assets/Screen Shot 2022-05-28 at 12.13.46 PM.png>)

I then use karabiner elements to map an application layer(hyper keys), to a browser layer that only triggers when chrome is the front most application. So hyper keys remapped into the vimuim keybindings like control + a letter. At the end I show the karabiner code since its quite lengthy.

![](<../../.gitbook/assets/Screen Shot 2022-06-19 at 3.39.29 AM.png>)

The full table showing the key mapping is below with an image of the application layer below.

| Description                    | Original Hotkey          | Updated Hotkey |
| ------------------------------ | ------------------------ | -------------- |
| Open a new window              | ⌘ + n                    | e              |
| Open a new tab, and jump to it | ⌘ + t                    | d              |
| Reopen tab in new window       | macro                    | t              |
| Move right a tab               | ⌘ + Option + Right Arrow | f              |
| Move left a tab                | ⌘ + Option + Left Arrow  | s              |
| reopen last closed tab         | ⌘ + Shift + t            | t              |
| close the current tab          | ⌘ + w                    | a              |
| close the current window       | ⌘ + Shift + w            | q              |
| refresh window                 | ⌘ + r                    | b              |
| jump to address bar            | ⌘ + l                    | r              |
| find                           | ⌘ + f                    | x              |
| find next                      | ⌘ + g                    | c              |
| find previous                  | ⌘ + Shift + g            | v              |
| scroll up                      | karabiner                | u              |
| scroll down                    | karabiner                | o              |
| scroll left                    | vimium                   | j              |
| scroll right                   | vimium                   | l              |
| page up                        | vimium                   | y              |
| page down                      | vimium                   | n              |
| top of page                    | vimium                   | i              |
| bot of page                    | vimium                   | k              |
| go to first tab                | vimium                   | h              |
| go to last tab                 | vimium                   | ;              |
| go to last visited tab         | vimium                   | F5             |
| search through tabs            | vimium                   | g              |
| open link in current tab       | vimium                   | m              |
| open link in new tab           | vimium                   | f9             |
| copy current link to clipboard | vimium                   | f10            |
| vimium help menu               | vimium                   | p              |



```
{
    "manipulators": [
        {
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome New Window",
            "from": {
                "key_code": "e",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "n",
                    "modifiers": [
                        "left_command"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome New Tab",
            "from": {
                "key_code": "d",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "t",
                    "modifiers": [
                        "left_command"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome Move Left Tab",
            "from": {
                "key_code": "s",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "left_arrow",
                    "modifiers": [
                        "left_command",
                        "option"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome Move Right Tab",
            "from": {
                "key_code": "f",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "right_arrow",
                    "modifiers": [
                        "left_command",
                        "option"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome Bring Back Closed Tab",
            "from": {
                "key_code": "w",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "t",
                    "modifiers": [
                        "left_command",
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome Select URL",
            "from": {
                "key_code": "r",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "l",
                    "modifiers": [
                        "left_command"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.microsoft\\.VSCode"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "VS Code View Open Previous Editor",
            "from": {
                "key_code": "j",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "j",
                    "modifiers": [
                        "command",
                        "option",
                        "shift",
                        "control"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome Close All",
            "from": {
                "key_code": "f12",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "w",
                    "modifiers": [
                        "left_command",
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome Close Current Tab",
            "from": {
                "key_code": "a",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "w",
                    "modifiers": [
                        "left_command"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome Reload Page",
            "from": {
                "key_code": "b",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "r",
                    "modifiers": [
                        "left_command",
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome Search Prev",
            "from": {
                "key_code": "x",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "g",
                    "modifiers": [
                        "left_command",
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome Search",
            "from": {
                "key_code": "c",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "g",
                    "modifiers": [
                        "left_command"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome Search Next",
            "from": {
                "key_code": "v",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "g",
                    "modifiers": [
                        "left_command"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome Back",
            "from": {
                "key_code": "z",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "left_arrow",
                    "modifiers": [
                        "left_command"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome Vimium scroll down",
            "from": {
                "key_code": "o",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "mouse_key": {
                        "vertical_wheel": 32
                    }
                }
            ],
            "type": "basic"
        }
    ]
},
{
    "manipulators": [
        {
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome Vimium scroll up",
            "from": {
                "key_code": "u",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "mouse_key": {
                        "vertical_wheel": -32
                    }
                }
            ],
            "type": "basic"
        }
    ]
},
{
    "manipulators": [
        {
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome Vimium search through tabs",
            "from": {
                "key_code": "g",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "g",
                    "modifiers": [
                        "control"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome vimium scroll left",
            "from": {
                "key_code": "j",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "j",
                    "modifiers": [
                        "control"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome vimium scroll right",
            "from": {
                "key_code": "l",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "l",
                    "modifiers": [
                        "control"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome vimium go to first tab",
            "from": {
                "key_code": "h",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "h",
                    "modifiers": [
                        "control"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome vimium go to last tab",
            "from": {
                "key_code": "semicolon",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "semicolon",
                    "modifiers": [
                        "control"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome vimium open link in current tab",
            "from": {
                "key_code": "m",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "m",
                    "modifiers": [
                        "control"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome vimium scroll page up,",
            "from": {
                "key_code": "y",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "y",
                    "modifiers": [
                        "control"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome vimium scroll page down",
            "from": {
                "key_code": "n",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "n",
                    "modifiers": [
                        "control"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome vimium show help",
            "from": {
                "key_code": "p",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "p",
                    "modifiers": [
                        "control"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome vimium go to last visit tab",
            "from": {
                "key_code": "f5",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "3",
                    "modifiers": [
                        "control"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome vimium copy current url to clipboard",
            "from": {
                "key_code": "f10",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "2",
                    "modifiers": [
                        "control"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome vimium open link in new tab",
            "from": {
                "key_code": "f9",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "1",
                    "modifiers": [
                        "control"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome vimium scroll to top",
            "from": {
                "key_code": "i",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "i",
                    "modifiers": [
                        "control"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome vimium scroll to bot",
            "from": {
                "key_code": "k",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "k",
                    "modifiers": [
                        "control"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome vimium help menu",
            "from": {
                "key_code": "p",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "p",
                    "modifiers": [
                        "control"
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
            "conditions": [
                {
                    "bundle_identifiers": [
                        "^com\\.google\\.Chrome"
                    ],
                    "type": "frontmost_application_if"
                }
            ],
            "description": "Chrome Open Tab In New Window. Macro see KM",
            "from": {
                "key_code": "t",
                "modifiers": {
                    "mandatory": [
                        "shift",
                        "command",
                        "option",
                        "control"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "l",
                    "modifiers": [
                        "left_command"
                    ]
                },
                {
                    "key_code": "return_or_enter",
                    "modifiers": [
                        "shift"
                    ]
                }
            ],
            "type": "basic"
        }
    ]
},
```
