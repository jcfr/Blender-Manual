..    TODO/Review: {{review|text=add more examples of possible effects
      (also some vid) and move the how-to-activate explanation in a new page}}.

************
Introduction
************

Dynamic paint is a modifier and physics system that can turn objects into paint canvases
and brushes, creating vertex colors, image sequences or displacement.
This makes many effects possible like, for example footsteps in the snow,
raindrops that make the ground wet, paint that sticks to walls, or objects that gradually freeze.


Activating the modifier
=======================

.. figure:: /images/physics_dynamic-paint_introduction.png

   How to activate the Dynamic Paint.

Dynamic Paint can be activated from the "Physics" tab of the "Properties" editor.


Types
=====

Modifier itself has two different types:

:doc:`Canvas </physics/dynamic_paint/canvas>`
   Makes object receive paint from Dynamic Paint brushes.

:doc:`Brush </physics/dynamic_paint/brush>`
   Makes object apply paint on the canvas.

.. note::

   You can also enable brush and canvas simultaneously.
   In that case same object's "brush" does not influence its "canvas",
   but can still interact with other objects in the scene.

.. seealso::

   - `A step-by step introduction <https://www.miikahweb.com/en/articles/blender-dynamicpaint-basics>`__
   - `A detailed guide that covers every setting with images and examples
     <https://www.miikahweb.com/en/articles/dynamic-paint-guide>`__ (Currently not up-to-date)
