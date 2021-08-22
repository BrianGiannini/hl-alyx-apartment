Prefab created by chrjen#2648 (discord) v.1

https://discord.gg/PnyMTtP


If you can, please credit me if you use any of these in a map.
Making these does take time and effort!

===========

The combine battery post, fully working. Used by the combine to power all their special gear remotely off the main power-grid.
Just insert a combine battery and it will power up. Even works with reviver hearts!

A second version, combine_battery_post_no_trigger.vmap, is also included. It has no trigger to open when the player goes near,
so you need to do that yourself by sending inputs to the prefab. This is included in case you want to place the battery post in
a small space where the normal trigger would clip through the wall into e.g. another room.

Outputs:
  - OnPowerOn: Triggered when the post starts outputting power.
  - OnPowerOff: Triggered when the post stops outputting power.

Inputs:
  - Open: Opens the post.
  - Close: Closes the post.

How to:
  1. Drag .vmap file to <SDK>/content/hlvr/maps/prefabs
  2. From withing hammer, click prefab tab and find the prefabs and drag them onto the floor and position and rotate if necessary.
  3. With the prefab selected hit alt+Enter and go to Outputs tab and add an output for OnPowerOn to activate something when a battery is inserted.

PS: Ctrl+Shift+F2 hides trigger volumes.