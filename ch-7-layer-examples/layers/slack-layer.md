# Slack Layer

{% embed url="https://slack.com/help/articles/201374536-Slack-keyboard-shortcuts" %}

A slack layer helps you navigate to different slack channels, view latest unread messages and arrange text by with edits, code blocks or emojis.

|                                    |                          |   |
| ---------------------------------- | ------------------------ | - |
| compose new message                | cmd + n                  | i |
| browse DMs                         | cmd + shift + k          | u |
| open all unread messages           | cmd + shift + a          | o |
| jump to conversation               | cmd + k                  | k |
| go back to last group              | cmd + \[                 | j |
| go forward to last group           | cmd + ]                  | l |
| start a search                     | cmd + g                  | c |
| search in the current conversation | cmd + f                  | v |
| edit a message                     | cmd + e                  | e |
| add emoji                          | cmd + r                  | r |
| hyperlink selected text            | cmd + shift + u          | d |
| code selected text                 | cmd + shift + c          | s |
| code block selected text           | cmd + shift + option + c | c |

```
                    {
                        "manipulators": [
                            {
                                "conditions": [
                                    {
                                        "bundle_identifiers": [
                                            "^com\\.tinyspeck\\.slackmacgap"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "slack compose a new message",
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
                                        "key_code": "n",
                                        "modifiers": [
                                            "command"
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
                                            "^com\\.tinyspeck\\.slackmacgap"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "slack browse DMs",
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
                                        "key_code": "k",
                                        "modifiers": [
                                            "command",
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
                                            "^com\\.tinyspeck\\.slackmacgap"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "slack open all unread messages",
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
                                        "key_code": "a",
                                        "modifiers": [
                                            "command",
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
                                            "^com\\.tinyspeck\\.slackmacgap"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "slack jump to a conversation",
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
                                            "command"
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
                                            "^com\\.tinyspeck\\.slackmacgap"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "slack go back to last group",
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
                                        "key_code": "open_bracket",
                                        "modifiers": [
                                            "command"
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
                                            "^com\\.tinyspeck\\.slackmacgap"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "slack go forward in history",
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
                                        "key_code": "close_bracket",
                                        "modifiers": [
                                            "command"
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
                                            "^com\\.tinyspeck\\.slackmacgap"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "slack start a search",
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
                                            "command"
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
                                            "^com\\.tinyspeck\\.slackmacgap"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "slack search in the current conversation",
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
                                        "key_code": "f",
                                        "modifiers": [
                                            "command"
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
                                            "^com\\.tinyspeck\\.slackmacgap"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "slack edit a message you sent",
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
                                        "key_code": "e"
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
                                            "^com\\.tinyspeck\\.slackmacgap"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "slack add an emoji reaction to a message",
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
                                        "key_code": "r"
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
                                            "^com\\.tinyspeck\\.slackmacgap"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "slack hyperlink selected text",
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
                                        "key_code": "u",
                                        "modifiers": [
                                            "command",
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
                                            "^com\\.tinyspeck\\.slackmacgap"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "slack code selected text",
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
                                        "key_code": "c",
                                        "modifiers": [
                                            "command",
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
                                            "^com\\.tinyspeck\\.slackmacgap"
                                        ],
                                        "type": "frontmost_application_if"
                                    }
                                ],
                                "description": "slack codeblock selected text",
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
                                        "key_code": "c",
                                        "modifiers": [
                                            "command",
                                            "shift",
                                            "option"
                                        ]
                                    }
                                ],
                                "type": "basic"
                            }
                        ]
                    }
                ]
            },
```
