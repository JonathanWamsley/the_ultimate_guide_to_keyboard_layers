# Discord Layer

{% embed url="https://support.discord.com/hc/en-us/articles/225878307--macOS-Discord-Hotkeys" %}

Discord can be navigated easily between different groups or channels using shortcuts. This make browsing for updates much faster

| Description              | Original Hotkey    | Updated Hotkey |
| ------------------------ | ------------------ | -------------- |
| group move up            | cmd + opt + up     | u              |
| group move down          | cmd + opt + down   | j              |
| channel move up          | opt + up           | i              |
| channel move down        | opt + down         | k              |
| unread channel move up   | opt + shift + up   | o              |
| unread channel move down | opt + shift + down | l              |
| emote picker             | cmd + e            | ;              |

```
                    {
                        "manipulators": [
                            {
                                "conditions": [
                                    {
                                        "bundle_identifiers": [
                                            "^com\\.hnc\\.Discord"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "Discord group up",
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
                                        "key_code": "up_arrow",
                                        "modifiers": [
                                            "command",
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
                                            "^com\\.hnc\\.Discord"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "Discord group down",
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
                                        "key_code": "down_arrow",
                                        "modifiers": [
                                            "command",
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
                                            "^com\\.hnc\\.Discord"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "Discord channel up",
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
                                        "key_code": "up_arrow",
                                        "modifiers": [
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
                                            "^com\\.hnc\\.Discord"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "Discord channel down",
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
                                        "key_code": "down_arrow",
                                        "modifiers": [
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
                                            "^com\\.hnc\\.Discord"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "Discord unread channel up",
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
                                        "key_code": "up_arrow",
                                        "modifiers": [
                                            "shift",
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
                                            "^com\\.hnc\\.Discord"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "Discord unread channel down",
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
                                        "key_code": "down_arrow",
                                        "modifiers": [
                                            "shift",
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
                                            "^com\\.hnc\\.Discord"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "Discord emote picker",
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
                                        "key_code": "e",
                                        "modifiers": [
                                            "command"
                                        ]
                                    }
                                ],
                                "type": "basic"
                            }
                        ]
                    },
```
