****
Load
****

The **Load** button allows you to quickly apply a preset to multiple objects.

**Loading a Preset**
    When you click the **Load** button, a list of all saved presets will be displayed.  
    The list includes a search function, making it easy to find the preset you want.

**Applying the Preset**
    After selecting a preset from the list, it will be applied to all selected objects.  
    Only compatible modifiers will be applied to each object.

**Pie Menu**
    For a faster way to load presets, use the :doc:`pie_menu`.

**Imported Objects**  
    - **Host Object**:  
        The first time you load a preset, a modifier host object will be imported with the name ``modifierpresets.preset_id``, where ``preset_id`` is the unique identifier of the preset.  
        Do not rename the host object. It is required for the preset to function correctly.  

    - **Additional Objects**:  
        If the preset uses additional objects, they will also be imported with the name ``modifierpresets.original_name``, where ``original_name`` is the name of the original object.  
        You can rename these objects as needed.  

    .. note::  
        The imported objects are not part of any scene and will not be visible in the outliner.  

    .. warning::  
        Do not delete the modifier host object or any of the imported objects. Doing so will break the preset.  