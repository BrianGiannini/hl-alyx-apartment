Prefab created by chrjen#2648 (discord) v.3

If you can, please credit me if you use this in a map.
Making these takes time and effort.

===========

Basic light switch as seen in the game. Can be used to turn things on or off.

Changes:
  - v.3
  	- Added option to change initial state instead of always spawning in the off position.
  	- Added option to change skin and colour of both the switch body and the switch.
  	- Added new output OnChange.
  - v.2
    - Made the output accessible from outside the prefab removing the need to collapse it.

Outputs:
  - OnTurnOff: Triggered when the light switch switches off.
  - OnTurnOn: Triggered when the light switch switches on.
  - OnChange: Triggered every time the light switch switches on or off.

How to:
1. Drag .vmap file to <SDK>/content/hlvr/maps/prefabs
2. From withing hammer, click prefab tab and drag light_switch_2 onto a wall and rotate if necessary.
3. With the prefab selected hit alt+Enter and go to Outputs tab and add desired outputs.