.. _setting_up_a_scene:

Setting Up a Scene
==================

.. _scene_settings_and_project_default_settings:

Scene Settings and Project Default Settings
-------------------------------------------
When you start working on a scene, automatically it will belong to the current project, inheriting its settings and default folders. In this way all the scenes belonging to a project are created with the same settings, assuring the consistency of the production (see  :ref:`Managing Projects <managing_projects>`  ). 

Settings concern different tasks you may perform in OpenToonz, such as the scanning, or cleanup process, the camera size and resolution, the frame rate, the output options, etc. They can be accessed in dialogs you can open with commands available in the related menu; for example the scan and cleanup settings commands are available in the Scan & Cleanup menu.

Settings for a particular scene can always be changed independently from the other ones, and will be automatically saved when the scene is saved. 

If you want to change the default values you can save current scene settings as default, so that all new scenes created for that project will have those values.

.. tip:: **To save current scene settings as project default settings:**

    Select File  →  Project Management  →  **Save Default Settings**: all the settings from the current scene will become the project default.


.. _choosing_the_working_unit:

Choosing the Working Unit
-------------------------
Positions, distances and sizes can be expressed in several units of measure: inches, millimeters, centimeters, fields and pixels. 

The field unit is equal to 1/2 inch on the horizontal dimension, and it depends on the A/R set in the field guide information of the Scene Settings... dialog on the vertical dimension (see  :ref:`Using the Viewer <using_the_work_area>`  ). For example if the A/R value is 1.77778, two horizontal fields are equal to an inch, while one vertical field equals to an inch divided by 1.77778.

In the Files  →  Preferences...  →  Interface dialog you can set the following default units:

- The **Unit** is used to display all measures in text fields, and applied when moving or changing the size of stage objects.

- The **Camera Unit** is used to display and define the camera size in the Xsheet  →  Camera Settings... dialog (see  :ref:`Defining Camera Settings <defining_camera_settings>`  ).

You can also express values in an unit different from the default one by entering any of the following units and abbreviations: in, inch, " , ' ' (two apostrophes), cm, mm, fld, field and px, after the input value itself. As soon as the value is entered it's converted in the default unit.

If a value without a specific unit is used, it is supposed to be expressed in the default unit.

.. tip:: **To set the default working units:**

    1. Choose File  →  Preferences...  →  Interface.

    2. Do one of the following:

    - In the **Unit** option menu choose the unit you want to use as default.

    - In the **Camera Unit** option menu choose the unit you want to use to express the camera size.


.. _setting_the_frame_rate:

Setting the Frame Rate
----------------------
|scene_settings|

The frame rate is the number of frames per second of animation, and has to be set according to the type of output you have to render, for instance it should usually be 24 for cinematic production, 25 for PAL output, or 30 for NTSC.

The current scene frame rate can be set in the Scene Settings... dialog, and it is displayed in the bottom bar of any Viewer pane. In case the play back is activated, the actual frame rate is displayed on its left.

Apart from affecting the playback speed when previewing or rendering a scene, the frame rate also determines the frame count of an audio file when it is imported into the Xsheet (see  :ref:`Creating a Soundtrack <creating_a_soundtrack>`  ).

Even if a scene has been composited with a specific frame rate for a certain output, it is possible to render it out at a different frame rate by using the Stretch from FPS: To: option in the Output Settings...  →  More Settings dialog section (see  :ref:`Choosing the Output Settings <choosing_the_output_settings>`  ).

|stretch_fps_to|


.. tip:: **To set the frame rate:**

    1. Choose Xsheet  →  Scene Settings...  →  More.

    2. In the Frame Rate text field set the frame rate value.


.. _defining_camera_settings:

Defining Camera Settings
------------------------
|camera_settings|

The Current Camera Settings dialog, that can be opened from the Xsheet menu, contains parameters for defining the current camera frame size and resolution. 

More than one camera can be defined for each scene, in order to have different output resolutions, or to shot only a particular area of the scene (see  :ref:`Using the Stage Schematic <using_the_stage_schematic>`  ).

The camera frame size can be expressed in any unit, but will be visualized in the default one chosen in the Preferences...  →  Interface dialog (see  :ref:`Choosing the Working Unit <choosing_the_working_unit>`  ). 

In OpenToonz the Camera is defined by different parameters:

    - X (Width) and Y (Height) frame size of the camera, expressed in the default Camera Unit (usually inches).

    - **A/R** is the aspect ratio value resulting by dividing Width/Height.

    - X and Y resolution **Pixels** of the resulting image frame seen by the camera.

    - X and Y **DPI** values, calculated using the standard formulas: XDpi=XPx/Width, and YDpi=YPx/Height. This two fields can be forced to have the same value, by activating the equal-sign button between them.

