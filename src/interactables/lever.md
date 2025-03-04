# Lever Class
__Extends__: [Area2D](https://docs.godotengine.org/en/stable/classes/class_area2d.html#class-area2d)

A togglable [Colored](../colors.md) Lever
- Can be toggled by the player, through the interaction button, and enemies, through collision
- Cannot be toggled by same colored objects (white being an exception)
- DOWN means ON, UP means OFF


## Properties
| Type |  Name | Default |
| ---- | ----- | ------- |
|[bool](https://docs.godotengine.org/en/stable/classes/class_bool.html#class-bool)|[sniffer_only](#bool-sniffer_only--false)|false|
|[bool](https://docs.godotengine.org/en/stable/classes/class_bool.html#class-bool)|[negative](#bool-negative--false)|false|
|[bool](https://docs.godotengine.org/en/stable/classes/class_bool.html#class-bool)|cops_only_pull|false|
|[bool](https://docs.godotengine.org/en/stable/classes/class_bool.html#class-bool)|starts_down|false|
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html#class-int)  | [color](../colors.md) | 0 |


## Signals

### lever_state_change(new_state : [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html#class-bool))
Emitted when the lever is toggled. True for the ON position and False for OFF position. This can be inverted by [negative](#bool-negative--false).


## Property Description

### [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html#class-bool) sniffer_only = false
Defines if the button will ignore anything that isn't the player. Mainly, this would be used to ignore cops.

### [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html#class-bool) cops_only_pull = false
Enemies (cops) will always try to pull the lever down. This could be used with starts_down = true to create the need to kill/move a cop, or with starts_down = false to create a cop directioning puzzle.

### [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html#class-bool) starts_down = false
This makes the lever start in the ON position.

### [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html#class-bool) negative = false
Inverts the output of the signal, making it false when pressed.