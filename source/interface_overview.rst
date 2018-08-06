.. _interface_overview:

Interface Overview
==================

|UI_1|

OpenToonz interface is organized into rooms, also known as workspaces: each room is a different collection of windows which are laid out at specific positions on the screen. 


.. _using_rooms:

Using Rooms
-----------
Available rooms are listed on the far right of the menu bar. Each of them always displays the content of the current scene.

Rooms can be named and their order can be rearranged. New rooms can be added and existing rooms can be deleted. When a room is added it is empty; to configure it, panes can be added one by one (see below).


.. tip:: **To enter a room:**

    Click the related tab on the far right of the menu bar.

.. tip:: **To name a room:**

    Double-click the tab and type the name you want to assign to the room.

.. tip:: **To order room tabs:**

    Click and drag the tab to the new position.

.. tip:: **To add a new room:**

    Right-click in the room tab area and choose New Room from the menu that opens.

.. tip:: **To delete a room:**

    Right-click the room tab and choose Delete Room "<Name>" from the menu that opens. The current room cannot be deleted.

.. tip:: **To return to the set of rooms provided with Toonz:**

    Choose Windows > Reset to Default Rooms.


.. _customizing_rooms:

Customizing Rooms
'''''''''''''''''
Rooms can be modified by setting different sizes to different panes, and adding or removing panes. To prevent the accidental addition or removal of panes, rooms configuration can be locked.

Most of the panes can be maximized to fill the full interface, and can be added as floating windows by using the Windows menu.


.. tip:: **To resize a pane in the room:**

    Click any vertical or horizontal separator and drag it to the new position.

.. note:: Some panes like the toolbar and the level strip have some fixed size, therefore they cannot be resized.

.. tip:: **To open a pane as a floating window:**

    Select in the Windows menu the pane you want to open.

.. tip:: **To resize a floating window:**

    Click and drag the border or corner of a window.

.. tip:: **To close a floating window or a dialog:**

    Click the close button at the right of the title bar.

.. tip:: **To add a pane to a room:**

    1. Use the Windows menu to open the pane as a floating window.

    2. Click and drag its title bar to move it around and release to dock it according to the highlighted insertion point.

.. note:: Trying to dock a pane to the leftmost/rightmost part of the interface may fail if the main OpenToonz window is maximized at that moment. To overcome this, you can restore the main window size, dock the desired pane, and then maximize it back.

.. tip:: **To remove a pane from a room:**

    1. Click and drag the title bar of the pane you want to remove to undock it from the room.

    2. Close the floating window.

.. tip:: **To maximize, or minimize a maximized pane:**

    Double-click its title bar.

.. note:: Some panes like the toolbar and the level strip have some fixed size, therefore they cannot be maximized. 

.. tip:: **To lock/unlock the rooms configuration:**

    Activate/deactivate the Windows > Lock Room Panes option.


.. _room_panes:

Room Panes
----------
Below there is a list of the panes that can be used to build rooms and that can be opened as floating windows.


.. _batch_servers:

Batch Servers
'''''''''''''
The Batch Servers window allows you to process the batch list by using the render farm, and contains information about the list of server (rendering) nodes defined for the farm. 

See  :ref:`Monitoring the Server Nodes <monitoring_the_server_nodes>`  .


.. _color_model:

Color Model
'''''''''''
The color model viewer displays the image, or animation level, you loaded as reference to paint the current animation level.

See  :ref:`Using a Color Model <using_a_color_model>`  .


.. _file_browser:

File Browser
''''''''''''
The file browser allows you to load and save files, and to access projects.

On the left there is a file tree with some main folders containing material stored on your computer: My Computer, Network, My Documents, History, Library and Projects. You can open folders and sub-folders in order to retrieve files that are displayed in the area on the right.

See  :ref:`Managing Projects <managing_projects>`  and  :ref:`Using the File Browser <using_the_file_browser>`  .


