
***************
Normal Map Node
***************

.. figure:: /images/render_blender-render_materials_nodes_vector_normal-map.png
   :align: right

   Normal Map Node.


The *Normal Map* node generate a perturbed normal from an RGB normal map image.
This is usually chained with an *Image Texture* node in the color input,
to specify the normal map image. For tangent space normal maps,
the UV coordinates for the image must match,
and the image texture should be set to *Non-Color* mode to give correct results.


Inputs
======

Strength
   Strength of the normal mapping effect.
Color
   RGB color that encodes the normal in the specified space.


Properties
==========

Space
   The input RGB color can be in one of three spaces: Tangent, Object and World space.
   Tangent space normal maps are the most common, as they support object transformation and mesh deformations.
   Object space normal maps keep sticking to the surface under object transformations,
   while World normal maps do not.
UV Map
   Name of the UV map to derive normal mapping tangents from. When chained with an Image Texture node,
   this UV map should be the same as the UV map used to map the texture.

Outputs
=======

Normal
   Normal that can be used as an input to BSDF nodes.


Examples
========

Todo.
