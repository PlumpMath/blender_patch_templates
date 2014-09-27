
Mesh Primitive
##############

This primitive works in a similar way to the mesh cube primitive.


Usage
=====

To use simply add a mesh from the menu and select **Wedge**.


Editing
=======

Most of the interesting editing to be had is in ``bmo_primitives.c``, ``bmo_create_wedge_exec`` function.


Keywords
========

When updating this patch be sure to replace the following.

- ``Wedge``
- ``wedge``


Observations
============

This patch is very simple and doesn't pass many options to ``bmo_create_wedge_exec``.

There is also a missing icon which would need to be added to our icons svg.

Creating a mesh one vertex at a time should typically be avoided unless the primitives are very simple,
see other examples in the same file for more interesting examples.

