..    TODO/Review: {{review}}.

*************
Fluid Control
*************

Using the Lattice-boltzman method, the fluid is controlled using particles which define local
force fields and are generated automatically from either a physical simulation or a sequence
of target shapes. At the same time, as much as possible of the natural fluid motion is preserved.

.. only:: builder_html and (not singlehtml)

   .. youtube:: WruTNnF6Ztg

   .. only:: not builder_html and (singlehtml)

      A video can be found at https://www.youtube.com/watch?v=WruTNnF6Ztg 


Options
=======

.. figure:: /images/physics_fluid_types_control.jpg

   Fluid control options.

Enabled
   Controls weather the control object contributes to the fluid system.
   This is useful when animating the fluid control object.
Quality
   Higher quality result in more control particles for the fluid control object.
Reverse Frames
     Reverses the control object's movement.
Time
   You specify the time interval (start and end time) during which the fluid control object is active.
Attraction Force
   Specifies the force which gets emitted by the fluid control object.

   Strength
      The strength of the force.
      Positive force results in attraction of the fluid, negative force in avoidance.
Velocity Force
   If the fluid control object moves, the resulting velocity can also introduce a force to the fluid.

   Strength
      The strength of the effect.
   Radius
      The radius of the force.


Examples
========

In these examples,
the Fluid Control is used to control part of the fluid so that it has a certain shape
(the sphere drop or the teapot drop) before it falls in the rest of the fluid:

.. figure:: /images/physics_fluid_types_control_example1.jpg

   Falling drop.

.. figure:: /images/physics_fluid_types_control_example2.jpg

   "Magic Fluid Control."
