===============================
Imported Objects (Technical)
===============================

.. _imported-objects:

When loading a modifier preset, the add-on automatically imports certain internal objects.  
These are **essential** for preset operation and must be preserved.

Modifier Host Object
---------------------

A dedicated *modifier host object* is created during the initial load of a preset.

**Name Format**::

    modstack.<preset_id>

- `<preset_id>` is the unique identifier of the preset.
- This object contains all saved modifiers and acts as the technical reference point.

.. warning::

    **Do not rename or delete** the host object.  
    It is required for correct functionality of the preset.

Supporting Objects
-------------------

If the preset uses additional geometry (such as empties, curves, or linked objects), they will also be imported.

**Name Format**::

    modstack.<original_mesh_name>

- The name is derived from the **original mesh data**, not the object name.
- These supporting objects may be renamed but **must not be deleted**.

Object Visibility
-------------------

Imported objects are **not linked to any active scene**.

.. note::

    As a result:

    - They are **not visible in the Outliner**
    - They are **not rendered**
    - They **do not affect scene statistics**

Data Integrity
----------------

.. danger::

    Deleting any of the imported objects will cause the preset system to fail.  
    Blender does not provide warnings in this case — handle with caution.

----

For practical usage instructions, see: :doc:`features/load`
