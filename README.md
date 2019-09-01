# assignment01
 
##Step One##
*Creating a New Scene*

Following the tutorial, I created a new scene called **Starting Area**.

##Step Two##
*Painting a Level*

I used the **Tile Palette** to create the level structure.

##Step Three##
*Testing the Level*

Sections 'a' and 'b' were tested first, the other section tests will be referenced chronologically.

a) This was done several times over the course of developing the level. 
b) Tested key bindings worked and controlled **Ellen**.
c) Tested speed of **Moving Platform** and wait times at each node. 
d) Tested the **Pushable Box's** interaction with **Pressure Pad**.
e) Tested **Door** interaction with **Pressure Pad**
f) Tested **Pressure Pad** interaction with **Spitter**
g) Tested **Health Pickup**.
h) Tested **Teleporter** and **Transition Starts and Ends**.

##Step Four##
*Adding Moving Platform*

**Moving Platfrom** added to map.
Back to Step 2 for more level design. The platform had to take the player somewhere.
Added nodes 3 and 4 to the platform and checked that the platform looped between all four.
Back to Step 3, section c.

##Step Five##
*Opening a Door with Events*

Added **Door, Pressure Pad, Reusable Switch, and Pushable Box** to level.
Made the Box a **Trigger** so it would trigger switches. 
*Step 3, sections d & e*
Decided **Reusable Switch** interacted with the **Hitbox** of the **Pushable Box** too strangely, and wasn't consistently openning doors.
Removed Switch.
Added extra **Door**, used **Pressure Pad's** *On Release* component to close **Doors** if released.

##Step Six##
*Enemies*

Added **Chomper and Spitter** to level.
Changed **FOV** so enemies wouldn't knock Ellen off the level. 
Adjusted enemy location for even more safety. Tests needed to be able to run quickly and efficiently. Killing Ellen early was getting in the way of that.

##Step Seven##
*Damaging with Objects*

Changed **Spitter** location to under pushable box.
**Spitter** interacted strangely with **Pressure Pad**, which was also under the **Pushable Box**
*Step 3, section f.*
Moved **Spitter** to a postion where it wouldn't accidentally trigger the doors to open and close.
Because Ellen was getting damaged, and to test my skill, I added a **health pickup** behind the first **Door**
*Step 3, section g*

##Step Eight## 
*Decorating*

Added Alien Flora and Alien Box Assets. Tested Alien Wall Tiles, which had layering issues. Removed Alien Wall Tiles.

##Step Nine##
*Teleporting the Player*

Added **Teleporters** and **Transitions**
Set **TransitionStart** to send Ellen to **TransitionEnd**, located in the same scene.
Set **TransitionStart1** to send Ellen to **TransitionEnd1**, located in **Zone 1**, a different scene.
*Step 3, section h*
**TransitionStart1** was teleporting Ellen to beginning of **Starting Area** instead of **Zone 1**.
Set **Transition Destination Tag** of **TransitionStart1** to A, while **TransitionEnd's** tag is set to B.
Set **TransitionEnd1's** Destiniation tag to A and placed it in **Zone 1**

##Step Ten##
*Having Fun*

Tested entire game 3 times, fixing bugs.
Played Zone 1 and 2. 
Adjusted enemy location.
