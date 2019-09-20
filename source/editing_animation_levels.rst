.. _editing_animation_levels:

Editing Animation Levels
========================
Once you have created your animation levels, you may need to work on them in order to add or insert new drawings, or rearrange the frame sequence.

All the editing can be saved by saving the level, or by saving the scene with the Save All command, thus automatically saving all of its levels.


.. _using_the_level_strip:

Using the Level Strip
---------------------
An animation level can be managed in the Level Strip. The Level Strip shows all of the drawings of the current level (even drawings not currently exposed in the Xsheet/Timeline) according to their numbering order. 

.. note:: In case a frame range of the animation level has been loaded with the Load Level dialog, only the frames within the allocated frame range will be visible in the level strip (see  :ref:`Using the File Browser <using_the_file_browser>`  ).

When a level is selected, each frame of the strip contains a level drawing, according to the level numbering order. When a frame in the strip is selected, the related drawing is displayed in the Viewer, replacing any previous displayed content, to let you work on it more easily. 

When one or more frames are selected you can perform standard cut, copy, paste, delete and insert operations. New drawings can be added, and any sequence can be renumbered. From the Level Strip, drawings can be also exposed in the Xsheet/Timeline.

When you change the order of the drawings in the Level Strip, or when a drawing is cut, deleted or inserted, and drawings are exposed in the scene, the Xsheet/Timeline will continue to contain a reference to that particular frame of the animation level, whatever its content is. When the Xsheet/Timeline contains a reference to a drawing that is eliminated in the Level Strip, the level name and number turn red, to warn you that there is no drawing available for that cell anymore.

The width of the level strip pane cannot be resized freely, because it depends on the size of the animation level preview icons, but it can be customized in the Preferences  →  Interface dialog.

.. tip:: **To edit an animation level in the Level Strip:**

    Do one of the following:

    - Select in the Xsheet/Timeline a cell containing a drawing from the animation level you want to edit.

    - Right-click the level icon in the Scene Cast and choose Display in Level Strip from the menu that opens.

.. tip:: **To scroll the Level Strip:**

    Do one of the following:

    - Middle-click and drag to scroll up or down.

    - Use the mouse wheel to scroll up or down.

    - Use the scrolling bars to scroll only within the actual level extent.

    - Use the Up Arrow and Down Arrow keys to move one frame up or down.

    - Use the Page Up and Page Down keys to scroll the visible frames up or down.

    - Use the Home and End keys to scroll up to the beginning or the end of the level strip content.

.. tip:: **To select drawings in the Level Strip:**

    Do one of the following:

    - Click a drawing to select it.

    - Click and drag to select a series of drawings.

    - Shift-click a frame to extend the selection up to that frame.

    - Ctrl-click (PC) or Cmd-click (Mac) the frames to add them to, or remove them from the selection.

    - Use the Edit  →  Select All command to select all of the level drawings.

    - Use the Edit  →  Invert Selection command to invert the current selection of drawings.

.. note:: The Select All and Invert Selection commands are also available in the menu that opens when right-clicking in the Level Strip.

.. tip:: **To exit the level strip editing mode:**

    Click a cell or select a frame in the frames area of the Xsheet/Timeline.

.. tip:: **To customize the level strip width:**

    1. Choose File  →  Preferences  →  Interface.

    2. Set the Width and Height values of the level strip Icon Size*.

    3. Restart OpenToonz to make the changes effective.


.. _editing_level_frames:

Editing Level Frames
''''''''''''''''''''
The level content can be edited one frame at a time, for example for retouching some artwork or copying a part of a drawing to a different frame, or several frames at the same time, for example to rearrange the drawing sequence.

.. tip:: **To edit a drawing of an animation level:**

    1. Select the frame in the Level Strip containing the drawing you want to modify.

    2. Use the tools to edit the drawing in the Viewer. 

