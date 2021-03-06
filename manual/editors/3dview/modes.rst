
************
Object Modes
************

.. _fig-view3d-mode-select:

.. figure:: /images/editors_3dview-mode.jpg
   :align: right

   The Mode select menu.

*Modes* are a Blender-level object-oriented feature,
which means that whole Blender application is always in a singular mode,
and that the available modes vary depending on the selected active object's type --
most of them only enable the default *Object Mode* (like cameras, lamps, etc.).
Each mode is designed to edit an aspect of the selected object.
See Tab. :ref:`tab-view3d-modes` below for details.

You set the current mode in the *Mode* selector of *3D View* header
(see Fig. :ref:`fig-view3d-mode-select`).

.. note::

   You can only select objects in *Object Mode*.
   In all others, the current object selection is "locked"
   (except, to some extent, with an armature's *Pose Mode*).


Modes might affect many things in Blender:

- They can modify the panels and/or controls available in some Properties editor tabs.
- They can modify the behavior of the whole editor, like e.g.
  the *UV/Image Editor* and *3D View*.
- They can modify the available header tools (menus and/or menu entries, as well as other controls...).
  For example, in the *3D View* editor, the *Object* menu in *Object Mode* changes to a *Mesh* menu in
  *Edit Mode* (with an active mesh object!), and a *Paint* menu in *Vertex Paint Mode*...

.. _tab-view3d-modes:

.. list-table:: Blender's Modes
   :header-rows: 1
   :class: valign
   :widths: 10 25 15 50

   * - Icon
     - Name
     - Shortcut
     - Details
   * - .. figure:: /images/icons_object-mode.png
          :width: 35px
     - *Object Mode*
     - *None* [1]_
     - The default mode, available for all object types,
       as it is dedicated to *Object* data-block editing (e.g. position, rotation, size).
   * - .. figure:: /images/icons_edit-mode.png
          :width: 35px
     - *Edit Mode*
     - :kbd:`Tab` [1]_
     - A mode available for all renderable object types,
       as it is dedicated to their "shape" *Object Data* data-block editing
       (e.g. vertices/edges/faces for meshes, control points for curves/surfaces, etc.)
   * - .. figure:: /images/icons_sculpt-mode.png
          :width: 35px
     - *Sculpt Mode*
     - *None* [1]_
     - A mesh-only mode, that enables Blender's mesh 3D-sculpting tool.
   * - .. figure:: /images/icons_vertex-paint.png
          :width: 35px
     - *Vertex Paint Mode*
     - *None* [1]_
     - A mesh-only mode, that allows you to set your mesh's vertices colors (i.e. to "paint" them).
   * - .. figure:: /images/icons_texture-paint.png
          :width: 35px
     - *Texture Paint Mode*
     - *None* [1]_
     - A mesh-only mode, that allows you to paint your mesh's texture directly on the model, in the 3D Views.
   * - .. figure:: /images/icons_weight-paint.png
          :width: 35px
     - *Weight Paint Mode*
     - :kbd:`Ctrl-Tab` [2]_
     - A mesh-only mode, dedicated to vertex group weighting.
   * - .. figure:: /images/icons_particle-edit.png
          :width: 35px
     - *Particle Edit Mode*
     - *None* [1]_
     - A mesh-only mode, dedicated to particle systems, useful with editable systems (hair).
   * - .. figure:: /images/icons_pose-mode.png
          :width: 35px
     - *Pose Mode*
     - :kbd:`Ctrl-Tab` [2]_
     - An armature only mode, dedicated to armature posing.
   * - .. figure:: /images/icons_grease-pencil.png
          :width: 35px
     - Edit Strokes Mode
     - :kbd:`D-Tab`.
     - A Grease Pencil only mode, dedicated to editing Grease Pencil strokes.


.. [1] :kbd:`Tab` toggles *Edit Mode*.
.. [2] :kbd:`Ctrl-Tab` switches between the *Weight Paint Mode* (meshes)/*Pose Mode* (armatures) ,
   and the other current one (by default, the *Object Mode*).
   However, the same shortcut has other, internal meanings in some modes
   (e.g. in *Sculpt Mode*, it is used to select the current brush)...

As you can see, using shortcuts to switch between modes can become quite tricky, especially with meshes.

.. note::

   The cursor becomes a brush in:

   - :ref:`painting-vertex-index` mode
   - :ref:`painting-weight-index` mode
   - :ref:`painting-texture-index` mode.

.. Todo add to chart

We will not go into any more detail on modes usages here, However,
most of them are tackled in the :doc:`modeling chapter </modeling/index>`, as they are mainly related to this topic.
The *Particle Edit Mode* is discussed in the :doc:`particle section </physics/particles/mode>`,
and the *Pose Mode* and *Edit Mode* for armatures, in the :doc:`rigging one </rigging/index>`.

.. note::

   If you are reading this manual and some button or menu option is referenced that does not appear on your screen,
   it may be that you are not in the proper mode for that option to be valid.
