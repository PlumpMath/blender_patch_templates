
Deform Modifier
###############

This modifier deforms vertices based on a strength slider and a vertex group.

Usage
=====

To use simply add a mesh or curve object, then add a modifier, select **My Deform** from the drop down list.

Editing
=======

Most of the interesting editing to be had is in ``MOD_mydeform.c``, ``mydeform_do`` function.


Keywords
========

When updating this patch be sure to replace the following.

- ``MyDeform``
- ``MY_DEFORM``
- ``mydeform``
- ``mmd`` (stands for ``MyDeformModifierData``)


Observations
============

The modifiers icon is defined in multiple places (ideally it would be defined centrally)

There is some opportunity to make this modifier multi-threaded if the vertices can be deformed in any order.
See shrink-wrap modifier for an example of this.

