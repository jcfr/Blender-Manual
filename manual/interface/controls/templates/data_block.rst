.. _ui-data-block:

***************
Data-Block Menu
***************

A set of menu buttons used to link :doc:`/data_system/data_blocks` to each other.
Data-blocks are items like meshes, objects, materials, textures, and so on.
If data-blocks are linked the data will be updated across all of the users when edited.

.. figure:: /images/interface_data-block.jpg
   :align: right

   The Data-Block menu with a search input.


Type
   Shows an icon indicating the data-block type. It opens up the following pop-up menu.
   The data-block can be dragged from here. e.g to drag an material onto an object in the 3D View or
   into a :ref:`ui-data-id` field.

   List
      A list of data-block available in the current blend-file or link in to select an item from.
      The menu may show a preview besides the items and
      a search box to search the items in the list by name.
Name
   Displays the internal name of the linked Data-Block, which can be edited as a regular text field.
   If a name already is in assigned Blender will add a digit to the name like ".001".
User count
   Displays the number of users of the data. Clicking on it to make it a single-user copy,
   with it linked only to the active object/object's data.
Fake User ``F``
   Keeps the data-block saved in the blend-file, even if it has no real users.
New/Add ``+``
   Creates a new data-block or duplicates the current data-block and applies it.
Open file
   Opens the :doc:`File Browser </editors/file_browser/introduction>`.
Unpack file
   :ref:`Unpack <pack-unpack-data>` the file packed into the current blend-file to external ones.
Unlink data-block ``X``
   Clears the link.

Sometimes there is a :ref:`list <ui-list-view>` of applied data-blocks
(such as a list of materials used on the object).


Data-Block Types
----------------

.. image source: Scene tab --> Active keying set panel --> ID-block (sound replaced)

.. figure:: /images/data_system_id-types.png

   Data-blocks types with their icon.


Preview
=======

.. figure:: /images/interface_data_block_preview.png

   The Data-Block menu with preview.

In the Tool Shelf is a version of the data-block menu with a bigger preview.


.. rename to selector?

.. _ui-data-id:

Data ID
=======

.. figure:: /images/interface_data_id.png

   The Data ID.

A Data ID is a text field with icon on the left, which opens a gray pop-up.
It is used to reference data-blocks selected by their name.

Type
   The icon on the left specifies the accepted data-block type.
Name
   The text field functions as a search field by matching elements in the list.
   Press of :kbd:`Tab` for auto-complete names to the level a match is found.
   If more than match exists you have to continue typing.
   If you type an invalid name, the value will remain unchanged.
List
   Lets you select the data-block directly.
Eye Dropper
   In some Data IDs there is an :doc:`/interface/controls/buttons/eye_dropper`
   available through the pipette icon on the right side.
Remove ``X``
   Click  the ``X`` button on the right to remove the reference.


Sub IDs
-------

.. figure:: /images/interface_controls_templates_data_subids.png

Vertex Group
   If selected object in the *Name* field is a mesh or a lattice,
   an additional field is displayed where a vertex group can be selected.
Bone
   If selected object in the *Name* field is an armature,
   a new field is displayed offering the choice to specify
   an individual bone by entering its name in the *Bone* data ID.

   Head/Tail
      If a Bone is set, a new field is displayed offering
      the choice of whether the head or tail of a Bone will be pointed at. 
      The slider defines where along this bone the point lies interpolating along the bone axis in a straight line.
      A value of zero will point at the Head/Root of a Bone,
      while a value of one will point at the Tail/Tip of a Bone.

      Use B-Bone Shape
         When the bone is a :doc:`/rigging/armatures/bones/properties/bendy_bones`,
         click on this button to make the point follow the curvature of the B-Spline between head and tail.
