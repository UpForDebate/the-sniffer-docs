# Button Class
__Extends__: [Area2D](https://docs.godotengine.org/en/stable/classes/class_area2d.html#class-area2d)
A pressable [Colored](../colors.md) button
- Can be pressed by players, boxes and enemies
- Cannot be pressed by same colored objects (white being an exception)


## Properties
| Type |  Name | Default |
| ---- | ----- | ------- |
|[bool](https://docs.godotengine.org/en/stable/classes/class_bool.html#class-bool)|[sniffer_and_box_only](#bool-sniffer_and_box_only--false)|false|
|[bool](https://docs.godotengine.org/en/stable/classes/class_bool.html#class-bool)|[negative](#bool-negative--false)|false|
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html#class-int)  | [color](../colors.md) | 0 |


## Signals
### button_state_change(new_state : [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html#class-bool))
Emitted when the button is pressed or unpressed. True for pressed and False for unpressed. This can be inverted by [negative](#bool-negative--false).

## Property Description

### [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html#class-bool) sniffer_and_box_only = false
Defines if the button will ignore anything that isn't a box or the player. Mainly, this would be used to ignore cops.

### [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html#class-bool) negative = false
Inverts the output of the signal, making it false when pressed.