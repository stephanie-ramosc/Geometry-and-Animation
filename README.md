# Geometry-and-Animation

Implement of geometric modeling and animations using the 2D HTML5 canvas.

Part 1: Ateroid-Animation and keyboard
Objective: Display animated objects and control them using the keyboard, similar to Asteroids game.
Code asteroid.html contains a canvas and a GUI to help debugging by enabling the visualization and modification of the parameters.
Q1) Ship drawing:
a) Transform asteroid spaceship in drawShip() so that it is centered on (x0, y0) and has the correct angle. Use only ctx.translate and ctx.rotate for that.
b) Replace the wireframe of the spaceship by a nice image of spaceship. This image should be centered on the wireframe, take roughly the same amount of space, and rotate and translate in the exact same way as the wireframe did.
Q2) Ship control:
Using keyboard polling to check if an arrow key or motion key is down at each animation frame. If an arrow is down, do the following:
- up arrow/i: accelerate the ship using a fixed acceleration in the forward direction.
- down arrow/k: accelerate the ship using a fixed acceleration in the backward direction.
- right arrow/l: rotate the ship clockwise using a fixed angular velocity.
- left arrow/j: rotate the ship counter-clockwise using a fixed angular velocity.
Q3) Bullet:
When the user presses key Space (onKeyDown), fire a bullet from the spaceship in the forward direction. The bullet should move with fixed velocity during 2 seconds, then disappear. The displacement of the ship after the bullet has been fired should not influence its trajectory. No bullet can be fired again until the first one has disappeared, as the ship needs to reload its gun.

Part 2: Pupet-Transform Composition
Objective: Use transform composition to draw articulated objects.
Code puppet.html that contains a canvas and a GUI to modify the parameters.
Create a function drawPuppet(). The translation of the puppet based on parameter (x0,y0) and the articulations based on angles a1, a2 and a3 should be performed using the composition of canvas transforms (ctx.translate, ctx.rotate...). Erase and redraw the whole scene whenever any parameter changes.
