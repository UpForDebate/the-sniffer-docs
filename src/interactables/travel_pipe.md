# TravelPipe Class
__Extends__: [Area2D](https://docs.godotengine.org/en/stable/classes/class_area2d.html#class-area2d)

A [Colored](../colors.md) pipe for in-level travelling.
target_pipe must be set for this to work.

While travelling through a pipe, you keep your entry velocity(rotated) as exit velocity.
You may also script the exit velocity.

When placing, a ghost_sniffer will appear and get shot at the scripted velocity to aid with scripting launches.

## Properties
| Type |  Name | Default |
| ---- | ----- | ------- |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html#class-int)  | [color](#int-color) | 0 |
| [TravelPipe](#travelpipe-class) | [target_pipe](#travelpipe-target_pipe) ||
| [float](https://docs.godotengine.org/en/stable/classes/class_float.html#class-float) | [minimum_entry_velocity](#float-minimum_entry_velocity--0) | 0 |
| [float](https://docs.godotengine.org/en/stable/classes/class_float.html#class-float) | [exit_velocity](#float-exit_velocity--0) | 0 |
| [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html#class-bool) | [horizontal_lock](#bool-horizontal_lock--false) | false |

## Property Descriptions
### [TravelPipe](#travelpipe-class) target_pipe
The pipe the sniffer will get launched from.

### [float](https://docs.godotengine.org/en/stable/classes/class_float.html#class-float) minimum_entry_velocity = 0
The minimum entry velocity to trigger the scripted exit velocity. If it is 0, the scripted exit velocity will always be triggered.

This may be used to force a jump from a high place or a yellow super jump to get to the pipe.

### [float](https://docs.godotengine.org/en/stable/classes/class_float.html#class-float) exit_velocity = 0
The scripted exit velocity. When triggered, the sniffer will be launched at this speed.

This may be used to force getting to a platform and no further.

### [bool](https://docs.godotengine.org/en/stable/classes/class_bool.html#class-bool) horizontal_lock = false
A movement lock for the player until he either touches the floor or touches the wall and is able to walljump.