.. _flipbook:

Flipbook
''''''''
The flipbook can display animation levels, clips or sequences of images. It can be used to check levels for instance before loading them, or to control a rendered sequence. 

See  :ref:`Using the Flipbook <using_the_flipbook>`  .


.. _function_editor:

Function Editor
'''''''''''''''
The function editor maps objects and FX transformations with key values and related interpolations by using a spreadsheet or a graph editor. It is divided into two sections: on the left there is an area where the spreadsheet or graph editor is displayed, on the right top is an area where the interpolation of the current transformation segment is displayed, and on the right bottom is the objects/FX tree.

See  :ref:`Using the Function Editor <using_the_function_editor>`  .


.. _level_strip:

Level Strip
'''''''''''
The level strip displays the sequence of drawings belonging to the level currently selected in the xsheet. 

It helps you to edit the sequence of drawings and to see all the drawings of the current level, even if those drawings are not exposed in a xsheet. 

See  :ref:`Editing Animation Levels <editing_animation_levels>`  .


.. _message_center:

Message Center
''''''''''''''
The message center displays in a list the messages OpenToonz is sending to the user. You can set filters on the messages showed in the window using the appropriate radio buttons, or you can clear completely the list pressing the Clear button.


.. _palette:

Palette
'''''''
It displays the styles defined for the current level, or in case it is inactive the styles defined for a previously selected level.

See  :ref:`The Palette Window <the_palette_window>`  .


.. _scene_cast:

Scene Cast
''''''''''
The scene cast pane lets you control the files loaded in the scene, save them and load new ones. It can be organized in folders and sub-folders. 

See  :ref:`Using the Scene Cast <using_the_scene_cast>`  .


.. _schematic:

Schematic
'''''''''
The schematic can alternatively display stage information or special FX usage.

The stage schematic displays as nodes all the objects defined in a scene, i.e. columns, pegbars, cameras, the table and motion paths, and allows you to manage the way they are linked to each other.

The FX schematic allows you to apply FX to the content of xsheet columns, and to manage the way they are applied. All the columns and FX are displayed as nodes that can be connected in order to set the way FX affect the scene content. 

See  :ref:`Using the Stage Schematic <using_the_stage_schematic>`  and  :ref:`Using the FX Schematic <using_the_fx_schematic>`  .


.. _style_editor:

Style Editor
''''''''''''
The style editor allows you to modify the palette styles. You can choose the type of style among color, texture, vector and raster. There also is a settings tab where you can decide some parameters for the style.

See  :ref:`Editing Styles <editing_styles>`  .


.. _studio_palette:

Studio Palette
''''''''''''''
The studio palette allows you to store an unlimited number of level palettes. From here any palette can be retrieved and assigned to the current level in order to paint it, with no need to define the same styles again and again. It also includes a viewer displaying the styles of the currently selected palette.

See  :ref:`Using the Studio Palette <using_the_studio_palette>`  .


.. _tasks:

Tasks
'''''
The Tasks window contains the task tree with all the tasks submitted to the batch processing, and information about the task currently selected in the tree. From the task tree you can start or stop a task execution, or remove it.

See  :ref:`Managing and Executing Render Tasks <managing_and_executing_render_tasks>`  .


.. _toolbar:

Toolbar
'''''''
The toolbar contains tools to draw, select and edit drawings, and to animate objects like the camera, columns and pegbars. The tools in the toolbar can only be used in the main viewer. 

.. note:: If the toolbar is too short to display all the tools, it can be scrolled by using arrow buttons available at its ends.

**Animate**  modifies the position, rotation and size of the current objects (see  :ref:`Animating Objects <animating_objects>`  ).




**Selection**  performs a selection and transforms it (see  :ref:`Using the Selection Tool <using_the_selection_tool>`  ).




**Brush**  draws in the work area in freehand mode (see  :ref:`Drawing with the Brush Tool <drawing_with_the_brush_tool>`  ).




**Geometric**  draws geometric shapes (see  :ref:`Drawing with the Geometric Tool <drawing_with_the_geometric_tool>`  ).




**Type**  adds text by setting the font and size (see  :ref:`Adding Text <adding_text>`  ).




**Fill**  fills drawing areas with the current style (see  :ref:`Filling Areas <filling_areas>`  ).




**Paint Brush**  paints lines and areas in Toonz raster drawings in freehand mode. (see  :ref:`Filling Areas <filling_areas>`  ).




**Eraser**  deletes vectors in vector drawings, and painted areas and lines in raster drawings (see  :ref:`Drawing Tools <drawing_tools>`  ).




**Tape**  joins two open ends of one or two vectors in vector drawings, or closes gaps in raster drawings (see  :ref:`Joining and Splitting <joining_and_splitting>`  ).




**Style Picker**  picks a style from the current drawing, that becomes the current style in the palette and in the style editor.




**RGB Picker**  picks red, green and blue values from the viewer content, and applies them to the current style (see  :ref:`Plain Colors <plain_colors>`  ).




**Control Point Editor**  modifies the vector shape by editing its control points (see  :ref:`Editing Vector Control Points <editing_vector_control_points>`  ).




**Pinch**  modifies the vector shape by clicking and dragging anywhere on the vector (see  :ref:`Changing the Bend of Vectors <changing_the_bend_of_vectors>`  ).




**Pump**  locally modifies the vector thickness by clicking on the section you want to affect and then dragging up or down (see  :ref:`Using Other Modifier Tools <using_other_modifier_tools>`  ).




**Magnet**  deforms several vectors at once by clicking the area you want to affect and dragging (see  :ref:`Using Other Modifier Tools <using_other_modifier_tools>`  ).




**Bender**  bends vectors in vector drawings (see  :ref:`Using Other Modifier Tools <using_other_modifier_tools>`  ).




**Iron**  removes creases from vectors by moving the cursor on the vector you want to flatten (see  :ref:`Using Other Modifier Tools <using_other_modifier_tools>`  ).




**Cutter**  splits a vector in two sections when clicking on it (see  :ref:`Joining and Splitting <joining_and_splitting>`  ).




**Skeleton**  defines character models, and animates them as in cutout animation (see  :ref:`Using the Skeleton Tool <using_the_skeleton_tool>`  )




**Hook**  defines reference points to be used in the stage schematic to move an object, or link one object to another (see  :ref:`Using Hooks <using_hooks>`  ).




**Tracker**  tracks specific regions in a sequence of images (see  :ref:`Tracking Points <tracking_points>`  ).




**Plastic**  builds a mesh that allows to deform and animate a character or part of it (see  :ref:`Using Plastic tool <using_plastic_tool>`  ).




**Zoom** zooms in and out the viewer content; after you click you can drag up to zoom in the work area, or drag down to zoom out.




**Hand**  pans over the viewer content; if the 3D view is activated, the Hand tool lets you pan over the 3D view as well.




**Rotate**  rotates the viewer content; if the 3D view is activated, the Rotate tool lets you change the point of view.


.. _tool_options_bar:

Tool Options Bar
''''''''''''''''
The tool options bar displays settings for the current tool, if it has any.

For example it lets you set the thickness and other properties of the Brush tool.

.. note:: If the tool options bar is too short to display all the tool options, it can be scrolled by using arrow buttons available at its ends.


.. _viewer:

Viewer
''''''
The viewer is the work area where you can draw images and see at the same time the result of your compositing. It is endless and you can scroll, zoom in, zoom out and rotate it the way you prefer.

It has different modes of visualization among which you can choose the more suitable to the operation you are performing.

See  :ref:`Using the Viewer <using_the_work_area>`  and  :ref:`Previewing the Animation <previewing_the_animation>`  .


.. _xsheet:

