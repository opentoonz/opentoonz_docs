.. _applying_special_fx:

Applying Special FX
===================
Special FX can be applied to animation levels, images and clips exposed in xsheet columns in the FX Schematic, where each element is represented as a node. 

The relationship between the contents of columns and FX can be managed by connecting or disconnecting links between nodes.

.. _using_the_fx_schematic:

Using the FX Schematic
----------------------
In the FX schematic all columns are displayed as nodes having an output port connected to the xsheet final node: this means that their content is part of the scene and is rendered as it is.




When FX are added, they are displayed as nodes as well, with ports to create links that let you set the way FX affect the scene contents. 

Column nodes have the camera stand (|camera_stand|) and the render (|preview|) toggles on the top right: these toggles are the same as the toggles available in the xsheet column headers (see :ref:`Working with Xsheet Columns <working_with_xsheet_columns>`  ). FX nodes have only the render toggle (|preview|) allowing you to include or exclude temporally the effect in the rendering.



Nodes can be easily selected and arranged. When selected, nodes are highlighted in white; the current node has its label in red.

It is also possible to group several nodes in one single node, in order to better manage the whole FX schematic. Groups can be opened to be examined and edited, and its components can be selected for further operations, like editing FX settings, or creating new groups.

.. tip:: **To access the FX schematic:**

    Click the schematic toggle button (|schematic|) in the bottom bar of the schematic window until the title bar displays FX Schematic.



.. tip:: **To navigate the FX schematic:**

    Do one of the following:

    - Use the mouse wheel, or the zoom shortcut keys (by default + and - keys) to zoom in and zoom out.

    - Middle-click and drag to scroll in any direction.

    - Use the Fit to Window button (|fit_to_window|) in the bottom bar of the schematic window to display all of the objects in the current window.



    - Use the Focus on Current button (|focus_on_current|) in the bottom bar of the schematic window to center the stage on the current object.

    - Use the Reset Size button (|reset|) in the bottom bar of the schematic window, or use the reset view shortcut (by default the 0 key) to display all of the objects at the default size.

.. tip:: **To name a node:**

    Ctrl + double-click the node name and type a new name.

.. tip:: **To minimize/maximize the column and FX nodes:**

    Do one of the following: 

    - Click the arrowhead next to the node name to minimize/maximize columns selectively.

    - Click the Minimize/Maximize (|minimize|/|maximize|) button in the bottom bar of the schematic window to minimize/maximize all the column nodes.



.. tip:: **To select nodes:**

    Do one of the following:

    - Click to select a node.

    - Click and drag to select a group of nodes.

    - Ctrl-click (PC) or Cmd-click (Mac) to add a node to, or remove it from the selection.

.. note:: Links can be selected together with nodes (see  :ref:`Editing the FX Schematic <editing_the_fx_schematic>`  ).

.. tip:: **To move the selection:**

    Click and drag any object of the selection.

.. tip:: **To group selected nodes:**

    Right-click any selected node and choose Group from the menu that opens.

.. tip:: **To open a group:**

    Right-click the group and choose Open Group from the menu that opens: the group nodes are displayed in a box, showing links between group nodes, and links with nodes outside of the group. 

.. note:: In the FX schematic, when the content of a group is displayed, it is possible to edit the links between group nodes, and links with nodes outside of the group.

.. tip:: **To close a group:**

    Click the close button on the right of the group box bar. 

.. tip:: **To release a group:**

    Right-click the group and choose Ungroup from the menu that opens.

.. tip:: **To include or exclude temporally an effect from the rendering:**

    Click the render toggle (|preview|) on the upper right corner of the effect node.



.. tip:: **To reorder nodes in the FX schematic:**

    Click the Reorder Nodes button (|reorder_nodes|) in the bottom bar of the schematic window.



.. _inserting_special_fx:

Inserting Special FX
''''''''''''''''''''
Special FX can be inserted or added in the schematic, or replace previously added FX nodes, either from and FX browser window, or from drop-down menus that open when right-clicking nodes or in the schematic area. Both are organized in folders/submenus containing sets of FX; if some presets are defined for an effect, an additional folder/submenu is available (see  :ref:`Creating Presets <creating_presets>`  ).

 |Toonz71_390| 

When inserting FX, they will be placed along the link that starts from the selected node output port; when adding FX, they will be placed at the end of a new link that will start from the selected node output port.

In case several nodes are selected, the effect will be added/inserted for each selected node, but all the added/inserted FX will be linked, and connected visually by a dashed line. This means that every time the effect is edited, all the linked nodes will be edited as well, unless you break the link to start editing them separately.

To apply FX globally it is possible to use the Xsheet node as a standard column node, representing the whole content of the scene.

Three different types of special FX can be used in the schematic, each with a different type of node:

- Basic FX, such as the Blur effect, that simply modify the contents of a column; they are displayed as a yellow node with an input port on the left, labelled Source, and an output port on the right. 

 |Toonz71_391| 

To affect a column, they have to be inserted in the link from the column to the xsheet, so that the column node is connected to the FX input port, and the FX node output port is connected to the xsheet node. 

If several FX are applied in a chain, they will be applied one after the other, following the order from the column to the xsheet node.

- Combined FX, such as the Matte In effect, that modify the column contents according to the contents other columns; they are displayed with a yellow node with two or more input ports on the left, and an output port on the right. 

To affect a column, they have to be inserted into the link from the column to the xsheet, so that the column node is connected to the first FX input port labelled Source, while the other columns are connected to the other input ports, whose labels depend on the effect; the FX node output port has to be connected to the xsheet node. 

 |Toonz71_392| 

For example in case of a Matte In effect, the column to be matted has to be linked to the Source input port, the matte column has to be linked to the Matte input port, and the output port has to be connected to the xsheet node.

- FX that create computer generated images, such as the Radial Gradient, that are exposed in xsheet columns and therefore are similar to columns; they are displayed with an orange node with only an output port on the right. These FX nodes have to be connected to the xsheet node to be rendered, or can be connected to other FX nodes.

 |Toonz71_393| 

.. tip:: **To open the FX browser:**

    Do one of the following:

    - Choose Xsheet > New FX.

    - Click the New FX button (|fx|) in the bottom bar of the schematic window.



.. tip:: **To insert an effect:**

    Do one of the following:

    - Select the nodes for which you want to insert a new effect, select the effect you want to insert in the FX browser and click the Insert button.

    - Select the nodes for which you want to insert a new effect, right-click any of them and choose Insert FX from the menu that opens, then select the effect you want to insert from the available submenus. 

    - Select the links where you want to insert a new effect, right-click any of them and choose Insert FX from the menu that opens, then select the effect you want to insert from the available submenus (see  :ref:`Editing the FX Schematic <editing_the_fx_schematic>`  ). 

.. tip:: **To add an effect:**

    1. Select the nodes for which you want to add a new effect at the end of a new link.

    2. Do one of the following:

    - Select the effect you want to add in the FX browser and click the Add button.

    - Right-click any of the selected nodes and choose Add FX from the menu that opens, then select the effect you want to add from the available submenus. 

.. tip:: **To replace an effect:**

    1. Select the FX nodes you want to replace with a new effect.

    2. Do one of the following:

    - Select the effect you want to add in the FX browser and click the Replace button.

    - Right-click any of the selected nodes and choose Replace FX from the menu that opens, then select the new effect from the available submenus. 

.. tip:: **To insert/add a global effect:**

    1. Select the Xsheet node.

    2. Do one of the following:

    - Select the effect you want to insert/add in the FX browser and click the Insert/Add button.

    - Right-click any of the selected nodes and choose Insert FX/Add FX from the menu that opens, then select the effect you want to a insert/add from the available submenus. 

.. tip:: **To name a node:**

    Double-click the node name and type a new name.

.. _editing_the_fx_schematic:

Editing the FX Schematic
''''''''''''''''''''''''
Links between nodes have to be considered like flows going from the column nodes to the Output node, via the Xsheet node. If along the way there is one or several effects, the column content will be consequently processed before becoming part of the output. 

From the nodes output port several links can start at the same time, thus allowing, for example, a column to be rendered as it is, and to be also used as a mask for another column. It is also possible to determine permanently whether columns will be rendered or not, by leaving or deleting the link to the Xsheet node.

By editing the links between nodes, or by creating new ones, you can control how column nodes will interact with each other and with special FX before being rendered. 

FX nodes and links can be selected in order to be cut, copied, pasted or deleted. When selected, nodes and links are highlighted in white; the current node has its label in red; when at least one object is selected, the related links are displayed in blue.

When pasting a copied/cut selection, several options are available:

- Use Paste to paste the copied/cut selection into the schematic

- Use Paste Insert to insert the pasted selection into the selected links.

- Use Paste Add to add the pasted selection from the selected nodes at the end of new links. 

- Use Paste Replace to replace selected FX nodes with the pasted selection.

.. note:: Links have to be selected together with nodes when copying/cutting a selection if you want to preserve the links among them when pasting.