.. tip:: **To edit drawings of an animation level with the Edit menu commands:**

    1. Select the frames you want to edit.

    2. Do any of the following:

    - Use the Copy command to keep in memory selected drawings for further operations.

    - Use the Cut command to eliminate selected drawings from the animation level and keep them in memory for further operations. The frames elimination causes a gap in the level numbering order.

    - Use the Paste command to paste drawings kept in memory in the animation level, starting from the selected insertion frame. The operation shifts down the following frames, and automatically renumbers them. If before the insertion frame there is a numbering gap, the pasted frames will fill the gap before starting to shift and renumber the following frames. 

    - Use the Paste Into command to paste drawings kept in memory in the frames selected in the level strip, overwriting their content. If the selection contains less frames than those kept in memory, frames in excess will be ignored; if the selection contains more frames than those kept in memory, frames in excess will be left as they are. 

    - Use the Delete command to delete selected drawings.

    - Use the Insert command to insert empty (white) frames before the selection; inserted frames will be as many as the selected ones. The operation shifts down the following frames, and automatically renumbers them.

.. note:: All of the Edit menu commands are also available in the menu that opens when right-clicking in the level strip.

.. tip:: **To edit drawings of an animation level with the Cells menu commands:**

    1. Select the frames you want to edit.

    2. Do any of the following:

    - Use the Reverse command to invert the order of selected drawings.

    - Use the Swing command to append selected drawings to the end of the selection in a reversed order. The last drawing of the selection will not be repeated.

    - Use the Step 2, Step 3 or Step 4 command to repeat selected drawings in order to have a step 2, step 3 or step 4 animation.

    - Use the Each 2, Each 3 or Each 4, command to preserve only one drawing each 2, each 3 or each 4, of the selection, and delete the others.

    - Use the Duplicate Drawing command to make a copy of the first drawing of the selection in the following frame. If the following frames already contain drawings, the duplicated drawing will be inserted by shifting the others down.

    - Use the Merge command to paste in the current level the drawings copied from a different level, according to their original frame position and regardless of the currently selected frames.

.. note:: All the Cells menu commands are also available in the menu that opens when right-clicking in the Level Strip.


.. _renumbering_and_adding_frames_in_a_level:

