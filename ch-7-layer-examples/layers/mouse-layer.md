# Mouse Layer

For a Mouse layer, I activate it using a dual function layer on hold. I use karabiner-elements to control the mouse using speed modifiers for the mouse speed and scrolling speed. For moving quickly, speed modifiers are useful. For precision, slow modifiers are useful. Additionally, you can set save points to teleport your mouse cursor to specific areas on the screen, such as the center. Teleporting the mouse cursor around is very convenient if you have multiple monitors.&#x20;

Getting used to a mouse layer does take some work. Doing practice drills at [aim trainer](https://aimtrainer.io/) can help. You can select custom challenge, click on the custom button to add custom settings like .5 targets per second with 0 increase speed. As you get better you can gradual increase this amount. I can do around 1.3 targets consistently for 100 hit.

{% embed url="https://www.youtube.com/watch?ab_channel=MetaTypers&v=HxGz8UXMUIc" %}
practice drills using aim trainer
{% endembed %}

![Mouse layer](<../../.gitbook/assets/Screen Shot 2022-05-29 at 5.10.29 PM.png>)

| Description                                 | Hotkey |
| ------------------------------------------- | ------ |
| left click                                  | f      |
| right lick                                  | g      |
| left click + cmd                            | v      |
| slow modifier .3                            | a      |
| slow modifier .5                            | 1      |
| speed modifier 2.0                          | s      |
| speed modifier 1.5                          | d      |
| scroll up                                   | u      |
| scroll down                                 | o      |
| left cursor movement                        | j      |
| right cursor movement                       | l      |
| up cursor movement                          | i      |
| down cursor movement                        | k      |
| move cursor to left side screen(ultrawide)  | m      |
| move cursor to center(ultrawide)            | 2      |
| move cursor to right side screen(ultrawide) | 3      |
| move cursor to center(laptop)(bottom)       | h      |
| move cursor to center 3rd monitor(top)      | n      |



```
            "name": "Default profile",
            "parameters": {
                "delay_milliseconds_before_open_device": 1000
            },
            "selected": true,
            "simple_modifications": [
                {
                    "from": {
                        "key_code": "1",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "mouse_key": {
                                "speed_multiplier": 0.5
                            }
                        }
                    ]
                },
                {
                    "from": {
                        "key_code": "2",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "software_function": {
                                "set_mouse_cursor_position": {
                                    "screen": 0,
                                    "x": "50%",
                                    "y": "50%"
                                }
                            }
                        }
                    ]
                },
                {
                    "from": {
                        "key_code": "3",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "software_function": {
                                "set_mouse_cursor_position": {
                                    "screen": 0,
                                    "x": "85%",
                                    "y": "50%"
                                }
                            }
                        }
                    ]
                },
                {
                    "from": {
                        "key_code": "a",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "mouse_key": {
                                "speed_multiplier": 0.3
                            }
                        }
                    ]
                },
                {
                    "from": {
                        "key_code": "d",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "mouse_key": {
                                "speed_multiplier": 1.5
                            }
                        }
                    ]
                },
                {
                    "from": {
                        "key_code": "f",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "pointing_button": "button1"
                        }
                    ]
                },
                {
                    "from": {
                        "key_code": "g",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "modifiers": [
                                "left_command"
                            ],
                            "pointing_button": "button1"
                        }
                    ]
                },
                {
                    "from": {
                        "key_code": "h",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "software_function": {
                                "set_mouse_cursor_position": {
                                    "screen": 2,
                                    "x": "50%",
                                    "y": "50%"
                                }
                            }
                        }
                    ]
                },
                {
                    "from": {
                        "key_code": "i",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "mouse_key": {
                                "y": -1536
                            }
                        }
                    ]
                },
                {
                    "from": {
                        "key_code": "j",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "mouse_key": {
                                "x": -1536
                            }
                        }
                    ]
                },
                {
                    "from": {
                        "key_code": "k",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "mouse_key": {
                                "y": 1536
                            }
                        }
                    ]
                },
                {
                    "from": {
                        "key_code": "l",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "mouse_key": {
                                "x": 1536
                            }
                        }
                    ]
                },
                {
                    "from": {
                        "key_code": "m",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "software_function": {
                                "set_mouse_cursor_position": {
                                    "screen": 0,
                                    "x": "23%",
                                    "y": "50%"
                                }
                            }
                        }
                    ]
                },
                {
                    "from": {
                        "key_code": "n",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "software_function": {
                                "set_mouse_cursor_position": {
                                    "screen": 1,
                                    "x": "50%",
                                    "y": "50%"
                                }
                            }
                        }
                    ]
                },
                {
                    "from": {
                        "key_code": "o",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "mouse_key": {
                                "vertical_wheel": 32
                            }
                        }
                    ]
                },
                {
                    "from": {
                        "key_code": "s",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "mouse_key": {
                                "speed_multiplier": 2.0
                            }
                        }
                    ]
                },
                {
                    "from": {
                        "key_code": "u",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "mouse_key": {
                                "vertical_wheel": -32
                            }
                        }
                    ]
                },
                {
                    "from": {
                        "key_code": "v",
                        "modifiers": {
                            "mandatory": [
                                "control",
                                "shift",
                                "right_option"
                            ]
                        }
                    },
                    "to": [
                        {
                            "pointing_button": "button2"
                        }
                    ]
                }
            ],
```
