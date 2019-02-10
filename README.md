## 2/10/19

Added single-player Steam platform support under appID 480 (Valve's developer test ID).
Sources: 
    https://docs.unrealengine.com/en-us/Programming/Online/Steam
    https://www.youtube.com/watch?v=TPakLkxc6f0&t=1060s  

...Then proceeded to fix the multitude of bugs that arose from testing the game for the first time in standalone mode...

## 2/8/19
Added Swap

Swap:

  A fast projectile that swaps the location of the player hit with the player who fired it. Snares for 0.3 seconds.

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