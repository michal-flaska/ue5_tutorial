# Unreal Engine Tutorial
Just me, learning UE5 again

Tutorial: https://youtu.be/6UlU_FsicK8?si=XmViRdgQcCJIb4xO

## What I learned, that I didn't know before

### Landscape:
- You can hold shift while using tools (like sculpt) to inverse them.
  - For example, you don't sculpt a hill but a hole.

### Blueprints
- There are level blueprints
- If you select an object in the level, then go to level blueprint and right click on empty space in event graph, you can add reference to that object.
- Shortcuts:
  - Hold D and press LMB -> Creates Delay node
  - Hold ALT and press LMB on Exec arrow (the white little shit where you drag spaghetti - or how to call it) -> Deletes spaghetti that is connecting two blocks.
  - Hold CTRL and drag Variable into the event graph to automatically GET the vector.

- That dots are called 'pins'. Atleast hey call them 'pins'
- That 'little white shit' is called an execution pin.

- Get Actor Location is a function, but it does not have execution pin. Then it is called a 'pure function'

- Event Tick is a function
  - It is called every frame

- Blueprint is based on C++

- Difference between Print String & Print Text
  - Print String: For debugging. Shows messages in the editor (top-left screen) and output log. Uses colored plain text.
  - Print Text: Same purpose, but supports rich text formatting, localization, and better performance in packaged builds. Preferred for production or multi-language.
  - Use Print String when debugging. Use Print Text when formatting, translating, or shipping.

- Variable Types (I already know most of the basic ones, but its better to write them down):
  - Boolean: True / False
  - Byte: Unsigned 8-bit integer
  - Integer: Whole number
  - Integer64: Whole number but for 64bit architecture, meaning it can be larger
  - Float: A decimal number
  - String Types:
    - Name: Used in tags
    - String: It's a String, in most cases we will use this.
    - Text: Text is mostly used for UI & HUD
  - Vector: Vector is a struct with 3 values: `X, Y, Z`.
  - Rotator: Simmilar to Vector, but there is a limitation from values of `0` to `360`. Beyond that, rotator is going to be invalid.
  - Transform: Transform is a struct, which contains `Vector, Rotator, Vector` (Location, Rotation and Scale)
  - Other:
    - Types: Structure, Interface, Object Types, Enum (Enumeration)
    - Most common: Hit Result, Actor, 

### Misc
- You can hit 'end' on your keyboard to snap items to the ground (landscape) in the level.
- Anything that can be placed in a level is called an 'Actor'
- Light Movability:
  - Types can be changed in Transform section in the details panel
  - Types of Light Movability:
    - Static: Can't be changed in-game
    - Stationary: Can only change color and intensity in-game, but cant move
    - Movable: Can be moved and changed in-game