.. tip:: **To create links between nodes:**

    Click and drag the output port of the node to the input port of the FX node.

.. tip:: **To select nodes and links:**

    Do one of the following:

    - Click to select a node or a link.

    - Click and drag to select a group of nodes and links.

    - Ctrl-click (PC) or Cmd-click (Mac) to add a node or a link to, or remove it from the selection.

.. tip:: **To delete links between nodes:**

    Select the links you want to delete and do one of the following:

    - Choose Edit > Delete.

    - Right-click any selected link and choose Delete from the menu that opens.

.. tip:: **To connect a node to the Xsheet node:**

    Do one of the following:

    - Click and drag the output port of the node to the input port of the Xsheet node. 

    - Right-click the node you want to connect to the Xsheet node, and choose Connect to Xsheet from the menu that opens.

.. tip:: **To disconnect a flow from the Xsheet node:**

    Do one of the following:

    - Delete the link from the node to the Xsheet node.

    - Right-click the node you want to disconnect from the Xsheet node, and choose Disconnect from Xsheet from the menu that opens.

.. tip:: **To insert an FX node into a link:**

    Alt-click and drag it onto the link.

.. tip:: **To extract an FX node from a link:**

    Alt-click and drag it away from the link.

.. tip:: **To edit an FX nodes selection:**

    Do one of the following:

    - Use the Copy command to keep the selection in memory for further operations.

    - Use the Cut command to eliminate the selection from the schematic and keep it in memory for further operations.

    - Use the Paste command to paste the selection kept in memory in the FX schematic. 

    - Right-click a link and use the Paste Insert command to insert the selection kept in memory into the selected link. 

    - Right-click any node and use the Paste Add command to add the selection kept in memory from the selected nodes at the end of the new links. 

    - Right-click an FX node and use the Paste Replace command to replace the selected FX nodes with the selection kept in memory. 

    - Use the Delete command to delete the selection.

.. note:: All these commands are available in the menu that opens when right-clicking nodes and links. 

.. tip:: **To create a linked effect:**

    1. Select the FX nodes you want to duplicate.

    2. Right-click any of the selected nodes and choose Create Linked FX from the menu that opens.

.. tip:: **To break linked effects:**

    1. Select the FX nodes you want to unlink.

    2. Right-click any of the selected nodes and choose Unlink from the menu that opens.

.. _using_multiple_output_nodes:

Using Multiple Output Nodes
'''''''''''''''''''''''''''
In the FX schematic by default the Xsheet node is connected to an Output node: this means that all the nodes connected to the Xsheet node will be rendered both in the preview and in the final rendering.

The scene rendering can be limited to a specific node of the schematic by creating additional output nodes, connected to the node where you want to limit the rendering. 

When more than one output node is defined, you can set which is the active one, that will be considered for previewing or rendering the scene; the active output node is displayed in blue, while the others in grey. 

.. tip:: **To limit the output to a specific node:**

    1. Select the node to which you want to limit the output.

    2. Do one of the following:

    - Click the New Output button (|output|) in the bottom bar of the schematic window.

    - Right-click the node and choose New Output from the menu that opens.

.. tip:: **To add an Output node:**

    Do one of the following:

    - Click the New Output button (|output|) in the bottom bar of the schematic window.



    - Right-click in the stage and choose New Output from the menu that opens.

.. tip:: **To connect a node to an Output node:**

    Click and drag the output port of the node to the input port of the Output node.

.. tip:: **To set the current Output node:**

    Right-click the output you want to set as current and choose Activate from the menu that opens.

.. tip:: **To remove an Output node:**

    1. Do one of the following:

    - Select it and choose Edit > Delete.

    - Right-click it and choose Delete from the menu that opens.

.. note:: The last Output node remaining cannot be removed from the stage.

.. _editing_fx_settings:

Editing FX Settings
-------------------
FX parameters and their animation can be controlled in the FX Settings window. According to the selected effect, it displays a different layout of sliders, check boxes, text fields, etc. At the bottom of the window a preview area is available to check the result of the applied effect: you can activate or deactivate it, navigate its content, set its size, its background color, and limit it to the camera shot.

Parameters can be animated by setting key values at specific frames. A Set Key button (|key|) is available in the bottom bar of the window to set key values for all of the parameters. For all of the parameters that can be animated there is also a specific set key button, a small square located on the far right of each parameter, in order to set key values for each parameter independently. 



The Set Key button (|key|) may have the following colors:



    - It is grey when no key values for any parameter is defined at the current frame.

    - It is blue-striped when key values are defined at least for one parameter.

    - It is blue when key values are defined for all the parameters.

The parameter specific set key button may have the following colors:

    - It is grey if no key value is defined for the parameter at the current frame.

    - It is black when a key value is defined for the parameter at the current frame.

    - It is outlined in black if the parameter is animated but no key value is defined at the current frame.

    - It is outlined in red if you change the parameter value and the current frame does not have a key for the parameter.

Frames and key values can be navigated by using the related buttons in the bottom bar of the window. The Next (|next_key|) and Previous Key buttons (|prevkey|) are available only if more than one key value is defined.  |Toonz71_401| 

If no key values are defined, parameters you set will be used throughout the scene.

.. tip:: **To open the FX Settings window:**

    Do one of the following:

    - Right-click the effect node, and choose Edit FX from the menu that opens.

    - Double-click the effect node.

.. tip:: **To define values for the effect:**

    Use the available sliders, check boxes, text fields, etc., to configure the effect the way you prefer.

.. tip:: **To set the current frame:**

    Do one of the following:

    - Type the frame number or use the Next and Previous Frame buttons available in the bottom bar of the window.

    - Move the current frame cursor in the xsheet or in the function editor.

    - Use the frame bar or the playback buttons in the bottom bar of the work area.

.. tip:: **To set key values for all the effect parameters at the current frame:**

    1. Do one of the following:

    - If the current frame is not a key, click the Set Key button (|key|) in the bottom bar of the window: it turns from grey to blue and current values become key values for all the parameters at the current frame. 

    - If the current frame is a key for some parameters only, click the Set Key button (|key|): it turns from blue striped to blue and current values become key values for all the parameters at the current frame. 

    2. Define the values for the parameters.

.. tip:: **To set key values for a specific parameter at the current frame:**

    1. If the current frame does not have a key for the parameter, click the squared set key button on the far right of the parameter: it turns from grey to black, and the current value becomes a key value for the parameter at the current frame.

    2. Define the value for the parameter.

.. note:: If the current frame is not a key for the parameter, the squared set key button on the far right of the parameter turns red. Click it to set the key.

.. tip:: **To remove all key values for the effect parameters at the current frame:**

    Do one of the following:

    - If the key values are set for all the parameters, click the Set Key button (|key|) in the bottom bar of the window: it turns from blue to grey.

    - If the key values are set for some parameters only, click twice the Set Key button (|key|) in the bottom bar of the window: with the first click it turns from blue-striped to blue as you set keys for all the parameters; with the second click, it turns from blue to grey.

.. tip:: **To remove a key value for a specific parameter at the current frame:**

    Click the squared set key button on the far right of the parameter: it turns from black to grey.

.. tip:: **To navigate frames where key values are defined:**

    Use the Next (|next_key|) and Previous Key buttons (|prevkey|) available at the side of the Set Key button.

.. tip:: **To activate/deactivate the preview area:**

    Do any of the following:

    - Click the Camera Preview button ( |Toonz71_408|) in the bottom bar of the FX settings window to limit the preview to the camera shot.



    - Click the Preview button (|preview|) in the bottom bar of the FX settings window to preview the results regardless of the camera shot.

.. tip:: **To resize the preview area:**

    Do any of the following:

    - Click and drag the horizontal separator. 

    - Click and drag the separator toward the window border to hide the preview area.

    - Click and drag the separator collapsed to the window border toward the window center to display again the preview area.

.. note:: The A/R of the preview area depends on the A/R of the current camera

.. tip:: **To change the background color of the preview area:**

    Use the buttons in the bottom bar of the FX settings window to choose a white (|preview_white|), black (|preview_black|) or transparent (|preview_checkbox|) background.



.. tip:: **To navigate the preview area:**

    Do one of the following:

    - Use the mouse wheel, or the zoom shortcut keys (by default + and - keys) to zoom in and zoom out.

    - Middle-click and drag to scroll in any direction.

    - Use the reset view shortcut (by default the 0 key) to display preview at its actual size.

.. _using_fx_gadgets:

Using FX Gadgets
''''''''''''''''
Some FX parameters related to positions or dimensions have some gadgets available in the work area in order to be set by using the camera box and the scene elements as a reference. For example the radial gradient effect has two circular gadgets that can be edited to set the inner size and the outer size of the gradient.




As soon as an effect node is selected in the schematic, the Animate tool becomes the current tool and the related effect gadgets, if available, are visualized. The Animate tool settings will refer to the column the effect is applied to, but in case the effect creates a computer generated image (e.g. a radial gradient or a light spot) the settings will refer to the effect column itself (see  :ref:`Animating Objects <animating_objects>`  ).