Xsheet
''''''
The xsheet allows you to manage the scene content, in the same manner as the timeline. It is organized in columns, and columns are divided into cells, representing the content of that column in that particular frame. In the columns you can load animation levels, clips, images, audio files or other xsheets. 

Each column has its own header containing information about its content. The column on the far left displays the frame number, with a cursor placed on the current frame. The headers area and the frame column are always visible, even when scrolling the xsheet area; in this way it's easier to understand how the scene is built.

Frames are rendered reading images from left to right in each cell row.

See  :ref:`Working in Xsheet <working_in_xsheet>`  .


.. _timeline:

Timeline
''''''''
The timeline allows you to manage the scene content, in the same manner as the xsheet. It is organized in horizontal layers, and layers are divided into cells, representing the content of that layer in that particular frame. In the layers you can load animation levels, clips, images, audio files or other timelines. 

At the leftmost part each layer has its own header containing information about its content. At the top part of the timeline there is a time ruler that displays the frame number, with a cursor placed on the current frame. The headers area and the time ruler are always visible, even when scrolling the timeline area; in this way it's easier to understand how the scene is built.

Frames are rendered reading images from bottom to top in each cell column.

See  :ref:`Working in Xsheet <working_in_xsheet>`  .


.. _customizing_the_interface_appearance:

Customizing the Interface Appearance
------------------------------------
The appearance of the OpenToonz interface can be customized to suit any production need by choosing a specific language and interface theme.

OpenToonz allows users to choose a specific language for the software interface, including menus, commands, tooltips, and on-screen messages. Currently available languages are: English, German, Spanish, French, Italian, Russian, Japanese and Chinese.

There are several included themes to choose from: Default, Blue, Dark and Light.

The interface themes are defined by means of a QSS file, whose concepts, terminology, and syntax are inspired by CSS files (HTML Cascading Style Sheets). The QSS files also refers to a set of PNG images that are used to create interface widgets. 

These files are stored in a folder named as the QSS file, and located in the ``C:\OpenToonz 1.x stuff\config\qss``  folder on Windows and ``OpenToonz 1.x stuff\config\qss``  folder on Macintosh. 

.. note:: The QSS file for Macintosh is named with the _mac suffix.

The QSS file can be edited with any text editor software, e.g. Notepad or TextEdit; the PNG images with any image editor software. Editing the QSS file requires some skill in CSS language, but some changes like colors of pane elements, can be easily done by expressing them with red, green and blue values.

.. note:: The QSS files defining the colors and the images used in the OpenToonz interface have to be written according to a specific syntax, otherwise OpenToonz interface will not be displayed properly. If you decide to edit a QSS file, make a backup copy first in case you need to revert the file to the original version.

.. tip:: **To choose the interface language:**

    1. Choose File > Preferences > Interface.

    2. In the Language* option menu choose the language you want to use in the interface.

    3. Restart OpenToonz to have the interface in the selected language.

.. tip:: **To choose the interface theme:**

    1. Choose File > Preferences > Interface.

    2. In the Theme option menu choose the style to be applied to the interface.

.. tip:: **To create a new theme:**

    1. Navigate to ``C:\OpenToonz 1.x stuff\config\qss``  folder on Windows and ``OpenToonz 1.x stuff\config\qss``  folder on Macintosh.

    2. Duplicate one of the already existing style folder.

    3. Rename the folder and the QSS files inside it with the name you want to assign to the style.

    4. Edit the QSS file and the PNG images contained in the new folder.

.. note:: The new style will be available in the Preferences dialog the next time you run OpenToonz.

.. tip:: **To edit style QSS file:**

    Open and edit with a text editor software (e.g. Notepad or TextEdit) the QSS files available in the style folder.

.. tip:: **To edit style images:**

    Open and edit with an image editor software the PNG files available in the style folder.

.. |UI_1| image:: /_static/UI_1.png