Renumbering and Adding Frames in a Level
''''''''''''''''''''''''''''''''''''''''
When you need to add one or several drawings to a level, you first need to create room for the new drawings. This task can be achieved either using the Insert command (see  :ref:`Editing Level Frames <editing_level_frames>`  ), or the Renumber dialog.

While the inserting operation automatically shifts the numbering of the following frames in order to make room for the new ones, the renumbering lets you control the way frames have to be renumbered. 

After the renumbering, drawings are rearranged to have an incremental numbering in the Level Strip, where blank frames are not considered. For example for a level where frames 4 and 5 are renumbered 11 and 12, the Level Strip will display only five frames correctly numbered 1, 2, 3, 11 and 12.

If you need to add a range of frames to a level, for instance for scanning them or creating some artwork, you can add it with the Add Frames dialog. This dialog allows you also to insert drawings in a level numbered in an irregular way, for example after some frames which have been cut or renumbered.

Both the renumbering and the adding frames operation fails if the numbering assigned to the frames is used by already existing frames.

.. note:: If the Automatically Create Drawings option is activated in the Preferences  →  Drawing dialog, when you want to add a drawing at the end of the sequence simply select the first grey frame available, and draw in the Viewer. 

.. tip:: **To renumber drawings of an animation level:**

    1. Select the drawings you want to renumber; also a non-continuous selection is allowed.

    2. Select Level  →  Renumber.

    3. In the dialog that opens set the Start Frame number that will be assigned to the first drawing of the selection, and the Step used to number all following frames in the selection.

.. tip:: **To add drawings to an animation level:**

    1. Select Level  →  Add Frames.

    2. In the dialog that opens sets the frame range you want to add, and the Step used to number the frames in the range.

.. note:: The Add Frames and Renumber commands are also available in the menu that opens when right-clicking in the Level Strip.


.. _reverting_level_frames_to_a_previous_version:

Reverting Level Frames to a Previous Version
''''''''''''''''''''''''''''''''''''''''''''
In case some mistakes are made during the editing of a level, or during the painting process, e.g. a drawing section is accidentally deleted, it is possible to retrieve the last saved version of the level frames.

For Toonz raster levels generated from a cleanup process, it is also possible to retrieve the original cleaned up drawings.

.. note:: In order to revert to the original cleaned up drawings the Preferences  →  Drawing  →  Keep Original Cleaned Up Drawings As Backup option has to be activated when the cleanup is performed (see  :ref:`Cleaning up Drawings <cleaning_up_drawings>`  ).

.. tip:: **To revert the level drawings to the last saved version:**

    1. In the Level Strip select the drawings you want to revert.

    2. Do one of the following:

    - Choose Level  →  Revert to Last Saved Version.

    - Right click the selection and choose Revert to Last Saved Version from the menu that opens.

.. tip:: **To revert to the original cleaned up drawings:**

    1. In the Level Strip select the drawings you want to revert.

    2. Do one of the following:

    - Choose Level  →  Revert to Cleaned Up.

    - Right click the selection and choose Revert to Cleaned Up from the menu that opens.


.. _merging_animation_levels:

Merging Animation Levels
------------------------
Toonz vector levels and standard raster levels can be easily merged into a single animation level generated by flattening them according to their stacking order, using the   →  Merge Levels command. TLV levels can be merged, using the   →  Merge TLV Levels command.

This can be useful for instance if you are sketching an animation with drawings repeated in several cells and exposed in several columns, and you want to generate a single sequence of drawings.

In both cases there is no limit to the number of columns you can merge.


.. _merging_toonz_vector_levels_or_raster_levels:

Merging Toonz Vector Levels or Raster Levels
''''''''''''''''''''''''''''''''''''''''''''
Using the   →  Merge Levels command the number of resulting drawings will depend on the number of drawings exposed in the first column on the left of the selection. When merging raster levels, the resolution of the resulting drawings will depend on the resolution of the drawings exposed in the first column on the left of the selection.

Animation levels are merged according to the following guidelines:

- The frame numbering order is followed; this means that all the drawings exposed at frame 1 will be merged to the drawing exposed at frame 1 of the first column of the selection. 

- If two different drawings are associated at different frames to the same drawing exposed in the first column of the selection, only the first one will be applied.

- Drawings not corresponding to any drawing exposed in the first column of the selection will be ignored.

- It is not possible to merge columns if more than one level is exposed in any of them.

When levels are merged, any geometrical transformation achieved by editing and moving the related column or pegbar, will be retained. 

For Toonz vector levels each drawing of the merged levels will be retained as a group of vectors in the resulting level drawings; the palette of the resulting level will contain all of the styles used in the drawings of the merged levels.

.. tip:: **To merge animation levels:**

    1. Select the columns where the animation levels you want to merge are exposed.

    2. Choose Xsheet  →  Merge Levels.

.. _merging_toonz_raster_levels:

Merging Toonz Raster Levels
'''''''''''''''''''''''''''
The   →  Merge tlv Levels allows to combine several columns containing Toonz Raster Levels creating a new TLV level. The merged columns will be eliminated from the  and replaced with a new TLV level.

Using the   →  Merge tlv Levels command the number of resulting drawings will depend on the frames combination of the involved levels. When merging Toonz Raster levels, the resolution of the resulting level will depend on the resolution of the drawings exposed in the first column on the left of the selection.

Animation levels are merged according to the following guidelines:

- The  frame numbering order is followed; this means that the merge level will be created following the frames numbering.

- If a combination of drawings will be reused the drawing previously created will be reused.

- Also the palettes of the selected levels will be merged.

When levels are merged, any geometrical transformation achieved by editing and moving the related column or pegbar, will be retained. 

.. tip:: **It is not possible to merge columns if more than one level is exposed in any of them.**

.. tip:: **To merge tlv levels:**

    1. Select two ore more columns filled with the tlv you want to merge.

    2. Choose   →  Merge tlv Levels

    3. Define File name and location in the pop up that opens and press Apply.

