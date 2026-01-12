## Took some notes from what I learned in the tutorial

### Viewport
- Shortcuts:
  - You can hit G to switch to Game View
  - QWERT for Tools (e.g. rotation, move, scale, etc.)

### Landscape:
- You can hold shift while using tools (like sculpt) to inverse them.
  - For example, you don't sculpt a hill but a hole.
- You can hit 'end' on your keyboard to snap items to the ground (landscape) in the level.

### Blueprints
- There are level blueprints
- If you select an object in the level, then go to level blueprint and right click on empty space in event graph, you can add reference to that object.
- Shortcuts:
  - Hold D and press LMB -> Creates Delay node
  - Hold ALT and press LMB on Exec arrow (the white little shit where you drag spaghetti - or how to call it) -> Deletes spaghetti that is connecting two blocks.
  - Hold CTRL and drag Variable into the event graph to automatically GET the vector.
  - Click on blueprint box, and hit CTRL + D, you can duplicate it.
  - Hold D and click LMB to add a delay in blueprint.
  - Hold B and click LMB to add `if` (branch) statement.

- That dots are called 'pins'. Atleast hey call them 'pins'
- That 'little white shit' is called an execution pin.
- If you double click on node, it will create a separate pin. It is called 'reroute node'
- You can add 'Sequence' to split 1 execution pins into more.

- Get Actor Location is a function, but it does not have execution pin. Then it is called a 'pure function'

- Event Tick is a function
  - It is called every frame

- Blueprint is based on C++

- Using spaces in names of functions, variables, etc. is not a good practice and can often lead to problems. Use 'Pascal Case' (example: `MyVariableName` -> each word starts with uppercase).

- Difference between Print String & Print Text
  - Print String: For debugging. Shows messages in the editor (top-left screen) and output log. Uses colored plain text.
  - Print Text: Same purpose, but supports rich text formatting, localization, and better performance in packaged builds. Preferred for production or multi-language.
  - Use Print String when debugging. Use Print Text when formatting, translating, or shipping.

- Variable Types (I already know most of the basic ones, but its better to write them down):
  - Boolean: True / False
    - You can use `select` for boolean in event graph.
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

- Structs:
  - You can create a 'struct' (content browser -> new -> blueprints -> structure), then create some variables. Then go to blueprint event graph -> right click -> add -> 'name of structure' -> Options: Break, Make, Set...
  - Struct (name of the structure) can also be a type of variable.
  - If we drag&drop the variable (which has a struct type) and choose 'get', we can right click on the blue pin and decide to 'Split Struct pin'.
  - It's basically a variable which stores multiple variables in it
  - Removing an existing variable from struct can cause issues in blueprints.
  - You can have array of structs

- Enums:
  - You can create 'enum' (content browser -> new -> blueprints -> enumeration).
  - Enumerator is a number between 0 and 256
  - Enum (name of the enumeration) can also be a type of variable.
    - After you assign a enum as a type of variable, you can set Default value of the enum in the variable details (in blueprint).
  - You can assign `Get "VariableName"` to print string (if it's enum).
  - If you drag&drop the variable (which has an enum type) and choose 'get', you can drag a node out of it to create `Switch on "EnumName"` where you can drag more nodes out of it based on enumerations names in your enum.

- Functions:
  - Function is basically a block of code which adds functionality to your program.
  - You can add input/output parameters for a function in its details panel
  - You can create something called 'Local Variables' in functions.
  - You can not add a delay node in functions.
  - Can be called from other blueprints. (can be disabled by setting access specifier to private)

- Macros:
  - You can not add a delay node in functions. That's why we use macros
  - Can not be called from other blueprints.

- Collapsed Graph
  - Notes are in `Content/Blueprints/BP_CollapsedGraph`

- Branching
  - There was just a branch :(
  - BUT, You can use `select` for boolean in event graph :)

- While Loop
  - `Condition`: (as long as its true, `Loop Body` will be executed)
  - `Loop Body`: Content to loop
  - `Completed`: What to do if loop is complete and condition is false
  - Note: avoid using loops with larger data sets (>100) and use c++ instead. Why? C++ is faster than blueprint

- Functions
  - Functions can either be Pure or Impure. The main difference is that Pure Functions promise not to modify state or the members of the class in any way, while Impure Functions are free to modify state. Pure Functions are generally used for getter Functions or operators that just output a data value.

- Game Instance
  - Created by going to explorer > blueprints > more > game instance
  - What this does is that it is referrign to the whole game application
  - Event init -> game start

### Misc
- Anything that can be placed in a level is called an 'Actor'
- Light Movability:
  - Types can be changed in Transform section in the details panel
  - Types of Light Movability:
    - Static: Can't be changed in-game
    - Stationary: Can only change color and intensity in-game, but cant move
    - Movable: Can be moved and changed in-game
- 'vice versa' means 'the other way around' in english
