Valve style prefab of the twohandlift anim interactable rolling garage door. One of the first doors/prefabs I was looking for and didn't exist. 


I built this for my map and have fixed it up and packaged it for others to save some time!


The way it's set up out of the box, if the player lifts it less than 50% it will close itself when released. If the player lifts it more than 50%, it will release from their grip and automatically raise up the rest of the way (also good for short players...) This fits what my expectation would be with a garage door of this type.


The intent for this door was for it to not be freely opened and closed by the player, so once it has been opened by the player, it will always return to fully open again if the player attempts to pull it back down to the ground.


Of course, you can collapse the prefab or save-as your own custom version if this isn't working for your specific scenario, but it felt like a useful starting place.

Relays included:
onDoorClosed | Sent when the door has closed (if the player releases it before it has lifted up, or it is forced closed by a trigger.

onDoorOpened | When the door fully opens.

onDoorTouched | When the player touches the handles, even if they let go or the door does not open.

triggerForceClosed | Use this to force close the door via trigger or debug testing.

triggerForceOpen | Use this to open the door without the player lifting it, if you have an override or are debug testing.

Enjoy,

@yost_king