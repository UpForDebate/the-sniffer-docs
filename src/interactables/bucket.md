# Bucket Class
__Extends__: [Area2D](https://docs.godotengine.org/en/stable/classes/class_area2d.html#class-area2d)

The bucket is what changes [Sniffer's](../sniffer.md) [Color](../colors.md).

Buckets are interacted with on collision with the Sniffer, making him sniff it and change color. The bucket gets deactivated when doing so.

## Properties
| Type |  Name | Default |
| ---- | ----- | ------- |
| [int](https://docs.godotengine.org/en/stable/classes/class_int.html#class-int)  | [color](#int-color) | 0 |

## Property Descriptions
### [int](https://docs.godotengine.org/en/stable/classes/class_int.html#class-int) color = 0
Visual color of the bucket and color that gets passed to the character. Follows the [Color](../colors.md) standard for value.