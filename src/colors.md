# Colors
Colors are stored as an int, ranging from 0 to 4:
- White = 0
- Red = 1
- Green = 2
- Yellow = 3
- Blue = 4

Objects with a color should have a custom setter to handle the change. Changes to other objects should be done referred, as color is set before ready. They should also visually change color.

A paint_colors array is present in PlatformerGlobal to standardize the colors used by all objects.