When inserting a value in one field, the others change accordingly as needed for having a consistent camera. You can decide which set of values has to be considered fixed by OpenToonz. The lock-shaped buttons and the radio buttons at the leftmost column of the camera parameters, let you select which column and row of values has to be preserved by OpenToonz, while changing the others as needed.

The **Use Current Level Settings** button let you set the camera for framing exactly the content of the selected level. Just press this button and OpenToonz will calculate the appropriate values for the camera.

Camera resolutions can also be selected from a list of predefined camera settings. You can add any camera preset you define to the list, as well as remove any predefined camera from it.

.. note:: The predefined cameras list is saved in the file ``reslist.txt``  stored in the projectroot (see  :ref:`Setting the Projectroot <setting_the_projectroot>`  ).

.. tip:: **To add a preset camera resolution:**

    1. Set the resolution and A/R for the camera you want to save.

    2. Click the **Add** button on the right of the preset cameras list.

    3. Assign a name to the camera resolution and click the **OK** button.

.. tip:: **To remove a preset camera resolution:**

    1. Select the camera resolution you want to remove in the preset cameras list.

    2. Click the **Remove** button on the right of the preset cameras list.


.. _color_calibration_using_lookup_tables:

Color Calibration using Look-up Tables
--------------------------------------

|3dlut|

OpenToonz can manage the previsualization of color through the use of 3D Look-up Tables. By applying a 3D LUT file, properly configured for the current display monitor, it will be possible to work on different color spaces, such as `Rec. 709 <https://en.wikipedia.org/wiki/Rec._709>`_, `DCI-P3 <https://en.wikipedia.org/wiki/DCI-P3>`_ or `Rec. 2020 <https://en.wikipedia.org/wiki/Rec._2020>`_.

Once a 3DLUT is active, all colors displayed on Viewer, Combo Viewer, Flipbook, Color Model, Palette, and Style Editor will be corrected.

.. note:: Currently, only the .3dl file format is supported. It must follow specification written `here <http://download.autodesk.com/us/systemdocs/help/2009/lustre_ext1/index.html?url=WSc4e151a45a3b785a24c3d9a411df9298473-7ffd.htm,topicNumber=d0e8061>`_.

.. note:: Currently, only the Windows version of OpenToonz can detect the currently connected monitor. For other platforms only one 3D LUT file can be applied for any type of monitors. (Even on Windows, connecting multiple different monitors at the same time is not supported for now. It will only identify the first registered monitor).

.. note:: PLEASE NOTE: At the moment, using Plastic deformation together with this feature causes a display issue such that the deformed image is not shown in *Camera Stand* mode of the Viewer.

.. tip:: **To apply a 3DLUT file for previsualizing color:**

    1. Choose File  →  Preferences...  →  Interface.

    2. Activate the **Color Calibration using 3D Look-up Table** option.

    3. In the **3DLUT File for [monitor]:** option, press the file browser button to navigate and select the desired .3DL file.

    4. Restart OpenToonz for the changes to take effect.


.. _assigning_memory_for_the_undo_operations:

Assigning Memory for the Undo Operations
----------------------------------------
All the operations performed in the software can be undone by using the Edit  →  Undo command, even to go back for several steps. 

Undo operations require computer memory in order to be performed, and some of them may require more memory than some others, according to their complexity. 

To prevent most of the computer memory to be used by undo operations while you work, a situation that slows down the software performance, it is possible to set a limit for it by specifying the Undo Memory Size (MB) in the Files  →  Preferences...  →  General dialog. 

As soon as the limit is reached, the oldest undo operations will be discarded to make room for the new ones.


.. _optimizing_the_memory_usage:

Optimizing the Memory Usage
---------------------------
When working with Raster images, predominantly being animation levels scanned with OpenToonz or GTS, an extensive usage of computer memory may be required during the cleanup, painting and rendering processes.

After a certain amount of time the computer performance may worsen, as the memory gets fragmented because of the several writing and reading accesses. To prevent this behavior, the Minimize Raster Memory Fragmentation* option can be activated in the Files  →  Preferences...  →  General dialog. When activated, a section of computer memory is reserved and used only for operations concerning Raster images.

If you are working mainly with vector images, that have been drawn inside OpenToonz, this option should be deactivated, as the reserved memory section would be otherwise unused by the computer.

.. note:: The change set for this option is valid only after OpenToonz is restarted.


.. |scene_settings| image:: /_static/setting_up_a_scene/scene_settings.png
.. |camera_settings| image:: /_static/setting_up_a_scene/camera_settings.png
.. |stretch_fps_to| image:: /_static/setting_up_a_scene/stretch_fps_to.png
.. |3dlut| image:: /_static/setting_up_a_scene/3dlut.png

.. |scene_settings_es| image:: /_static/setting_up_a_scene/es/scene_settings.png
.. |camera_settings_es| image:: /_static/setting_up_a_scene/es/camera_settings.png
.. |stretch_fps_to_es| image:: /_static/setting_up_a_scene/es/stretch_fps_to.png
