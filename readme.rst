
Blender Patch Templates
#######################

This repository is to host patches which apply to the Blender ``git.blender.org``, which are good examples
of how to add functionality.

Motivation
==========

Blender is a complex application, some changes may end up needing to touch C, C++, Python and
build systems (CMake and SCons), this increases the barrier of entry to anyone who is interested to become involved.

Tutorials can work however you end up copying and pasting from them and when they become out-dated its not always
clear if the changes are made incorrectly or if the tutorial its self is wrong.


Proposal
========

While we can't expect to make this process _easy_ we can at least provide some examples to help developers.

This repository plans to host multiple patches, each which can be applied on its own and makes some addition to
Blender which can be used as the basis for further work.


Goals
-----

- Help new developers understand Blender's codebase.
- Patches should be well commented to help in understanding the purpose of changes.
- Patches should be easily manipulated and customized once applied.
- Patches should be up to date and apply to the latest revision of Blender's git repository.


Pitfalls
--------

There are some things which we would like to avoid:


Cargo Cult Programming
^^^^^^^^^^^^^^^^^^^^^^

*Developers applying changes without understanding what they do.*

The purpose of these patches is so you can quickly identify what changes are needed and
then extend them for your own use, rather then blindly copying changes and expecting it to work because you followed
the template, admittedly early on many developers will do their fair share of copy-paste from existing code,
but we would encourage developers to take care they understand all the changes made.


New Features (because we can!)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Generally the bottleneck with the development is _not_ that we can't add new features fast enough.

New features are of course interesting, but if you spend 5 minutes to edit one of these patches to add a new feature,
this is a hint that probably any of Blender's existing developers could have added this, and you may need to expand
upon this some more, or that the feature may need to be part of some larger project.

Having said that, making small changes right away is a great way to learn.


Prerequisites
=============

To make use of these patches you should have Blender building and a development environment setup.

See:

- http://wiki.blender.org/index.php/Dev:Doc/Building_Blender
- http://wiki.blender.org/index.php/Dev:Doc/New_Developer_Env


Usage
=====

Each patch is comprised of 2 files, a read-me and a diff which can be applied to Blenders source using. eg.

.. code-block::

    git apply modifier_deform.diff

If any of the patches fail to apply to the latest Blender version report an issue,
However you can always checkout the version of Blender which the patch was made against.


Patches
=======

Currently this is more of a TODO list.

*Done*

- ``modifier_deform.diff`` simple deformation modifier (moves vertices).

*TODO*

- ``modifier_generate.diff`` simple modifier which generates new geometry.
- ``sequencer_type.diff`` define a new sequence strip type.
- ``texture_type.diff`` define a new texture type.
- ``cycles_shader_node.diff`` define a new cycles shader type.
- ``compositor_node.diff`` define new compositor node.
- ``editmesh_tool.diff`` edit-mode mesh tool.
- ``editcurve_tool.diff`` edit-mode curve tool.
- ``ui_button_type.diff`` define a new button type.


Contributing Back
=================

If the patch is finished and you think its useful to include in Blender releases, you can submit the patch here.

Blenders developer site: http://developer.blender.org
Under the **BF Blender** heading, **Submit Code**

