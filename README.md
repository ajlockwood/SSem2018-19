## 4/1/19

Fixed a UI bug.

Fixed a bug that caused the mouse cursor to disappear while the player was firing weapons, effectively not allowing players to rotate their character while firing.

Added ChickenCoop

ChickenCoop:

	Creates a chicken coop that lasts for five seconds, spawning chickens in random directions every 0.3 seconds with a 1 in 7 chance to spawn a large chicken that lays eggs.

	Chickens explode.

## 3/31/19

Added Chicken, Comet, and Solar System.

Comet: 

	Fires a slow-moving comet that spawns slower-moving ice projectiles that move behind it. The result is a cool-looking trail effect that also deals damage. Hits walls hard.

	Damage: 75. Secondary damage: 25

Chicken: 
	
	Fires a large, randomly rotating chicken that lays eggs along its path and explodes when it hits something. It's really funny to watch.

	Will add an obnoxious chicken noise on spawn and on death to complete this amazing creation.

	Eggs spawn a new, smaller chicken after 0.5 seconds, which cannot lay its own eggs. These chickens also explode.

	Damage: 90. Chick damage: 30

	No chickens were harmed in the making of this ability.

Solar System:

	Creates an area that repeatedly spawns a comet, sun, or four asteroids in random directions every 0.5 seconds.


## 3/17/19 - 3/30/19

Took a break. (Finally!)

## 3/16/19

Fixed a few bugs to do with player character visibility.

Fixed some UI bugs

## 3/13/19

Fixed up a few UI elements and incorporated a bit of feedback.

Added a timer UI element so that users can see how long is left in a round.

Increased real-time round duration from 10 seconds to 20 seconds.

Icicle: 

	Damage increased from 35 to 40.

	Shard damage increased from 10 to 25.

Added Sniper and Piercer:

Sniper:

	A fast-moving projectile that deals high damage with a very slow fire rate.

	Damage: 90

Piercer:

	Same as sniper but can pierce through walls. Slower fire rate.

	Damage: 80

## 3/12/19

Added an in-game menu for leaving an in-progress game.

## 3/10/19

Added an additional lobby menu widget that allows the players to tell who is in their lobby.

## 3/7/19

Successfully hosted a game and connected a user from a different system using the Steam Online Subsystem. There were bugs, but nothing game-breaking. 

We played for a few minutes of testing before noting some bugs and closing the program. This marks the first successful test of a multiplayer hosted game!

This push contains no content, only the change that fixed a bug which previously didn't allow players to connect to hosted games properly after a map transition.

## 3/6/19

Fixed a particularly frustrating bug that prevented users' steam profiles from being connected to the game and showing up in the main menu.

While there is no current functional use for this information, players should now be able to see their steam profile name and portrait in the main menu.

## 3/4/19

Progress has been slow this week due to a family emergency.

Packaged the project and tested it on another system. Lo and behold it doesn't work as intended. Big surprise.

## 2/26/19

Spent the past few days getting assets ready for packaging. Packaging is a time-consuming process that gets all the code in the project ready for distribution.

This will be used to further testing by putting the project on another system and seeing what bugs this generates.

## 2/22/19

Added respawning for dead players and fixed some more ability-related bugs.

Temporarily disabled Blink, Teleport, and Swap pending a fix.

## 2/21/19

Converted the damage numbers widget to show up properly on the screen of the player who dealt damage. Huzzah!

Also cleaned up the function that was used to generate those widgets. It was really ugly before and now its only a little ugly.

Additionally, players all have their HUD's updated correctly when they take damage now.

Fixed some replication-related bugs for projectiles that spawn other projectiles.

## 2/20/19 

Began work on converting the menu and gameplay work I had done in a single player context to multiplayer. 

Players who enter the main game after a multiplayer lobby are now greeted with a pre-game movement phase followed by a unique ability selection phase.

Shots fired by the player now occur on the server and replicate to clients properly. I think I'm getting the hang of this!

	https://docs.unrealengine.com/en-us/Resources/ContentExamples/Networking

Also did some work on commenting functions and making things a little prettier.

## 2/19/19