.. tip:: **To visualize FX gadgets in the work area:**

    Select the effect node in the FX schematic.

.. tip:: **To edit FX gadgets:**

    Click and drag the FX gadgets visible in the work area. As you roll over the gadget and the related handles, the cursor changes shape to indicate you are editing FX gadgets. 

.. note:: Some gadgets have a handle for reference; however any point along the gadget shape can be clicked and dragged.

.. _defining_colors_and_color_spectrums:

Defining Colors and Color Spectrums
'''''''''''''''''''''''''''''''''''
Some special FX may require the definition of a color, or a color spectrum.

Colors can be defined by editing the related Red, Green, Blue and Alpha values, or by using the Style Editor. 

 |Toonz71_414| 

Color spectrums, i.e. a series of colors defining a continuous gradient, can be defined by adding any color you need, and editing each color separately. The color in the spectrum can be moved to set the distance between two colors and the related gradient.

.. tip:: **To define a color:**

    Do one of the following:

    - Set the Red, Green, Blue and Alpha values.

    - Click the color thumbnail and use the Style Editor to edit it (see  :ref:`Plain Colors <plain_colors>`  ).

.. tip:: **To define a color of the spectrum:**

    Select the arrow below the spectrum identifying the color, and edit the related color.

.. tip:: **To add a color to the spectrum:**

    Click the spectrum where you want to add the new color.

.. tip:: **To move a color in the spectrum:**

    Click and drag the arrow identifying the color to a new position.

.. tip:: **To remove a color from the spectrum:**

    Click and drag down the arrow identifying the color.

.. _creating_presets:

Creating Presets
----------------
A particular configuration and animation of FX parameters can be saved as a preset to be available later on both in the FX Browser and drop-down menus that open when right-clicking nodes or in the schematic area.

When a preset for a particular effect is saved, in the FX Browser the effect icon turns into a folder containing the saved preset, with the folder icon still selectable to insert the effect with its default values; in the drop-down menus the effect has an additional drop down menu where the first item can be selected to insert the effect with its default values.

 |Toonz71_415| 

Presets are saved in the projectroot, in the ``fxs\preset`` folder. This allows the presets to be available on all the computers sharing the same Projectroot (see  :ref:`Setting the Projectroot <setting_the_projectroot>`  ).

Once a preset is applied there is no link between the saved preset and the applied preset: the applied preset can be edited without affecting the saved one.

.. note:: When you save a preset with a name already used, a confirmation dialog will open, asking you whether you want to overwrite the previously saved preset.

.. tip:: **To save a preset:**

    1. Right-click the effect node you want to save as a preset and choose Save As Preset from the menu that opens.

    2. Assign a name to the preset and click the Save button.

.. tip:: **To retrieve a saved preset:**

    Do any of the following:

    - Open the FX Browser and open the folder related to the effect for which you saved the preset.

    - In the right-click menus Insert FX, Add FX and Replace FX, choose the sub-menu related to the effect for which you saved the preset.

.. tip:: **To remove a preset from the FX browser:**

    Right-click the preset in the FX browser and choose Remove Preset from the menu that opens. 

.. _creating_macro_fx:

Creating Macro FX
-----------------
Special FX can be combined to create a macro effect that can be saved and retrieved when needed.

When a macro effect is defined, you can edit its settings either in the standard way with the FX settings window that contains a page for each effect combined to define the macro, or by opening it and editing one effect at a time.

A macro effect can be opened also to check how the FX nodes are connected, and can be exploded to dissolve it and put its FX nodes back in the schematic.

When saved, the macro effect will be available in the FX browser and in the drop-down menus that open when right-clicking nodes or in the schematic area, inside the Macro folder, at the bottom of the list.

.. tip:: **To create a macro effect:**

    1. Select the FX nodes you want to combine to create the macro effect.

    2. Right-click the selection and select Make Macro FX from the menu that opens.

.. tip:: **To open a macro effect:**

    Right-click the macro node and choose Open Macro FX from the menu that opens: the macro nodes are displayed in a box, with the right links to the rest of the schematic. 

.. note:: When the content of a macro is displayed it is not possible to edit the links between macro nodes, and links with nodes outside the macro.

.. tip:: **To close a macro effect:**

    Click the close button on the right of the macro box bar. 

.. tip:: **To release a macro effect:**

    Right-click the macro node and choose Explode Macro FX from the menu that opens.

.. tip:: **To edit a macro effect:**

    Do one of the following:

    - Right-click the macro node and choose Edit FX from the menu that opens.

    - Right-click the macro node and choose Open Macro FX from the menu that opens, then edit the macro FX nodes.

.. tip:: **To save a macro effect:**

    1. Right click the macro effect node you want to save and choose Save As Preset from the menu that opens.

    2. Assign a name to the macro effect and click the Save button.

.. tip:: **To remove a macro effect from the FX browser:**

    Right-click the macro effect in the FX browser and choose Remove Macro FX from the menu that opens. 

.. _special_fx_list:

Special FX List
---------------
.. _background:

Background
''''''''''
.. _checkerboard:

Checkerboard
~~~~~~~~~~~~
 |Toonz71_417| 

Creates in the selected column a layer with a checkerboard defined by two Colors, and a grid Size. 

.. note:: The grid size can also be set by using a square gadget with a handle in the work area (see  :ref:`Using FX Gadgets <using_fx_gadgets>`  ).

.. _color_card:

Color Card
~~~~~~~~~~
 |Toonz71_418| 

Creates in the selected column a layer of the set Color. It can be used, for example, as a background color or to create a colorize effect by applying it combined with a multiply effect.

.. _kaleido:

Kaleido
~~~~~~~
 |Toonz71_419| 

Repeats the Source generating a kaleidoscopic effect.

The center of the effect can be defined interactively, moving the small red cross widget in the preview area, or writing the desired values in the X and Y text fields.

The angle of reflection, and the number of iterations can be set in the appropriate input text fields (Angle and Count).

.. _tile:

Tile
~~~~
 |Toonz71_420| 

Repeats the Source content in order to define a larger image: the Tile mode forms a pattern that completely fills the camera shot, the Tile Horizontally repeats the source content horizontally; the Tile Vertically repeats the source content vertically.

The Mirror Horizontally and Mirror Vertically options repeat the tiles by flipping them respectively in the horizontal and vertical directions; If both the options are activated, tiles will be mirrored in both directions.

The Margin value sets the size of a margin around each tile, with positive values adding some space around the tiles, and negative values collapsing them.

.. _blur:

