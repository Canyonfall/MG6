# MG6

1. The entire for loop will complete before the Update() method finishes. So if the loop takes a really long time to finish, it will make the game lag or freeze temporarily because Unity has to finish the loop before moving to the next frame.

2. There is an issue that the player sometimes fall through a platform instead of landing on top of it. This can happen because the logic temporarily disables collisions to let the player jump through the bottom of platforms. If the collision is not turned back on at the correct time, the player can also pass through the platform when falling down.
