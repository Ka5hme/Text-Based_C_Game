# Text-Based_C_Game

Rules:

The world consists of a series of rooms, joined by doors. A room can have multiple doors to other rooms. Every door can be locked or not. A room can also contain keys and creatures.

The player acts as a person (the player character, or PC) trying to escape the maze of rooms. The PC has a carrying capacity and a leadership parameter. The carrying capacity, which is an integer, indicates how many keys the PC can carry; the leadership parameter, which is another integer, indicates how many escapees can follow the PC at the same time.

Every key can be used to unlock precisely one specific door.

There are two kinds of other creatures in the maze: escapees and guards. Every guard has a target escapee he must ensure does not escape (this can be the PC). Whenever one or more escapees encounter one or more guards in the same room, the following happens:
- if there are equal or more guards than escapees, all creatures (including the PC, escapees, and guards) are returned to their original locations. Carried items are not confiscated. The PC can be returned to the original location no more than 5 times; if the PC is caught for the fifth time, the game is lost.
- if there are more escapees than guards, any guards whose targets are in the group of escapees start following the escapees in the hope that they'll encounter more guards. Other guards do not follow.

The goal of the game is for the PC to reach a specific door, which is the exit.
