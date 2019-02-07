## 2/6/19
Added Sun and Meteor Storm.

Sun:
  A large, undamaging projectile that repeatedly spawns 10 quick, very short-lived projectiles around itself in all directions. 
  "Shotgunning" with this will prove effective.

  Total Damage: 8x10

Meteor Storm:
  A non-colliding marker which travels slowly. Meteors fall from the sky around it after a short delay.

  Damage: 40 per meteor

Other Changes:

  Icicle:

    Now pierces and explodes at the end of its movement instead of when it hits something.

    Speed increased from 1750 to 2500.

    Lifetime decreased from 1.75 to 0.5 seconds.


  Added a new class of projectiles that can collide with other projectiles and bounce off of walls. BouncyBall and SuperBouncyBall added to this category.

  Reworked how projectiles are spawned to improve performance when spawning many projectiles on the same frame. This is because Sun was causing a lot of lag.

## 2/4/19
Added Parallel and Perpendicular.

Perpendicular:

  A short-lived projectile that spawns a line of damaging projectiles perpendicular to its Z-axis rotation at the end of its lifetime.

  Total Damage: 30x6

Parallel:

  A derivative of Perpendicular that instead fires one instance of perpendicular on either side of itself when it expires.

  The result of this is two parallel lines of projectiles that are also parallel to the original projectile's direction vector.

  Total Damage: 20x6x2

## Changelog Beginning 2/4/19
## Changes and additions before this have been undocumented. Whoops!