Blur
''''
Blur
~~~~
 |Toonz71_421| 

Softens the Source content, creating an out of focus effect, according to a specific Intensity.

.. _directional_blur:

Directional Blur
~~~~~~~~~~~~~~~~
 |Toonz71_422| 

Blurs the Source content according to a specific Intensity along a specific direction defined by the Angle. 

The Bidirectional option applies the blur also on the other side of the direction.

.. note:: The intensity and the angle can also be set by using an arrow gadget with a handle in the work area (see  :ref:`Using FX Gadgets <using_fx_gadgets>`  ).

.. note:: The directional blur does not depend on the movement and the speed of the column to which it is applied. 

.. _local_blur:

Local Blur
~~~~~~~~~~
 |Toonz71_423| 

Blurs the Source content according to the brightness value of the node content connected to the Reference input handle. The Intensity value amplifies uniformly the blur given by the Reference node content.

.. _motion_blur:

Motion Blur
~~~~~~~~~~~
Creates a motion-blur effect, according to the movement of the Source content in the previous and current frame. The movement has to be defined by an animated column, pegbar or table: the higher the speed, the more visible the effect.

If the movement is constant between consecutive frames, you can increase or decrease the Intensity to have a more or less visible effect. If there is no movement between the previous and the current frame, no motion blur will be visible even though you may have set a high Intensity.

.. note:: No result will be visible if the motion blur is applied to a column that always stands in the same position while the content is a level where the movement is drawn.

.. _radial_blur:

Radial Blur
~~~~~~~~~~~
 |Toonz71_424| 

Blurs along radial lines whose origin is the set Center, defined by horizontal (X) and vertical (Y) coordinates, starting from an unaffected inner area defined by the Radius. 

.. note:: The center and the radius can be also set by using a point and a circle gadget with a handle in the work area (see  :ref:`Using FX Gadgets <using_fx_gadgets>`  ); the center can be set in the FX Settings preview as well.

.. _spin_blur:

Spin Blur
~~~~~~~~~
 |Toonz71_425| 

Blurs along concentric circular lines as if the Source content turns around the set Center, defined by horizontal (X) and vertical (Y) coordinates, starting from an unaffected inner area defined by the Radius.

.. note:: The center and the radius can be also set by using a point and a circle gadget with a handle in the work area (see  :ref:`Using FX Gadgets <using_fx_gadgets>`  ); the center can be set in the FX Settings preview as well.

.. _distort:

Distort
'''''''
.. _free_distort:

Free Distort
~~~~~~~~~~~~
 |Toonz71_426| 

Distorts the Source content according to the position of four points, defined by horizontal (X) and vertical (Y) coordinates. For each point you can set the actual position and its origin, to determine which feature of the image will be distorted to the new position. 

The Mode option menu lets you set the way the distortion is applied: Bilinear distorts the images according to the four points end positions, and Perspective forces the distortion to fit a perspective projection plane.

To better set the origin position for each point, you can use the Deactivate option that lets you see the image without distortion.

.. note:: The position of the four points and their origins can be also set by using arrow gadgets with handles at the ends in the work area (see  :ref:`Using FX Gadgets <using_fx_gadgets>`  ) and in the FX Settings preview as well.

.. _linear_wave:

Linear Wave
~~~~~~~~~~~
 |Toonz71_427| 

Distorts the Source content creating a wave effect that uses an automatically generated displacement map image. The Quantity value sets the number of waves; the Period sets the distance between waves; the Cycle shifts distortion in the wave direction.

You can also add a Distortion Wave on the main linear waves: the Amplitude sets the intensity of the distortion; the Frequency sets the number of waves creating the distortion; the Phase shifts the distorting waves.

A rotation for the whole wave effect can be set by using the Angle value.

The amount of distortion is controlled by the Intensity value; the  of the distortion, by the Size of the displacement map grid; the sharpen option allows you to decrease the blur on the final result.

.. _perlin_noise:

Perlin Noise
~~~~~~~~~~~~
 |Toonz71_428| 

Distorts the Source content by using a computer-generated displacement map image whose type can be chosen between Clouds and Marble/Wood.

The amount of distortion is controlled by the Intensity value; the , by the Size of the displacement map grid. The Horizontal and Vertical Offset, and the Evolution stage of the displacement map image can be controlled as well; by setting the variation of these values between two keys, you can set how much the displacement map moves and changes during the animation.

The Alpha option adds also a transparency displacement to fully-opaque images.

.. note:: The horizontal and vertical offset can also be set by using a point gadget in the work area (see  :ref:`Using FX Gadgets <using_fx_gadgets>`  ).

.. _random_wave:

Random Wave
~~~~~~~~~~~
 |Toonz71_429| 

Distorts the Source content creating a random wave effect that uses an automatically generated displacement map image. It can be used, for instance, to create a reflection on a water surface, or an underwater view. 

The stage of the displacement map image can be controlled by using the Evolution value; by setting the variation of this value between two keys, you set how much the displacement map image changes during the animation.

The position of the displacement map image can be shifted along the Horizontal and the Vertical axis. By setting the variation of this value between two keys, the distortion effect can be animated in any direction.

The amount of distortion is controlled by the Intensity value; the  of the distortion, by the Size of the displacement map grid; the sharpen option allows you to decrease the blur on the final result.

.. note:: The position along the horizontal and vertical axis can also be set by using a point gadget in the work area (see  :ref:`Using FX Gadgets <using_fx_gadgets>`  ).

.. _ripple:

Ripple
~~~~~~
 |Toonz71_430| 

Distorts the Source content creating a circular wave effect that uses an automatically generated displacement map image. The Quantity value sets the number of ripples; the Period value sets the distance between ripples; the Cycle shifts the ripple distortion, with increasing values expanding the ripples, and decreasing values collapsing them.

The Center of the circular waves can be set with a Horizontal and Vertical value; circular waves can be scaled in the Horizontal and Vertical directions, and rotated according to a set Angle. 

The amount of distortion is controlled by the Intensity value; the  of the distortion, by the Size of the displacement map grid; the sharpen option allows you to decrease the blur on the final result.

.. note:: The center and the period can be also set by using a point and a circle gadget with a handle in the work area (see  :ref:`Using FX Gadgets <using_fx_gadgets>`  ); the center can be set in the FX Settings preview as well.

.. _warp:

Warp
~~~~
 |Toonz71_431| 

Distorts the Source content according to the brightness variation of the node content connected to the Warper input handle, that is used as a displacement map image affecting the Source content.

The amount of distortion is controlled by the Intensity value; the  of the warp, by the Size of the displacement map grid; the sharpen option allows you to decrease the blur on the final result.

.. _gradients:

Gradients
'''''''''
.. _diamond_gradient:

Diamond Gradient
~~~~~~~~~~~~~~~~
 |Toonz71_432| 

Creates in the selected column a gradient, that goes hyperbolically from the center to the four corners, defined by a color spectrum (see  :ref:`Defining Colors and Color Spectrums <defining_colors_and_color_spectrums>`  ) and a Size value.

.. note:: The size can also be set by using a circle gadget with a handle in the work area (see  :ref:`Using FX Gadgets <using_fx_gadgets>`  ).

.. _four_points_gradient:

Four Points Gradient
~~~~~~~~~~~~~~~~~~~~
 |Toonz71_433| 

Creates in the selected column a gradient defined by four Colors, defined by Red, Green, Blue and Alpha values, whose source Points can be placed where needed defining horizontal (X) and vertical (Y) coordinates.

.. note:: The source points can also be set by using point gadgets in the work area (see  :ref:`Using FX Gadgets <using_fx_gadgets>`  ) and in the FX Settings preview as well.

.. _linear_gradient:

Linear Gradient
~~~~~~~~~~~~~~~
 |Toonz71_434| 

Creates in the selected column a gradual blend between two Colors defined by Red, Green, Blue and Alpha values. The Size controls the area of the gradient between the two colors.

You can also add a Distortion Wave on the linear gradient: the Amplitude sets the intensity of the distortion; the Frequency sets the number of waves creating the distortion; the Phase shifts the distorting waves.

.. note:: The size can also be set by using a gadget with two handles at the ends in the work area (see  :ref:`Using FX Gadgets <using_fx_gadgets>`  ).

.. _multi_linear_gradient:

Multi Linear Gradient
~~~~~~~~~~~~~~~~~~~~~
 |Toonz71_435| 

Creates in the selected column a multi linear gradient defined by a color spectrum (see  :ref:`Defining Colors and Color Spectrums <defining_colors_and_color_spectrums>`  ). The Period value sets the size of a spectrum gradient; the Quantity is the number of times the spectrum is repeated; the Phase shifts the gradient colors.

You can also add a Wave distortion on the multi linear gradient: the Amplitude sets the intensity of the distortion; the Frequency sets the number of waves creating the distortion; the Phase shifts the distorting waves.

.. note:: The period can also be set by using a gadget with two handles at the ends in the work area (see  :ref:`Using FX Gadgets <using_fx_gadgets>`  )

.. _multi_radial_gradient:

Multi Radial Gradient
~~~~~~~~~~~~~~~~~~~~~
 |Toonz71_436| 

Creates in the selected column a multi radial gradient defined by a color spectrum (see  :ref:`Defining Colors and Color Spectrums <defining_colors_and_color_spectrums>`  ). The Period value sets the size of a spectrum gradient; the Quantity is the number of times the spectrum is repeated; the Phase shifts the gradient colors.

.. note:: The period can be also set by using a circle gadget with a handle in the work area (see  :ref:`Using FX Gadgets <using_fx_gadgets>`  ).

.. _radial_gradient:

Radial Gradient
~~~~~~~~~~~~~~~
 |Toonz71_437| 

Creates in the selected column a gradual blend between two colors, defined by Red, Green, Blue and Alpha values, shading them in a circular pattern. The Inner Size controls the area where the gradient between the two colors begins; the Outer Size where it ends.

.. note:: The inner and outer sizes can be also set by using circle gadgets with a handle in the work area (see  :ref:`Using FX Gadgets <using_fx_gadgets>`  ).

.. _spiral:

Spiral
~~~~~~
 |Toonz71_438| 

Creates in the selected column a spiral pattern gradient defined by a color spectrum (see  :ref:`Defining Colors and Color Spectrums <defining_colors_and_color_spectrums>`  ). The Frequency sets the size and number of the spires; the Phase shifts the gradient colors.

.. _square_gradient:

Square Gradient
~~~~~~~~~~~~~~~
 |Toonz71_439| 

Creates in the selected column a square gradient, that goes linearly from the center to the four corners, defined by a color spectrum (see  :ref:`Defining Colors and Color Spectrums <defining_colors_and_color_spectrums>`  ) and a Size value.

.. note:: The size can also be set by using a rotated square gadget with handles in the work area (see  :ref:`Using FX Gadgets <using_fx_gadgets>`  ).

.. _image_adjust:

Image Adjust
''''''''''''
Adjust Levels
~~~~~~~~~~~~~
 |Toonz71_440| 

Adjusts the highlights and shadows of the Source content by remapping pixels intensity according to the Input and Output levels values for the RGB, Red, Green, Blue and Alpha channels; it also controls the Gamma value for each channel separately.

For each channel the Input values remaps pixel intensity whose value is equal or lower than the Minimum value, to 0, and those whose value is equal or higher than the Maximum value, to 255. This may be helpful to increase the contrast of an image.

