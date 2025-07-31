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

- That dots are called 'pins'. Atleast hey call them 'pins'
- That 'little white shit' is called an execution pin.

- Get Actor Location is a function, but it does not have execution pin. Then it is called a 'pure function'

- Event Tick is a function
  - It is called every frame

 

### Misc
- You can hit 'end' on your keyboard to snap items to the ground (landscape) in the level.
- Anything that can be placed in a level is called an 'Actor'
- Light Movability:
  - Types can be changed in Transform section in the details panel
  - Types of Light Movability:
    - Static: Can't be changed in-game
    - Stationary: Can only change color and intensity in-game, but cant move
    - Movable: Can be moved and changed in-game