Prefab created by chrjen#2648 (discord)

If you can, please credit me if you use this in a map.
Making these takes time and effort.

===========

Simple keycard reader. Reacts only to keycards and triggers only on the correct one.

How to:
1. Drag .vmap file to <SDK>/content/hlvr/maps/prefabs
2. From withing hammer, click prefab tab and drag keycard_reader.vmap onto a wall and rotate as necessary.
3. While selected, hit alt+Enter and open the Outputs tab.
4. Add output for OnCorrectKeycard to unlock e.g. a door.
5. Create a new prop_physics, set model to 'models/props/misc/keycard_001.vmdl' and give it a name.
6. Select prefab again, click on eye-drop tool next to Keycard name and click the keycard.


Inputs:
  - Activate: Makes the indicator green.
  - Reset: Makes the indicator red.
  - Enable: Enables the scanner.
  - Disable: Disables the scanner.
  - Toggle: Toggles between enabled and disabled.

Outpus:
  - OnCorrectKeycard: Triggered when the correct keycard is scanned.
  - OnIncorrectKeycard: Triggered when an incorrect keycard is scanned.
  - OnNotKeycard: Triggered when an item that was not a keycard got scanned.
  - OnItemScanned: Triggered when any item got scanned.

Bonus tip:
	Manage all keycard colours from one place:
		1. Shift+Ctrl+M
		2. Go to Map Variables tab
		3. Add variable, ex.
			Name: my_door_keycard_colour
			Type: color255
			Value: <your colour>
		4. Click on reader and keycard, and alt+Enter.
		5. Find the colour property, click on the chain symbol and pick your variable name.
		6. Colour can now be seen and changed from the Map Variables tab.
	Multiple accepted keycards:
		Just makes sure they all have the same name. Hold shift and drag keycard to easily make copies.