For each channel the Output values remaps pixel intensity whose value is lower than the Minimum value, to the Minimum value, and those whose value is higher than the Maximum value, to the Maximum value. This may be helpful to decrease the contrast of an image.

.. _brightness_&_contrast:

Brightness & Contrast
~~~~~~~~~~~~~~~~~~~~~
 |Toonz71_441| 

Increases or decreases the brightness and contrast of the Source content. 

.. _despeckle:

Despeckle
~~~~~~~~~
 |Toonz71_442| 

Elimantes small imperfections (dirt, scratches, stains and similar) of the drawing. The size in pixels of the s that will be retouched can be defined in the Size input text field. The background of the images can be Transparent or White, the choise is available in the Detect On menu.

In the preview area is possible to check the results to avoid erasing s relevant for the drawing.

.. _channel_mixer:

Channel Mixer
~~~~~~~~~~~~~
 |Toonz71_443| 

Swaps the channels of the Source content. For each channel you can set if it remains as it is, or if you want it to have another channel mixed. For example to leave the red channel as it is, Red to Red is 1, the other channels to Red are 0; by setting Green to Red to 0.5 adds half intensity of the green channel to the red one.

It can be used for example to create a black and white key for an image with the alpha channel, by setting all the values to 0 but the Alpha to Red, Green, Blue and Alpha to 1. 

.. _curves:

Curves
~~~~~~
 |Toonz71_444| 

Adjusts the tonal range of the Source content by remapping pixels intensity according to a tonal curve for the RGB, Red, Green, Blue and Alpha channels.

The horizontal axis of the graph represents the original brightness levels of the pixels (Input levels); the vertical axis represents the new brightness levels (Output levels).

The default diagonal line indicates that no pixels are mapped to new values, so all pixels have the same Input and Output values. 

It is possible to use many adjustment points to correct the curve: to add a point, click the curve; to change the curve, use the point direction handles; to delete a point, select it and use the delete shortcut (by default the Delete button).

The Linear option constrains the curve to a series of straight segments.

.. _gamma:

Gamma
~~~~~
 |Toonz71_445| 

Changes the gamma value of the Source content.

.. _invert:

Invert
~~~~~~
 |Toonz71_446| 

Inverts the color values of the Source content, e.g. makes a positive black and white image negative, or a positive one from a scanned black and white negative. 

.. _multitone:

Multitone
~~~~~~~~~
 |Toonz71_447| 

Applies to the Source content the colors defined by a color spectrum (see  :ref:`Defining Colors and Color Spectrums <defining_colors_and_color_spectrums>`  ) according to the image brightness. The original image is turned into black and white and the color on the far left of the spectrum will be use for black pixels, the color on the far right for white pixels, and in-between colors for in-between grey pixels. 

.. _rgba_cut:

RGBA Cut
~~~~~~~~
 |Toonz71_448| 

Delimits the Minimum and the Maximum values of the Red, Green, Blue and Alpha components of the Source content. The maximum can be decreased from 255, the original value, to 0, when no red, green, blue or alpha component will be visible. The minimum can be increased from 0, the original value, to 255, when the red, green, blue components will be saturated, and alpha will be fully opaque.

.. _rgb_fade:

RGB Fade
~~~~~~~~
 |Toonz71_449| 

Fades the Source content toward a color defined by Red, Green and Blue values. The Intensity, expressed as a percentage, ranges from 0 (no fade) to 100 (fade to full color).

.. _rgba_scale:

RGBA Scale
~~~~~~~~~~
 |Toonz71_450| 

Changes the percentage of the Red, Green, Blue and Alpha components of the Source content. At 0 there is no red, green, blue or alpha component; at 100 the components have their original value.

.. _hsv_scale:

HSV Scale
~~~~~~~~~
 |Toonz71_451| 

Shifts the Hue, Saturation and Value values of the Source content. Hue ranges from -180 to 180; Saturation and Value from -100 to 100. All the three settings preserve their original value at 0.

.. _sharpen:

Sharpen
~~~~~~~
 |Toonz71_452| 

Increases the sharpness of the Source content according to a specific Intensity.

.. _layer_blending:

Layer Blending
''''''''''''''
.. _add:

Add
~~~
 |Toonz71_453| 

Adds the red, green and blue values of the Up node content to the Down one, pixel by pixel. 

If no Down node is defined, the adding operation is applied to all the images underlaying the Up node content according to the xsheet layering order.

The Intensity value expresses the percentage of values used in the addition; a negative value defines a subtraction instead of an addition. 

.. _color_burn:

Color Burn
~~~~~~~~~~
 |Toonz71_454| 

Darkens the pixel colors of the Down node content in order to reflect the color of the Up node content. The white in the Up node content does not affect the result.

If no Down node is defined, the color burning operation is applied to all the images underlaying the Up node content according to the xsheet layering order.

.. _color_dodge:

Color Dodge
~~~~~~~~~~~
 |Toonz71_455| 

Brightens the pixel colors of the Down node content in order to reflect the color of the Up node content. The black in the up node content does not affect the result.

If no Down node is defined, the color dodging operation is applied to all the images underlaying the Up node content according to the xsheet layering order.

.. _cross_dissolve:

Cross Dissolve
~~~~~~~~~~~~~~
 |Toonz71_456| 

Creates a cross-dissolve between the Up and Down node content. When the Intensity value is 0, only the Down node content is visible; when it is 100, only the Up one.

.. _darken:

Darken
~~~~~~
 |Toonz71_457| 

Compares the pixels color of the Up and Down node content and selects the darker one as the result color. The white in the Up node content does not affect the result; the black gives a black result.

If only one node is defined, the darkening operation is applied to all the images underlaying its content according to the xsheet layering order.

.. _dissolve:

Dissolve
~~~~~~~~
 |Toonz71_458| 

Eliminates randomly pixels from the Source content according to the set Intensity. 

.. _lighten:

Lighten
~~~~~~~
 |Toonz71_459| 

Compares the pixels color of the Up and Down node content and selects the lighter one as the result color. The black in the Up node content does not affect the result; the white gives a white result.

If only one node is defined, the lightening operation is applied to all the images underlaying the connected node according to the xsheet layering order.

.. _local_transparency:

Local Transparency
~~~~~~~~~~~~~~~~~~
 |Toonz71_460| 

Applies a transparency to the Source content according to the brightness value of the node content connected to the Reference input port.

The Intensity value amplifies uniformly the transparency given by the Reference node content.

.. _multiply:

Multiply
~~~~~~~~
 |Toonz71_461| 

Multiplies the red, green, blue and alpha values of the connected noded content. 

The Intensity value expresses the percentage of values used in the multiplication. By activating the Alpha option, also the alpha information is considered.

If only one node is defined, the multiplying operation is applied to all the images underlaying theupper node content according to the xsheet layering order.

.. _over:

Over
~~~~
 |Toonz71_462| 

Puts the connected nodes one over the other. Each time a node is connected a new port will be added, this way the overlap of columns can be defined regardless from the xsheet columns order.The columns order is up to bottom, where the column connected on the upper port is over the other ones.This can be used when you need to combine several nodes in a single one, for example to mask several columns with the same mask.

.. _premultiply:

Premultiply
~~~~~~~~~~~
Premultiplies the alpha channel of the Source node content. 

Full-color images which have a meaningful alpha channel come in two types: premultiplied or not. A non-premultiplied image can be recognized when it is loaded in OpenToonz because its edge, where there is a complete transparence on one side and opacity on the other, is not smooth, but displays a solid halo. With the premultiply effect it is possible to transform the image alpha-channel so that it is correctly read by OpenToonz.

.. note:: Full-color images can also be premultiplied by using a Level Settings option, or processed permanently in the browser, so that there is no need to apply the effect in the schematic (see  :ref:`Editing Level Settings <editing_level_settings>`  and  :ref:`Using the File Browser <using_the_file_browser>`  ).

.. _screen:

Screen
~~~~~~
 |Toonz71_463| 

Combines by multiplying the inverse of the pixels color of the Up and Down node content, giving a result color that is lighter than both Up and Down node pixels, except when one of them equals 0. The black in the Up node content does not affect the result; the white gives a white result.

If no Down node is defined, the screening operation is applied to all the images underlaying the Up node content according to the xsheet layering order.

.. _subtract:

Subtract
~~~~~~~~
 |Toonz71_464| 

Subtracts the red, green and blue values of the Up node content from the Down one, pixel by pixel. By activating the Alpha option, also the alpha information is considered. 

If only one node is defined, the screening operation is applied to all the images underlaying connected node content according to the xsheet layering order.

.. _transparency:

Transparency
~~~~~~~~~~~~
 |Toonz71_465| 

Sets the transparency of the Source content. The Intensity, expressed as a percentage, ranges from 0, fully opaque, to 100, fully transparent.

.. note:: In the FXs that accept multiple input nodes it is possible to change the stacking order of the input nodes by clicking and dragging in ports area.

