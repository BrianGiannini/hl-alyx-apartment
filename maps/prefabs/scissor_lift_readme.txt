Prefab created by chrjen#2648 (discord) v.1

https://discord.gg/PnyMTtP


If you can, please credit me if you use this in a map.
Making these does take time and effort!

===========

Working scissor lift with hoist boxes with buttons. Goes up and down!

Scissor lift inputs:
  - StartExtend : Makes the scissor lift go up.
  - StartRetract : Makes the scissor lift go down.
  - Stop : Stops the scissor lift from moving.
  - LockUp : Stops the scissor lift from moving up.
  - LockDown : Stops the scissor lift from moving down.
  - UnlockUp : Allows the scissor lift to move up.
  - UnlockDown : Allows the scissor lift to move down.

Hoist buttons outputs:
  - OnUpPressed : Triggered when the top button gets pressed.
  - OnDownPressed : Triggered when the bottom button gets pressed.
  - OnUpReleased : Triggered when the top button gets released.
  - OnDownReleased : Triggered when the bottom button gets released.

How to:
  1. Drag .vmap files to <SDK>/content/hlvr/maps/prefabs
  2. From withing hammer, click prefab tab, find the prefabs and drag them onto the floor and position and rotate as necessary.

Add additional stops:
  To make the scissor lift stop at a specific height add a filter_activator_name entity with Filter Name set to "@lift_logic_height_check_brush".
  Next create a trigger_multiple that touches the long vertical column and set Filter Name to the name of the filter_activator_name you just created.
  The trigger should trigger when the scissor lift passes it. Now set OnStartTouch on the trigger to Stop on the prefab and you are done.
  To stop it from going further up also tie OnStartTouch to LockUp and OnEndTouch to UnlockUp. Similar for down.

PS: Shift+O toggles editor only objects.