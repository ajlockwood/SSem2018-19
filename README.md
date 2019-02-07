## 2/6/19
Added Sun.

Sun:
  A large, undamaging projectile that repeatedly spawns 10 quick, very short-lived projectiles around itself in all directions. 
  "Shotgunning" with this will prove effective.
  Total Damage: 8x10

Other Changes:
  Icicle:
    Now pierces and explodes at the end of its movement instead of when it hits something.
    Speed increased from 1750 to 2500.
    Lifetime decreased from 1.75 to 0.5 seconds.

  Fixed a bug that allowed projectiles to move along the Z-axis after bouncing.
  Reworked how projectiles are spawned to improve performance when spawning many projectiles on the same frame. This is because Sun was causing undue lag.
  Added a new class of projectiles that can collide with other projectiles and bounce off of walls. BouncyBall and SuperBouncyBall added to this category.


## 2/4/19
Added Parallel and Perpendicular.

Perpendicular:
  A short-lived projectile that spawns a line of damaging projectiles perpendicular to its Z-axis rotation at the end of its lifetime.

Parallel:
  A derivative of Perpendicular that instead fires one instance of perpendicular on either side of itself when it expires.
  The result of this is two parallel lines of projectiles that are also parallel to the original projectile's direction vector.


## Changelog as of 2/4/19
## Changes and additions before this have been undocumented. Whoops!