.. _light:

Light
'''''
.. _backlit:

Backlit
~~~~~~~
 |Toonz71_466| 

Creates a backlit effect, using the Light node content as a light source affecting the Source node content. The light node content can be also faded to a Color defined by Red, Green and Blue values, according to the set Intensity.

.. _body_highlight:

Body Highlight
~~~~~~~~~~~~~~
 |Toonz71_467| 

Creates a highlighted area for the Source node content, according to its alpha channel. You can set the Color of the highlight, as well as a Transparency and a Blur value to be applied.

The shifting of the highlighted area is defined by horizontal (X) and vertical (Y) Offset values, that can also be interactively set in the preview of the FX Settings window, where the offset center is displayed with a cross.

Enabling the Invert option the effected areas will be toggled.

The effect can be used to create a body shadow as well, by defining a black color for the highlight.

.. _cast_shadow:

Cast Shadow
~~~~~~~~~~~
 |Toonz71_468| 

Turns the Source content into a shadow that can be distorted and faded to a color with a variable transparency and blur.

The distortion can be done like in the Free Distort effect (see  :ref:`Free Distort <free_distort>`  ). The fade Color can be defined by Red, Green and Blue values and an Intensity can be set. A different Blur and Transparency value can be set for the top and the bottom part of the Source content, in order to have a more realistic shadow.

.. _glow:

Glow
~~~~
 |Toonz71_469| 

Creates a glowing effect, using the Light node content as a light glowing on the node content connected to the Source input port. The Blur and Brightness of the glowing can be set; the Light node content can be also faded to a color defined by Red, Green and Blue values, according to the set Intensity.

If no Source node is defined, the glowing is applied to all the images underlaying the Light node content according to the xsheet layering order.

.. _light_spot:

Light Spot
~~~~~~~~~~
 |Toonz71_470| 

Creates in the selected column a light spot whose size and color can be set respectively with the Width and Height values, and the Reg, Green, Blue and Alpha values. The Softness sets the light diffusion in the area outside the spot.

.. note:: The width and height can be also set by using a box gadget with handles in the work area (see  :ref:`Using FX Gadgets <using_fx_gadgets>`  ).

.. _raylit:

Raylit
~~~~~~
 |Toonz71_471| 

Places a source of light behind the Source node content, casting rays of light outside or inside the image outline.

The light source position is defined by horizontal (X) and vertical (Y) coordinates. By changing the light source position you change the way rays are cast along the image outline; by changing the Distance value you can make the light source approach to or go away from the image.

Properties of the light can be set by defining the Intensity, the Color, that is set by Red, Green, Blue and Alpha values, the Decay, that is the decrease of the light intensity according to its distance from the image, and the Smoothness, that determines how sharp the rays are along the image outline.

The Invert option switches the casting of rays of light from the outside of the image to the inside.

.. note:: The center can be also set by using a point gadget in the work area (see  :ref:`Using FX Gadgets <using_fx_gadgets>`  ) and in the FX Settings preview.

.. note:: The Source node content needs to have a significant alpha channel in order to have an effective result.

.. _color_raylit:

Color Raylit
~~~~~~~~~~~~
 |Toonz71_472| 

Places a source of light behind the Source node content, casting rays of light outside the image outline.

The light source position is defined by horizontal (X) and vertical (Y) coordinates. By changing the light source position you change the way rays are cast along the image outline; by changing the Distance value you can make the light source approach to or go away from the image.

The colours of the rays are calculated from the original drawing colours.

Properties of the light can be set by defining the Intensity, the Decay, that is the decrease of the light intensity according to its distance from the image, and the Smoothness, that determines how sharp the rays are along the image outline.

The Keep image check-box determines if the original drawing is rendered in the output or not.

.. _target_spot:

Target Spot
~~~~~~~~~~~
 |Toonz71_473| 

Creates in the selected column a light spot whose size and color can be set respectively with the Width and Height values, and the Red, Green, Blue and Alpha values. The direction of the spot can be set by defining the Distance of the light from the table and the Angle between the light spot direction and the table. The Decay, that is the decrease of the light intensity according to the distance from table, can be controlled as well.

.. _matte:

Matte
'''''
.. _erode/dilate:

Erode/Dilate
~~~~~~~~~~~~
 |Toonz71_474| 

Morphologically erodes or dilates the alpha channel of the connected node by the specified value, where positive values correspond to dilations and negative ones to erosion.

.. _hsv_key:

HSV Key
~~~~~~~
 |Toonz71_475| 

The Type parameter specifies the filter shape to be applied, the square filter being faster than the circular. Key

Defines a chroma key for the Source content using the set Hue, Saturation and Value values. You can set the range for each value by using the related Range slider. The selection can be inverted using the Invert button.

.. _matte_in:

Matte In
~~~~~~~~
 |Toonz71_476| 

Makes the Source content visible only inside the opaque areas of the node content connected to the Matte input port.

.. _matte_out:

Matte Out
~~~~~~~~~
 |Toonz71_477| 

Makes the source content visible only outside the opaque areas of the node content connected to the Matte input port.

.. _rgb_key:

RGB Key
~~~~~~~
 |Toonz71_478| 

Defines a chroma key for the Source content using the set Red, Green and Blue values. You can set the range for each value by using the related Range slider. The selection can be inverted using the Invert button.

.. _visible_matte_in:

Visible Matte In
~~~~~~~~~~~~~~~~
 |Toonz71_479| 

Makes the Up node content visible only inside the opaque areas of the node content connected to the Down input port, keeping the Down node still visible.

.. _noise:

Noise
'''''
Noise
~~~~~
 |Toonz71_480| 

Adds a noise effect to the Source content according to the set Intensity. You can decide which noise component among Red, Green and Blue you want to activate, and if the result has to be in Black and White.

.. _salt_&_pepper_noise:

Salt & Pepper Noise
~~~~~~~~~~~~~~~~~~~
 |Toonz71_481| 

Adds a black and white noise effect to the Source content according to the set Intensity. 

Render
''''''
.. _clouds:

Clouds
~~~~~~
 |Toonz71_482| 

Creates in the selected column a fractal image whose type can be chosen between Clouds and Marble/Wood. The Size affect the grid used for generating the fractal image; a color spectrum defines the used colors (see  :ref:`Defining Colors and Color Spectrums <defining_colors_and_color_spectrums>`  ).

Increasing the Minimum value shifts the color spectrum to the right, and consequently more pixels will be colored as the color defined at the far left of the spectrum. Decreasing the Maximum value shifts the color spectrum to the left, and consequently more pixels will be colored as the color defined at the far right of the spectrum.

The Evolution stage of the fractal image can be controlled as well; by setting the variation of this value between two keys, you set how much the fractal image changes during the animation.

.. _particles:

Particles
~~~~~~~~~
See  :ref:`Using the Particles Effect <using_the_particles_effect>` .

.. _stylize:

Stylize
'''''''
.. _color_emboss:

Color Emboss
~~~~~~~~~~~~
 |Toonz71_483| 

Traces the edges of the Source content with a combination of highlights and shadows. You can set the Intensity of the effect, and the Distance and Direction of the light that create the emboss effect. The Radius sets the depth of the embossing.

By connecting a node to the Controller port, the Source content will be embossed according to the Controller node content.

.. _emboss:

Emboss
~~~~~~
 |Toonz71_484| 

Turns the Source content to grey areas and traces its edges with a combination of highlights and shadows. You can set the Intensity of the effect, and the Distance and Direction of the light that create the emboss effect. The Radius sets the depth of the embossing.

.. _mosaic:

Mosaic
~~~~~~
 |Toonz71_485| 

Turns the Source content in a series of tiles according to the specified Size and Distance. The color and transparency of the tiles are sampled from the source content. 

A Background Color can be set, and will be visible around the tiles. The tile shape can be chosen between Square and Round.

.. _posterize:

Posterize
~~~~~~~~~
 |Toonz71_486| 

Converts the Source content into a number of shades according to the set number of Levels. The shades depends on the brightness values of the source content and the levels are intended for each channel; for example, two levels produces six colors: two for the red, two for the green, and two for the blue.

.. _solarize:

Solarize
~~~~~~~~
 |Toonz71_487| 

Blends a negative and a positive version of the Source content, as if exposing a photographic print briefly to light during development. You can set the Intensity of the effect and control the Peak Edge, that is the amount of positive and negative image that is used in the blend.

.. _toonz_level:

Toonz Level
'''''''''''
The Toonz Level special FX can be applied only to Toonz raster and vector levels (TLV and PLI files). They usually affect the drawings they are applied to according to style indexes. Style indexes can be retrieved in the palette after the # symbol in the style tooltip, or in the bottom right corner of the style in large thumbnails mode. 

Index numbers can be specified in the related text field. They have to be separated by a comma; to define a range of indexes, you can type the first and the last separated by a dash (e.g. 4-7 will refer to indexes 4, 5, 6 and 7). To select all indexes, type ``all`` ; to select no index, type ``none`` .