.. _processing_levels:

Processing Levels
-----------------
Some commands are available to process the raster levels in order to adjust the brightness and contrast or the levels, to fade the colors toward a defined set of Red, Green, Blue and Alpha values, to adjust the levels of the images or to binarize them. The Adjust Thickness command is available to modify the thickness of the lines on Toonz Vector Levels.

A preview area is available to check the result of the applied processing: you can navigate its content and set its size.

The processed images are stored in the cache and will be saved on disk using the save level or the save scene command.

.. tip:: **To resize the preview area:**

    Do any of the following:

    - Click and drag the horizontal separator. 

    - Click and drag the separator toward the window border to hide the preview area.

    - Click and drag the separator collapsed to the window border toward the window center to display again the preview area.

.. tip:: **To navigate the preview area:**

    Do one of the following:

    - Use the mouse wheel, or the zoom shortcut keys (by default + and - keys) to zoom in and zoom out.

    - Middle-click and drag to scroll in any direction.

    - Use the reset view shortcut (by default the 0 key) to display preview at its actual size.

.. _brightness_and_contrast:

Brightness and Contrast
'''''''''''''''''''''''
In case it is needed to adjust drawings in order to increase the darkness and the opacity of the drawing, it is possible to process them by calibrating the brightness and contrast.This is available only for raster levels.

.. tip:: **To process drawings brightness and contrast:**

    1. Select the images or the level frames to process in the .

    2. Choose Level  →  Brightness and Contrast.

    3. In the dialog that opens set the brightness and contrast variation.

    4. Click the Apply button.

.. _add_antialias:

Add Antialias
'''''''''''''
Allows to add antialias or to make it smoother or harder on raster and Toonz raster images.

.. tip:: **To use the Add Antialias command:**

    1. Select the images or the level frames to process in the .

    2. Choose Level  →  Add Antialias...

    3. In the dialog that opens set the threshold and the smoothness values.

    4. Click the Apply button.

.. _adjust_levels:

Adjust Levels
'''''''''''''
Adjusts the highlights and shadows of the Source content by remapping pixels intensity according to the Input and Output levels values for the RGB, Red, Green, Blue and Alpha channels.

.. tip:: **To adjust images levels:**

    1. Select the images or the level frames to adjust in the .

    2. Choose Level  →  Adjust Levels.

    3. Adjust the image levels

    4. Click the Apply button.

.. _adjust_thickness:

Adjust Thickness
''''''''''''''''
The Adjust Thickness command allows to modify the thickness of all the lines of the layer or of those selected. If no line is selected the command acts on the whole level, otherwise it works on selected lines.

.. tip:: **To adjust the thickness of the lines:**

    1. Select the images or the level frames to adjust in the .

    2. Choose Level  →  Adjust Thickness.

    3. Choose a mode. The modes are: Scale Thickness that scale lines up or down using a percentage value, Add Thickness that add an amount of thickness to the lines using the current unit, Costant Thickness that apply a thickness value, ignoring its variations, using the current unit.

    4. Sets a starting and an ending value.

    5. Press the Apply button.

.. _color_fade:

