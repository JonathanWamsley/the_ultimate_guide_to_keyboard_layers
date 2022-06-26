# Default Layer

The default layer is the root of all the layers. The majority of your layers should be accessible from the default layer+1 layer. The best layer keys are the thumb keys because you can won't have to move your hands and can still easily tap alphanumeric keys. I have also used other keys, like caps lock for a modifier layer or even "3" for a number layer.

In the default layer, I encourage removing the number keys and replacing them for commonly used symbols made of [tap-dance/super](../../ch-3-layer-activators/3.6-tap-dance-super-keys.md) keys. The keys have 3 outputs depending on if the key is single tapped, double tapped, or tapped and held. By using super keys, all the symbol keys can be used in the default layer without having to use the shift key. I used to use a [symbols layer](symbols-layer.md), but found superkeys easier and faster to use.

Not all keys are equally easy to press and each user will have their own preferences. When does a shift layer become faster and more ergonomical than typing a further to reach key is a gray zone that varies from user to user. Some users won't want to use the number keys at all, some will use 3, 4, 5, 8, 9, 0 and some use all numbers.

The layer below is not my own, but what I imagine what I would like if I used a qwerty layout. I also included another variant with super keys on the shift layer too. There may be some keys such as the qwerty bracket keys that can be no key and the super keys`<` and `>` can be placed on the shift layer.

![Default qwerty layer](<../../.gitbook/assets/Screen Shot 2022-06-18 at 1.10.40 AM.png>)

| Description                      | layer number                                                                                                        |
| -------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| Shift Layer                      | [L#2](shift-layer.md)                                                                                               |
| Numpad Layer                     | [L#3](numpad-layer.md)                                                                                              |
| Edit/Nav Layer                   | [L#4](editing-and-navigating-layer.md)                                                                              |
| Mouse Layer                      | [L#5](mouse-layer.md)                                                                                               |
| Application Layer                | L#6([vs code](vs-code-layer.md), [browser](browser-layer.md), [slack](slack-layer.md), [discord](discord-layer.md)) |
| Appliaction 2 Layer              | L#6 -> L#7([vs code terminal](vs-code-layer.md))                                                                    |
| Screen Manipulation /Media Layer | L#5 -> L#8([spectale](screen-management-layer.md), [media](media-layer.md))                                         |
| Gaming Layer                     | Lock [L#10](gaming-layer.md)                                                                                        |
| Context Control/Macros Layer     | [Meh+](context-control-macro-layer.md)                                                                              |



```
{
    "from": {
        "key_code": "f24"
    },
    "to": [
        {
            "key_code": "delete_or_backspace",
            "modifiers": [
                "left_option"
            ]
        }
    ]
},
```

There is a limitation with the software that I currently use, where a dual key can not be a macro. To get around this, I set a dual key to output layer 6 / F24 and then in karabiner-elements remap the F24 to option+backspace which deletes a word. I find that action very useful as correcting a word is often slower than just deleting the word and retyping it.
