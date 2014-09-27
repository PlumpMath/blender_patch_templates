
BMesh Modifier
##############

This modifier deletes faces matching a size value.

BMesh API provides advanced mesh editing functionality not found with ``DerivedMesh``
(the native mesh format for modifiers).

Using BMesh API incurs overhead, converting from and to ``DerivedMesh`` so only use BMesh
when advanced editing is requited.


Usage
=====

To use simply add a **Monkey** mesh object, then add a modifier, select **My BMesh** from the drop down list.

Change the sides from 3 to 4 and see the difference.


Editing
=======

Most of the interesting editing to be had is in ``MOD_mybmesh``, ``mybmesh_do`` function.


Keywords
========

When updating this patch be sure to replace the following.

- ``MyBMesh``
- ``MY_BMesh``
- ``mybmesh``
- ``mmd`` (stands for ``MyBMeshModifierData``)


Observations
============

The modifiers icon is defined in multiple places (ideally it would be defined centrally)