Color Fade
''''''''''
In case it is needed to adjust the drawing colors it is possible to fade the drawings toward a color defined by Red, Green, Blue and Alpha values. The Intensity, expressed as a percentage, ranges from 0 to 100.The original color will fade to the color you set according with the Intensity parameter. This is available only for raster levels.

.. tip:: **To fade drawing colors:**

    1. Select the images or the level frames to fade in the .

    2. Choose Level  →  Color Fade.

    3. In the dialog that opens set the color you want to fade the selection to by doing one of the following:

    - Set the Red, Green and Blue values.

    - Click the color thumbnail and use the Style Editor to edit it (see  :ref:`Editing Styles <editing_styles>`  ).

    - Move the Intensity slider to set the value.

    4. Click the Apply button.

.. _binarize:

Binarize
''''''''
Allows you to process colored raster lines images recognizing basic colors (red, green, blue, cyan, magenta and yellow) plus black. The process produce an uniform background color, eliminating shadows and dirty pixels.

The colored lines are identified and all the pixels belonging to each line are changed to the maximum value of the identified color. The anti-aliasing is removed.

The use o f this command is useful to pre-process scanned images simplifying the Cleanup process.

The preview is available to check the result. The alpha toggle allows to produce images with a transparent background.

.. tip:: **To binarize images:**

    1. Select the images or the level frames to process in the .

    2. Choose Level  →  Binarize.

    3. Activate the Preview toggle to check the result.

    4. Activate the Alpha toggle if you need transparent background.

    5. Click the Apply button.

.. _saving_levels:

Saving Levels
-------------
All the editing performed in the level strip is not saved until you save the level. You can also automatically save all of the editing done on any level of the  by saving the scene (see  :ref:`Saving and Loading Scenes <saving_and_loading_scenes>`  ). 

When saving an animation level it is possible to automatically create a backup file of the previous version by setting the Backup Animation Levels when Saving option in the Preferences  →  General dialog. The backup version is created in the same location where the level is saved, and has an _backup suffix.

.. note:: An asterisk after the level name in the level strip title bar denotes that there are unsaved changes for the current level.

.. tip:: **To save the current level:**

    Do one of the following:

    - Choose File  →  Save Level.

    - Right-click in the scene cast and choose Save Level from the menu that opens.

.. tip:: **To save the current level with a different name in a different location:**

    1. Choose File  →  Save Level As.

    2. In the browser that opens select for the level you want to save a location and name, and click the Save button.

.. note:: The Save Level As command creates a copy of the level with a different file name and location, but does not change the name and location of the level used in the scene.

.. _exporting_levels:

Exporting Levels
----------------
Animation levels created with OpenToonz can be exported in a variety of image file formats in order to be used in third-party software. The levels are exported as a sequence of files named with a progressive four-digits number written between the file name and the file extension, e.g. ``animation.0001.tif`` , ``animation.0002.tif`` , etc.or a single file for the .TLV format. File formats available are BMP, JPG, PNG, TGA ,TIF and TLV (the .TLV format is available only to export vector levels (.PLI); the format options can be set for each format in the Output Settings dialog (see  :ref:`Choosing the Output Settings <choosing_the_output_settings>`  ).

When exporting vector levels, the size and resolution of the exported sequence can be defined in the Export Level dialog. The default size and resolution are those defined in the camera settings, and the preview of the resulting image is visible in the preview area of the Export Options page to understand how the exported images will be cropped (see  :ref:`Defining Camera Settings <defining_camera_settings>`  ). The size of the exported image can be changed entering a scale value in the Scale field.

.. note:: Any trucking, resizing and animation of the camera is not considered when exporting vector levels.

The Retas Compliant option name the exported sequence with a a progressive four-digits number suffix before the file extension, e.g. ``animation0001.tga`` , ``animation0002.tga`` , etc and sets the exporting format to TGA.

Background Color allows to set the RGBA values of the background color.

The No Antialias option allow to remove the antialias from the exported sequence.

.. tip:: **To export the current level:**

    1. Choose File  →  Export Level.

    2. In the File Browser page select the level you want to save, a location and a name.

    3. Do one of the following:

    - Choose the file format you want the exported level to have.

    - Activate the Retas Compliant option to export the level in the same format and with the same options that the Retas software uses when exporting painted drawings.

    - In the Export Options, sets the RGBA values for the background color.

    - Activate the No Antialias option to remove the anitialias from the exported levels sequence images.

    4. If you are exporting a Toonz Vector Level:

    - Set the Output Size in the Vectors Export Box fields

    - Set a Start and End percentage value for the line thickness

    5. Click the Export button.

.. note:: The Export Level command creates a new version of the level with a different file name, location and format, but does not change the name, location and format of the level used in the scene.

.. tip:: **To set the file format options:**

    1. Choose File  →  Output Settings.

    2. Set the options for the format you want to use for exporting levels.