Toonz Level special FX have to be always applied first when a series of special FX are applied to an animation level, as they work only on Toonz raster or vector levels that have not been transformed by other effects. However two or more Toonz Level special FX can be applied to the same animation level.

.. _art_contour:

Art Contour
~~~~~~~~~~~
 |Toonz71_488| 

Creates in the Source content a pattern, by repeating the Controller node content, along lines painted with styles whose indexes are specified in the Color Indexes text field. It can be used for example to create scattered brush, or hair and fur effects along drawing lines.

The Keep Color option assigns the color of the line to the applied pattern; while the Keep Contour option retains the drawing line that will be visible beneath the pattern.

The way the contents of the Controller node create the pattern depends on the Pattern settings. 

The Density sets the amount of pattern to be applied along the line. By setting the Density to 0, you can specify a Minimum and Maximum Distance between two subsequent images applied as pattern on the line.

The Size sets the Minimum and Maximum resizing percentage applied to the images used as the pattern; the value 100 is the original size of the images.

The Orientation sets the Minimum and Maximum rotation angle for the images used as the pattern, according to the line direction; the value 0 display the images perpendicular to the line direction. If the Absolute Orientation option is used, the orientation values do not depend on the direction of the lines: the value 0 is the original images orientation.

.. _calligraphic_line:

Calligraphic Line
~~~~~~~~~~~~~~~~~
 |Toonz71_489| 

Changes in the Source content the thickness of the drawing lines painted with styles whose indexes are specified in the Color Indexes text field. 

You can specify the Thickness increase and how it is applied, as a percentage, to the different line directions Horizontal, Vertical, Up Diagonal, Down Diagonal.

The Smoothness sets the smoothness of the passage between sections of the lines affected by the effect, and those not affected; while the Noise sets the regularity of the edge of the line.

.. _color_blending:

Color Blending
~~~~~~~~~~~~~~
 |Toonz71_490| 

Blends in the Source content lines and areas painted with styles whose indexes are specified in the Color Indexes text field. It can be used for example to blend shadow and highlight areas with the plain colored area, or to create gradients of colors.

The Intensity sets how wide the blended area between the selected colors will be; while the Smoothness sets how smooth the dithering between blended colors is.

The No Blending over Other Colors option stops the blending as soon as a line, or an area, whose index is not included in the selection, is detected; if deactivated, the blending between selected colors continues under excluded lines and areas.

.. _external_palette:

External Palette
~~~~~~~~~~~~~~~~
 |Toonz71_491| 

Applies to the Source content the palette node connected to the Palette input port; if a column node is connected to the Palette input port, the palette related to its content will be considered. 

The original styles of the Toonz levels contained in the source node are replaced with those of the levels contained in the palette node according to their style indexes.

.. _outline:

Outline
~~~~~~~
 |Toonz71_492| 

Changes in the Source content the thickness of the drawing external outline. 

You can specify the Thickness increase and how it is applied, as a percentage, to the different line directions Horizontal, Vertical, Up Diagonal, Down Diagonal.

The Smoothness sets the smoothness of the passage between sections of the lines affected by the effect, and those not affected; while the Noise sets the regularity of the edge of the outline.

.. _palette_filter:

Palette Filter
~~~~~~~~~~~~~~
 |Toonz71_493| 

Filters the styles of the Source content palette according to the indexes specified in the Color Indexes text field.

The Apply To option menu lets you choose if you want to affect Lines & Area, only Lines or only Areas, even if painted with the same styles; the Action option menu lets you choose if you want to keep or remove the specified styles. 

.. _pinned_texture:

Pinned Texture
~~~~~~~~~~~~~~
 |Toonz71_494| 

Distorts the Texture node content and applies it to the Source content areas that are painted with styles whose indexes are specified in the Color Indexes text field.

The distortion can be done like in the Free Distort effect (see  :ref:`Free Distort <free_distort>`  ) and the texture can be applied like in the Texture effect (see below).

.. _texture:

Texture
~~~~~~~
 |Toonz71_495| 

Applies the Texture node content to the Source content lines and areas that are painted with styles whose indexes are specified in the Color Indexes text field.

As the texture node content can be animated as you like, this effect allows you to generate animated texture as well.

The Action option menu lets you choose if you want to apply the texture to the specified styles (Keep) or to apply it to all styles except for the specified ones (Delete). 

The Mode option menu lets you set how the texture node content will be applied: Texture uses the texture to replace selected styles; Pattern preserves the original colors but varies them according to the texture brightness; Add, Subtract, Multiply, Lighten and Darken defines the way the texture is applied to the original colors (see  :ref:`Layer Blending <layer_blending>`  ). In case the Add, subtract or Multiply mode are selected, you can also set the Value of the effect.

.. note:: To repeat the texture image and tile it to create a larger texture, you can apply the Tile effect to the texture column before linking it to the Texture node (see  :ref:`Tile <tile>`  ).

.. _shaders:

Shaders
'''''''
OpenToonz enables support for special fxs rendered through hardware-accelereted pixelshaders. Shaders are simple programs compiled by a graphics processing unit that harness the massively parallel architecture of modern graphics devices to execute with extreme speed. OpenToonz's shader fxs are written in the OpenGL Shading Language (GLSL), and are located in PROJECTROOT/library/shaders. Refer to the readme.txt file there for further s on editing or creating new shader fxs.

.. _caustic:

Caustic
~~~~~~~
 |Toonz71_496| 

Create in the selected column a simulation of the reflection of light on a water surface. Sets the color of the water defining the RGBA values of the Water Color parameter. 

The stage of the displacement map image can be controlled by using the Evolution value; by setting the variation of this value between two keys, you set how much the displacement map image changes during the animation.





.. _fireball:

Fireball
~~~~~~~~
 |Toonz71_497| 

Create in the selected column a ball of flames erupting from a point.

A range of colors can be defined setting the RGBA values of color 1 and color 2. The stage of the displacement map image can be controlled by using the Evolution value; by setting the variation of this value between two keys, you set how much the displacement map image changes during the animation.



.. _glitter:

Glitter
~~~~~~~
 |Toonz71_498| 

Adds cross-shaped light rays extending from the brightest part of an image.

Use Threshold to specify the cut-out on the input image's brightest part. Higher values will make the fx add lights also to darker image parts, producing more lights. The Brightness specifies the brightness of added light rays; the Radius specify how much the light rays will extend from bright input pixels; the Angle specify the angle of light crosses. A value 0 means that produced light crosses will be axis-aligned. Halo is the amount of light disperion orthogonal to the direction of light rays. Higher values will produce broader rays.

.. _star_sky:

Star Sky
~~~~~~~~
 |Toonz71_499| 

Creates, in the selected column, a simple star field with variable brightness with overlayed clouds. Sets the color of the overlayed clouds defining the RGBA values of the Cloud Color parameter. 

The stage of the stars displacement can be controlled by using the Evolution value; by setting the variation of this value between two keys, you set how much the displacement map image changes during the animation.

Use the Brightness parameters to define the brightness of the stars.



.. _sun_flare:

Sun Flare
~~~~~~~~~
 |Toonz71_500| 

Creates, in the selected column, rays of colored light extending from a radial gradient at the center. Sets the color of the sun rays defining the RGBA values of the Cloud Color parameter. The number of rays is defined by the Rays parameter while their brightness is set by the Intensity one. The angle parameter sets the direction of the rays and the Bias parameter define the size of the rays. Use the Sharpness parameter to make the rays sharper or smoother.





.. _wavy:

Wavy
~~~~
 |Toonz71_501| 

Creates a simple gradient with a colored 'wavy' pattern in the selected column.The waves colors are definied by setting the RGBA value of the Color and Color 2 parameters. The stage of the displacement map image can be controlled by using the Evolution value; by setting the variation of this value between two keys, you set how much the displacement map image changes during the animation.





.. _gpu_radial_blur:

GPU Radial Blur
~~~~~~~~~~~~~~~
 |Toonz71_502| 

Blurs along radial lines whose origin is the set Center, defined by horizontal (X) and vertical (Y) coordinates, starting from an unaffected inner area defined by the Safe Radius. The Blur Factor parameter sets the amount of blur.

.. _gpu_spin_blur:

GPU Spin Blur
~~~~~~~~~~~~~
 |Toonz71_503| 

Blurs along concentric circular lines as if the Source content turns around the set Center, defined by horizontal (X) and vertical (Y) coordinates, starting from an unaffected inner area defined by the Safe Radius. The Blur parameter sets the amount of blur.


