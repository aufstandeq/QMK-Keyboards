# Understanding Key Codes

There the basic keys and then custom keys that we can program in to our new keyboard. Here I wanted to review the key codes and how I could use them in the tools, not how to program my own [keymap file](https://docs.qmk.fm/#/keymap). I may get to that in the future.

All the main keys are listed on the [QMK site](https://docs.qmk.fm/#/keycodes_basic).


### Useful for Development

| Key | Description |
| --- | --- |
| RESET | Put the keyboard into DFU mode for flashing |

The reset key will allow you to keep flashing the keyboard for testing your firmware update. Depending on your keyboard you would need to push the reset button on the bottom or hold *spacebar* and *B* while unplugging and plugging in the USB cable.

### Multi Key for Smaller Keyboards
Leveraging Quantum codes we can quickly customize part of our keyboard and we can toggle development. Modifier keys also provide flexibility by allowing the key to be programmed with a secondary function.

#### Multi-purpose ESC
| Key | Description |
| --- | --- |
| KC_GENSC | Escape key when tapped and ` when pressed with shift |

#### Multi-purpose shift
| Key | Description |
| --- | --- |
| KC_LSPO | Left Shift when held and ( when tapped |
| KC_RSPC | Right shift when held and ) when tapped |
| LSFT(kc) | Hold left shift and press *kc* |
| RSFT(kc) | Hold right shift and press *kc* |

#### Multi-purpose Control
| Key | Description |
| --- | --- |
| LCTL(kc) | Hold left control and press *kc* |
| RCTL(kc) | Hold right control and press *kc*  |

#### Multi-purpose Alt
| Key | Description |
| --- | --- |
| LATL(kc) | Hold left ALT and press *kc* |
| RATL(kc) | Hold right ALT and press *kc*  |

Now we can go a step further and create macro like keys.
#### Multi-Purpose Mult Key Functionality
| Key | Description |
| --- | --- |
| HYPR(kc) | Hold LEFT CONTROL, SHIFT, ALT, & GUI and press *kc* |
| MEH(kc) | Hold LEFT CONTROL, SHIFT, ALT and press *kc* |

## Some Ideas
- Map left control asa multi with RESET
- Left shift and MO key for layer 1


## References
- https://docs.qmk.fm/#/keycodes
