# DigitalPoi
Experimenting with motion graphics with HTML5 Canvas

Digital Poi started out with me attempting to emulate Adobe AfterEffects' stock "Radio Waves" effect using javascript.

It ended up turning into a side project and hobby where I experimented with utilizing different physics equations to simulate fluid
motion. Within the source code you can find the equations for position, velocity, acceleration, magnitude vectors, and radius.

The simulations are interactive and can be controlled using the mouse and the following keys:  W A S D Q E F

The paticle generator is initialized in the Particle() function. This sets the values for the particles being generated at the user's mouse
position. 

The movement and motion comes from the Particle.draw() function. Here, all the values are updated every frame. The differences and 
specifics of each particles movement comes from the magnitude, vs, vy, and radius values. These values generally vary based on the particle's
life value, which increases over time until the particle reaches its last cycle and gets deleted.

This allows for a pseudo-time value, a value that constantly increases but then resets. With a value like this, experimentation with
mixtures of different basic trig function allow for complex, satisfying oscillations among the particles.

The series of paths that follow the physics section is responsible for creating the two axis symmetry.

To experiment with the source code, open any of these files with a text-editor of your choice.

To use them, simply open the file in your browser. These are static html files and don't require any extra configuration to test and use.