.. |Toonz71_390| image:: /applying_special_fx\Inserting Special FX\FX Browser.gif
.. |Toonz71_391| image:: /applying_special_fx\Inserting Special FX\Basic FX Example.gif
.. |Toonz71_392| image:: /applying_special_fx\Inserting Special FX\Combined FX Example.gif
.. |Toonz71_393| image:: /applying_special_fx\Inserting Special FX\Generated FX Example
.. |Toonz71_401| image:: /_static/Toonz71/Toonz71_401.gif
.. |Toonz71_408| image:: /_static/Toonz71/Toonz71_408.gif
.. |Toonz71_414| image:: /_static/Toonz71/Toonz71_414.gif
.. |Toonz71_415| image:: /_static/Toonz71/Toonz71_415.gif
.. |Toonz71_417| image:: /_static/Toonz71/Toonz71_417.gif
.. |Toonz71_418| image:: /_static/Toonz71/Toonz71_418.gif
.. |Toonz71_419| image:: /_static/Toonz71/Toonz71_419.gif
.. |Toonz71_420| image:: /_static/Toonz71/Toonz71_420.gif
.. |Toonz71_421| image:: /_static/Toonz71/Toonz71_421.gif
.. |Toonz71_422| image:: /_static/Toonz71/Toonz71_422.gif
.. |Toonz71_423| image:: /_static/Toonz71/Toonz71_423.gif
.. |Toonz71_424| image:: /_static/Toonz71/Toonz71_424.gif
.. |Toonz71_425| image:: /_static/Toonz71/Toonz71_425.gif
.. |Toonz71_426| image:: /_static/Toonz71/Toonz71_426.gif
.. |Toonz71_427| image:: /_static/Toonz71/Toonz71_427.gif
.. |Toonz71_428| image:: /_static/Toonz71/Toonz71_428.gif
.. |Toonz71_429| image:: /_static/Toonz71/Toonz71_429.gif
.. |Toonz71_430| image:: /_static/Toonz71/Toonz71_430.gif
.. |Toonz71_431| image:: /_static/Toonz71/Toonz71_431.gif
.. |Toonz71_432| image:: /_static/Toonz71/Toonz71_432.gif
.. |Toonz71_433| image:: /_static/Toonz71/Toonz71_433.gif
.. |Toonz71_434| image:: /_static/Toonz71/Toonz71_434.gif
.. |Toonz71_435| image:: /_static/Toonz71/Toonz71_435.gif
.. |Toonz71_436| image:: /_static/Toonz71/Toonz71_436.gif
.. |Toonz71_437| image:: /_static/Toonz71/Toonz71_437.gif
.. |Toonz71_438| image:: /_static/Toonz71/Toonz71_438.gif
.. |Toonz71_439| image:: /_static/Toonz71/Toonz71_439.gif
.. |Toonz71_440| image:: /_static/Toonz71/Toonz71_440.gif
.. |Toonz71_441| image:: /_static/Toonz71/Toonz71_441.gif
.. |Toonz71_442| image:: /_static/Toonz71/Toonz71_442.gif
.. |Toonz71_443| image:: /_static/Toonz71/Toonz71_443.gif
.. |Toonz71_444| image:: /_static/Toonz71/Toonz71_444.gif
.. |Toonz71_445| image:: /_static/Toonz71/Toonz71_445.gif
.. |Toonz71_446| image:: /_static/Toonz71/Toonz71_446.gif
.. |Toonz71_447| image:: /_static/Toonz71/Toonz71_447.gif
.. |Toonz71_448| image:: /_static/Toonz71/Toonz71_448.gif
.. |Toonz71_449| image:: /_static/Toonz71/Toonz71_449.gif
.. |Toonz71_450| image:: /_static/Toonz71/Toonz71_450.gif
.. |Toonz71_451| image:: /_static/Toonz71/Toonz71_451.gif
.. |Toonz71_452| image:: /_static/Toonz71/Toonz71_452.gif
.. |Toonz71_453| image:: /_static/Toonz71/Toonz71_453.gif
.. |Toonz71_454| image:: /_static/Toonz71/Toonz71_454.gif
.. |Toonz71_455| image:: /_static/Toonz71/Toonz71_455.gif
.. |Toonz71_456| image:: /_static/Toonz71/Toonz71_456.gif
.. |Toonz71_457| image:: /_static/Toonz71/Toonz71_457.gif
.. |Toonz71_458| image:: /_static/Toonz71/Toonz71_458.gif
.. |Toonz71_459| image:: /_static/Toonz71/Toonz71_459.gif
.. |Toonz71_460| image:: /_static/Toonz71/Toonz71_460.gif
.. |Toonz71_461| image:: /_static/Toonz71/Toonz71_461.gif
.. |Toonz71_462| image:: /_static/Toonz71/Toonz71_462.gif
.. |Toonz71_463| image:: /_static/Toonz71/Toonz71_463.gif
.. |Toonz71_464| image:: /_static/Toonz71/Toonz71_464.gif
.. |Toonz71_465| image:: /_static/Toonz71/Toonz71_465.gif
.. |Toonz71_466| image:: /_static/Toonz71/Toonz71_466.gif
.. |Toonz71_467| image:: /_static/Toonz71/Toonz71_467.gif
.. |Toonz71_468| image:: /_static/Toonz71/Toonz71_468.gif
.. |Toonz71_469| image:: /_static/Toonz71/Toonz71_469.gif
.. |Toonz71_470| image:: /_static/Toonz71/Toonz71_470.gif
.. |Toonz71_471| image:: /_static/Toonz71/Toonz71_471.gif
.. |Toonz71_472| image:: /_static/Toonz71/Toonz71_472.gif
.. |Toonz71_473| image:: /_static/Toonz71/Toonz71_473.gif
.. |Toonz71_474| image:: /_static/Toonz71/Toonz71_474.gif
.. |Toonz71_475| image:: /_static/Toonz71/Toonz71_475.gif
.. |Toonz71_476| image:: /_static/Toonz71/Toonz71_476.gif
.. |Toonz71_477| image:: /_static/Toonz71/Toonz71_477.gif
.. |Toonz71_478| image:: /_static/Toonz71/Toonz71_478.gif
.. |Toonz71_479| image:: /_static/Toonz71/Toonz71_479.gif
.. |Toonz71_480| image:: /_static/Toonz71/Toonz71_480.gif
.. |Toonz71_481| image:: /_static/Toonz71/Toonz71_481.gif
.. |Toonz71_482| image:: /_static/Toonz71/Toonz71_482.gif
.. |Toonz71_483| image:: /_static/Toonz71/Toonz71_483.gif
.. |Toonz71_484| image:: /_static/Toonz71/Toonz71_484.gif
.. |Toonz71_485| image:: /_static/Toonz71/Toonz71_485.gif
.. |Toonz71_486| image:: /_static/Toonz71/Toonz71_486.gif
.. |Toonz71_487| image:: /_static/Toonz71/Toonz71_487.gif
.. |Toonz71_488| image:: /_static/Toonz71/Toonz71_488.gif
.. |Toonz71_489| image:: /_static/Toonz71/Toonz71_489.gif
.. |Toonz71_490| image:: /_static/Toonz71/Toonz71_490.gif
.. |Toonz71_491| image:: /_static/Toonz71/Toonz71_491.gif
.. |Toonz71_492| image:: /_static/Toonz71/Toonz71_492.gif
.. |Toonz71_493| image:: /_static/Toonz71/Toonz71_493.gif
.. |Toonz71_494| image:: /_static/Toonz71/Toonz71_494.gif
.. |Toonz71_495| image:: /_static/Toonz71/Toonz71_495.gif
.. |Toonz71_496| image:: /_static/Toonz71/Toonz71_496.gif
.. |Toonz71_497| image:: /_static/Toonz71/Toonz71_497.gif
.. |Toonz71_498| image:: /_static/Toonz71/Toonz71_498.gif
.. |Toonz71_499| image:: /_static/Toonz71/Toonz71_499.gif
.. |Toonz71_500| image:: /_static/Toonz71/Toonz71_500.gif
.. |Toonz71_501| image:: /_static/Toonz71/Toonz71_501.gif
.. |Toonz71_502| image:: /_static/Toonz71/Toonz71_502.gif
.. |Toonz71_503| image:: /_static/Toonz71/Toonz71_503.gif
.. |camera_stand| image:: /_static/sfx/camera_stand.png
.. |fit_to_window| image:: /_static/sfx/fit_to_window.png
.. |focus_on_current| image:: /_static/sfx/focus_on_current.png
.. |fx| image:: /_static/sfx/fx.png
.. |key| image:: /_static/sfx/key.png
.. |maximize| image:: /_static/sfx/maximize.png
.. |minimize| image:: /_static/sfx/minimize.png
.. |next_key| image:: /_static/sfx/next_key.png
.. |output| image:: /_static/sfx/output.png
.. |preview_black| image:: /_static/sfx/preview_black.png
.. |preview_checkbox| image:: /_static/sfx/preview_checkbox.png
.. |preview_white| image:: /_static/sfx/preview_white.png
.. |preview| image:: /_static/sfx/preview.png
.. |prevkey| image:: /_static/sfx/prevkey.png
.. |reorder_nodes| image:: /_static/sfx/reorder_nodes.png
.. |reset| image:: /_static/sfx/reset.png
.. |schematic| image:: /_static/sfx/schematic.png