Player characters now replicate properly; remote clients can now see the locations and rotations of actors on the server, including other replicated player characters.

	Basically this just means that players can now see each other properly in game and the server updates everyone properly when someone moves.

	https://forums.unrealengine.com/development-discussion/blueprint-visual-scripting/40390-problem-with-character-rotation-on-client

## 2/18/19

Locally spawning players into the world works now. 

	https://wiki.unrealengine.com/Replication

	https://forums.unrealengine.com/development-discussion/blueprint-visual-scripting/2238-come-learn-blueprint-multiplayer-with-me-aka-tom-s-a-glutton-for-punishment/page3?2107-Come-Learn-Blueprint-Multiplayer-with-me!-(aka-Tom-s-a-Glutton-for-Punishment)=&viewfull=1

Took one look at how much I'd have to do to move everything I'd already created so that it would work on servers and closed my session. See you tomorrow!

## 2/13-2/14/19

Several very long nights later... the lobby chat system now works! Huzzah!

Specifically...

   Players can now host a lobby and browse available lobbies to join. This puts them in a multiplayer session complete with chat system (yay).

## 2/12/19

Tried to get a rudimentary chat system to work. It's harder than it seems.

Source:

    https://www.youtube.com/watch?v=ommD3qgCrnI 

## 2/11/19

Made some more progress toward multiplayer support with the following sources:

    https://www.youtube.com/watch?v=3lN2eZIgAQ0

    https://www.youtube.com/watch?v=VATImPiTj1g

## 2/10/19
Added single-player Steam platform support under appID 480 (Valve's developer test ID).

Sources: 

    https://docs.unrealengine.com/en-us/Programming/Online/Steam

    https://www.youtube.com/watch?v=TPakLkxc6f0&t=1060s  

...Then proceeded to fix the multitude of bugs that arose from testing the game for the first time in standalone mode...

Added bland menus and barebones functionality for them.

Hosting multiplayer games is now possible (though there aren't win conditions... onward!).

Credit to mordentral for their Advanced Sessions plugin, which I am now using:

    https://forums.unrealengine.com/community/community-content-tools-and-tutorials/41043-advanced-sessions-plugin

## 2/8/19
Added Swap

Swap:

  A fast projectile that swaps the location of the player hit with the player who fired it. Deals no damage and snares for 0.3 seconds.

## 2/7/19
Added Shockwave and DualSMG

Shockwave:

  A ring that expands rapidly over a 0.5 second lifetime. Deals no damage but deflects projectiles.

DualSMG:

  A rapid-fire, high capacity weapon that shoots two projectiles at once at a 60 degree spread. Fire rate 0.05 seconds.
  
  Damage: 8x2

Other Changes:

  Fixed some bugs regarding collision and damage channels.

## 2/6/19
Added Sun and Meteor Storm.

Sun:

  A large, undamaging projectile that repeatedly spawns 10 quick, very short-lived projectiles around itself in all directions. 
  "Shotgunning" with this will prove effective.

  Damage: 8x10

Meteor Storm:

  A non-colliding marker which travels slowly. Meteors fall from the sky around it after a short delay.

  Damage: 40 per meteor

Other Changes:

  Icicle:

    Now pierces. Explodes at the end of its movement instead of when it hits something.

    Speed increased from 1750 to 2500.

    Lifetime decreased from 1.75 to 0.5 seconds.


  Added a new class of projectiles that can collide with other projectiles and bounce off of walls. BouncyBall and SuperBouncyBall added to this category.

  Reworked how projectiles are spawned to improve performance when spawning many projectiles on the same frame. This is because Sun was causing a lot of lag.

## 2/4/19
Added Parallel and Perpendicular.

Perpendicular:

  A short-lived projectile that spawns a line of damaging projectiles perpendicular to its Z-axis rotation at the end of its lifetime.

  Damage: 30x6

Parallel:

  A derivative of Perpendicular that instead fires one instance of perpendicular on either side of itself when it expires.

  The result of this is two parallel lines of projectiles that are also parallel to the original projectile's direction vector.

  Damage: 20x6x2

## Changelog Beginning 2/4/19
## Changes and additions before this have been undocumented. Whoops!