.. _managing_palettes_and_styles:

Managing Palettes and Styles
============================
In OpenToonz, each Toonz raster and vector animation level comes with its own palette containing styles that can be used to draw lines and paint lines and areas. Raster levels, on the contrary, can be edited by using styles available in the raster drawing palette, that is shared by all of the raster levels.

In Toonz levels, palette styles are interactively “linked” to drawn lines and filled areas by using indexes. The main advantage of this method is that if you edit a style of the palette, all the lines and filled areas using that style will be automatically updated. This allows you to change or calibrate colors, even after the painting process has been done, without correcting the style line by line, or area by area.

In raster levels, palette styles are simply used to draw or touch up images, and no link exists between the styles and the drawn lines. This palette, named Raster Drawing Palette, is shared by all the raster levels belonging to a specific project and is stored in the ``+palettes``  project default folder (see  :ref:`Project Default Folders <project_default_folders>`  ).

.. note:: All the editing performed in palettes and styles is not saved until you save the related Toonz level, the palette itself, or the Save All command is used (see  :ref:`Saving Levels <saving_levels>`  ).

.. _the_palette_window:

The Palette Editor
------------------

|palette| 
 
The palette editor displays the styles of the current animation level that are used, or can be used, to draw and paint the level itself. 

The default palette of any new Toonz vector level contains only the plain black color; the default palette of a Toonz raster level contains the colors recognized during the cleanup process. Any palette always contains the Color 0 item, that allows you to remove any style from lines and filled areas. 

.. note:: Each palette can contain up to 4096 styles.

Styles in the palette can be displayed in different modes:

- Small Thumbnails View displays styles as small squares. The style index is displayed at the bottom right corner. Full name of the style can be displayed as a tooltip.

- Medium Thumbnails View displays styles as medium squares. You can read the first letters of the name of the style directly inside the chips; the style index is displayed at the bottom right corner. Full name of the style can be displayed as a tooltip. 

- Large Thumbnails View displays styles as large squares. You can read the first letters of the name of the style directly inside the chips; the style index is displayed at the bottom right corner. Full name of the style can be displayed as a tooltip. 

- List View displays style thumbnails next to their names in a list; the index of the style is displayed as a tooltip. If the palette styles refer to a studio palette, its path will be displayed along with the style name (see  :ref:`Using the Studio Palette <using_the_studio_palette>`  ).

By default each palette is active, that means that it automatically displays the styles of the current animation level, but it can be turned off in order not to be updated when you select a different level. In this way, by opening more than one palette it is possible to compare and edit palettes referring to different animation levels at the same time.

Palettes also can be saved as independent files in TPL format, to be loaded back into the scene to retrieve colors, or to be used with the External Palette FX (see  :ref:`Using the File Browser <using_the_file_browser>`  and  :ref:`External Palette <external_palette>`  ).

.. note:: Most of the palette editing described below can be applied to the palette viewer available in the studio palette as well (see  :ref:`Using the Studio Palette <using_the_studio_palette>`  ).

.. tip:: **To change the palette display mode:**

    Do one of the following:
    
    - Click the option button ( |Toonz71_127| ) on the right of the top bar of the palette editor, and choose a display mode from the menu that opens.
    
    - Use the standard zoom ``+`` or ``-`` shortcut keys in the palette editor to increase or decrease the styles chips size.


.. tip:: **To make the palette inactive or active:**

    Click the switch button ( |Toonz71_128| ) on the right of the palette editor title bar.



.. tip:: **To save a palette with a different name in a different location:**

    1. Click the Save Palette As button () in the top bar of the palette editor.

    2. In the browser that opens choose a location and name for the palette you want to save, and click the Save button.

.. note:: The Save Palette As command creates a copy of the palette with a different file name and location, but does not change the name and location of the palette used in the scene.


.. _arranging_palette_styles_and_pages:

Arranging Palette Styles and Pages
''''''''''''''''''''''''''''''''''
Palette styles can be added, named, reordered and arranged in pages. They can be copied and pasted from one position to another, or from a palette to another.

.. note:: When styles used for painting drawings are cut, lines and areas painted with them will be displayed in red; if they are deleted, you will be prompted whether to delete the styles only and show the lines and areas painted with them in red, or to delete the lines and areas painted with them as well.

.. tip:: **To select a style:**

    Do one of the following:

    - Click it in the palette editor.
    
    - Use the number keys on the main or numerical keyboards to select the corresponding style. 
    
.. note:: When in Medium/Large Thumbnails View a visual cue of which key shortcut corresponds to which style is shown on the upper center of each style chip.

.. note:: In case of having more than 10 styles in the current palette, you can use the Tab key on the keyboard to switch to the next bank of 10 styles. 

.. tip:: **To select multiple styles:**

    Do one of the following:

    - Shift-click to extend the selection.

    - Ctrl-click (PC) or Cmd-click (Mac) to add a style to, or remove it from the selection.

.. tip:: **To add a new style:**

    Click the New Style button ( |Toonz71_130| ) in the top bar of the palette editor. 

.. tip:: **To name a style:**

    When styles are displayed in Medium/Large Thumbnails View or List View modes, double-click the style name to edit it.

.. tip:: **To edit palette styles with the Edit menu commands:**

    1. Select the styles you want to edit.

    2. Do any of the following:

    - Use the Copy command to keep in memory selected styles for further operations.

    - Use the Cut command to eliminate selected styles from the palette and keep them in memory for further operations.

    - Use the Paste Insert command to paste styles kept in memory in the palette, after the currently selected style. Cut styles will be added preserving their indexes; copied styles will be added using new indexes.

    - Use the Paste Color & Name command to paste styles kept in memory, over the styles selected in the palette, overwriting their content. If the selection contains less styles than those kept in memory, styles in excess will be ignored; if the selection contains more styles than those kept in memory, styles in excess will be left as they are.

    - Use the Paste Color command to paste the red, green, blue and alpha values of the styles kept in memory in the styles selected in the palette, preserving their name. If the selection contains less styles than those kept in memory, styles in excess will be ignored; if the selection contains more styles than those kept in memory, styles in excess will be left as they are. 
    
    - Use the Paste Name command to paste the names of the styles kept in memory in the styles selected in the palette, preserving their colors. If the selection contains less styles than those kept in memory, styles in excess will be ignored; if the selection contains more styles than those kept in memory, styles in excess will be left as they are. 

    - Use the Delete command to delete selected styles.

.. note:: All the Edit menu commands are also available in the menu that opens when right-clicking the selection.

.. tip:: **To move selected styles:**

    Ctrl-click (PC) or Cmd-click (Mac) and drag the selection to the new position; the insertion point is marked while you drag.

.. tip:: **To move selected styles into a different page:**

    Ctrl-click (PC) or Cmd-click (Mac) and drag the selection to the tab of the page where you want to put selected styles.

.. tip:: **To move styles into a new page:**

    Ctrl-click (PC) or Cmd-click (Mac) and drag the selection to the right of the last page tab: a new page will be created containing the dragged styles.

.. tip:: **To remove all the unused styles:**

    Right-click in the palette and choose Remove Unused Styles from the menu that opens.

.. tip:: **To add a new page:**

    Do one of the following:

    - Click the New Page button ( |Toonz71_131| ) in the top bar of the palette editor.

    - Right-click in the palette area where page tabs are displayed and choose New Page from the menu that opens.

.. tip:: **To name a page:**

    Double-click the page name to edit it.

.. tip:: **To move a page:**

    Click and drag the page tab to the new position.

.. tip:: **To delete a page:**

    Right-click the page tab and choose Delete Page from the menu that opens. The current page cannot be deleted.


.. _using_the_studio_palette:

Using the Studio Palette
------------------------
 |studio_palette| 

The studio palette allows you to store and manage an unlimited number of palettes. It is intended as a library of character and prop palettes related to one or more specific productions. From here palettes, or styles contained in them, can be retrieved, assigned, or merged to the current level palette, with no need to define the same styles again and again. 

It consists of a palette tree and a palette viewer: the palette tree lists two main folders, Global Palettes and Project Palettes, and all the folders and palettes you add; the palette viewer displays the currently selected palette and allows you to edit it as a standard palette (see  :ref:`The Palette Window <the_palette_window>`  ).

Any level palette can be added to the studio palette; if a color model is defined for that level, it will be saved along with the palette and retrieved any time that palette will be assigned to a level (see  :ref:`Using a Color Model <using_a_color_model>`  ).

Palettes added to the Global Palettes folder will be available in the studio palette in any OpenToonz session, regardless of the current project. 

Palettes added to the Project Palettes folder will be available only when the current project is the relevant one. For example if your current project is Production One, and you add some palettes to the Project Palettes folder, those palettes will be available only when the current project is Production One. 

If you want to add to the studio palette a series of palettes you have previously created and stored in a folder, you can also automatically retrieve them by searching that specific folder.

Styles that are imported from the studio palette to the palette of the current level are marked with a small white square. This reference can be used to link styles to the original studio palette styles: the link can be activated or deactivated anytime for any selection of styles. 

|regular-imported-linked_style| 
 
When the link is activated, an arrow is displayed on the small white square, and the style will be updated according to the original studio palette style. When the link is deactivated, the style can be modified regardless of the original studio palette style. 

Linking animation level palettes to the studio palette can assure color consistency for the whole production, because as soon as a change is needed, it can be done in the studio palette automatically updating all the linked animation levels palettes and, consequently, drawings. 

In the level palette, the information about which studio palette the palette styles refers to can be retrieved in the List view mode, where, next to the style thumbnails and names, the path to the source studio palette is displayed. 

When palettes are added to the global studio palette, they are copied to the ``studiopalette``  folder located where OpenToonz projects are stored (see  :ref:`Setting up Projects <setting_up_projects>`  ). 

When palettes are added to the project studio palette, they are copied to the ``+palettes`` folder you specified for the current project (see  :ref:`Project Default Folders <project_default_folders>`  ). 

These folders can be used, for example, to move your studio palette, or the project studio palette, to a different network, or to make a backup copy of it.


.. tip:: **To add an empty palette:**

    1. Select the folder where you want to create the new palette.

    2. Right-click the folder where you want to locate the palette and choose New Palette from the menu that opens.

.. tip:: **To name a palette:**

    Double click its name and type a new name.

.. tip:: **To view a palette in the studio palette:**

    Select it in the palette tree.

.. tip:: **To add a level palette to the studio palette:**

    1. Select the level to display its palette.

    2. Do one of the following:

    - Click the Palette button ( |Toonz71_135| ) in the top bar of the palette editor and drag the current palette to the studio palette folder where you want to locate it. The palette will retain its name.

    - Add an empty palette in the studio palette browser, right-click it and select Replace with Current Palette from the menu that opens.

.. tip:: **To add palettes by searching in a computer folder:**

    1. Select the folder where you want to place palettes retrieved during the search.
    
    2. Right-click the folder and select Search for Palettes from the menu that opens.

    3. Type the full path to the computer folder you want to scan.

.. tip:: **To add a new folder:**

    1. Select the folder where you want to create the new folder.

    2. Right-click the folder where you want to locate your new folder and choose New Folder from the menu that opens.

.. tip:: **To name a folder:**

    Double click its name and type a new name.

.. tip:: **To delete a palette or a folder:**

    1. Select it in the palette tree.

    2. Right-click the palette or the folder you want to delete and choose Delete Palette from the menu that opens.

.. tip:: **To rearrange palettes in the studio palette folders:**

    Click and drag the palette from the current location to the new one.

.. tip:: **To load a palette from the studio palette to the current level palette:**

    Do one of the following:

    - Click and drag the palette, from the studio palette tree to the Palette button ( |Toonz71_139| ) in the top bar of the palette editor.

    - Right-click the palette you want to use and select Load into Current Palette from the menu that opens.

.. note:: In case the palette misses some styles used to paint the level drawings, you will be prompted whether to delete the styles only and show the lines and areas painted with them in red, or to delete the lines and areas painted with them as well.

.. tip:: **To reorder the current palette using a specific studio palette as reference:**

    1. Select the level that uses the palette that has to be modified.

    2. Select into the Studio Palette window the palette you want to use as reference.

    3. Right-click the palette and select Adjust Current Level to This Palette. 

    4. Insert a Tolerance value in the window that opens. 

.. note:: The Tolerance parameter defines the range of RGB values that will be used for matching colors from the curret palette to those of the studio palette. Default value of 0 means no range use, just colors with the same RGB values will be reordered and all the others will be added as new colors.

.. note:: All the colors of the studio palette will be transferred into the current palette, all of this colors will show the Reference to Studio Palette box. The colors that are used in both palettes will be ordered, for positon and color index, as in the reference studio palette. All the colors that are new into the curent palette will be moved after the last transferred color. Pages will be added when required.

.. tip:: **To merge a palette from the studio palette to the current level palette:**

    Do one of the following:

    - Click and drag the palette from the studio palette tree to the level palette.

    - Right-click the palette you want to use and select Merge to Current Palette from the menu that opens.

.. tip:: **To replace a palette from the studio palette with the current palette:**

    1. Select the palette you want modify in the studio palette, or project palette.

    2. Right-click the palette and select Replace with Current Palette.

.. tip:: **To copy styles from the studio palette to the current level palette, and vice versa:**

    1. Select the palette in the studio palette to display it in the palette viewer.

    2. Select the styles you want to copy in one palette.

    3. Ctrl-click (PC) or Cmd-click (Mac) and drag the selection to the other palette.

.. note:: If you drag the selection to the right of the last page tab, a new page will be created containing the dragged styles.

.. tip:: **To activate a style link to the studio palette:**

    1. Select the styles that have been imported from the studio palette.

    2. Right-click the selection and select Toggle Link to Studio Palette from the menu that opens.

.. tip:: **To deactivate a style link to the studio palette:**

    1. Select the styles that have been linked to the studio palette.

    2. Right-click the selection and select Toggle Link to Studio Palette from the menu that opens.

.. tip:: **To remove style reference to the studio palette:**

    1. Select the styles that have a reference to the studio palette.

    2. Right-click the selection and select Remove Reference to Studio Palette from the menu that opens.

.. tip:: **To resize the studio palette sections:**

    Do any of the following:

    - Click and drag the separator to resize sections. 

    - Click and drag the separator towards the window border to hide a section.

    - Click and drag the separator collapsed to the window border toward the window center to display again the hidden section.


.. _animating_palettes:

Animating Palettes
------------------
For Toonz raster and vector levels, colors in a palette can be animated and changed according to the frames of the animation.

The animation is defined by keys that refer to timing of the xsheet: this means that there is no relation between the level length and the length of the animation of the palette colors. For example you can create a palette animated from frame 1 to 100 even if its level is only five frames long.

The color animation will always refer to the xsheet timing, even if you move the related level to a different frame range. For example if you animate a palette from frame 1 to frame 20, and the level is exposed after frame 20, no color animation will be visible and the color used for the level will refer to the last key of the colors animation.

Keys are set for all the palette colors and settings (in the case of Special Styles and Textures) at once and can be navigated directly in the palette (with the expected update of the viewer content) to check the color animation.

.. tip:: **To define a palette key:**

    1. Select in the xsheet the frame where you want to define the key.

    2. Click the key button ( |Toonz71_140| ) in the top bar of the palette editor.

.. tip:: **To check if the palette has a key at a specific frame:**

    Select the frame you want to check: if the key button ( |Toonz71_141| ) in the top bar of the palette editor is blue, the colors have a key at the current frame.

.. tip:: **To navigate the palette keys:**

    Use the Next ( |Toonz71_142| ) and Previous Key buttons ( |Toonz71_143| ) available at the side of the key button in the top bar of the palette editor.

.. tip:: **To remove a palette key:**

    1. Do one of the following to select the frame you want to remove the key from:

    - Select it in the xsheet frame column.

    - Navigate the palette keys.

    2. Click the key button ( |Toonz71_144| ) in the top bar of the palette editor.


.. _editing_styles:

Editing Styles
--------------

Palette styles can be modified with the Style Editor. There are four types of styles to choose from: Color, Texture, Vector and Raster. Generated, Trail and Vector Brushes are available for vector animation levels only. For several types of styles, there is also control over various Settings.

An Auto button lets you decide whether the edits have to be assigned automatically to the style, or only after you click on the Apply button. In the bottom right corner you can see swatches for the previous and new style status; if you want to go back to the previous style, simply click on it. 

Only the first style in the palette, labeled Color 0, cannot be edited: instead, it allows you to remove any style from lines and filled areas.

.. tip:: **To open the style editor as a floating window:**

    Do one of the following:

    - Choose Windows > Style Editor.

    - Double-click the style you want to edit in the palette editor.

.. tip:: **To automatically apply the editing to the style:**

    Activate the Auto button in the style editor.

.. tip:: **To apply manually the editing to the style:**

    1. Deactivate the Auto button in the style editor.

    2. Click the Apply button every time you want to apply the editing to the style.

.. tip:: **To return to the old style cancelling the editing:**

    Click the style swatch in the very bottom right corner of the style editor.


.. _plain_colors:

Colors
''''''

|style_editor_color|

Colors can be defined either by Hue, Saturation and Value or by Red, Green and Blue values. They can be used for both drawing lines and filling areas.

You can also set the color opacity with the Alpha slider: the lower the value, the more transparent the color. You can check the opacity of the color with the checkerboard pattern visible beneath the color, whose visibility is proportional to the color transparency.

To edit a color you can use either the sliders or the color wheel. To pick a color from the sliders or from the wheel, click it; to adjust values you can use the arrowhead buttons available at each slider ends. 

Colors can also be picked from the viewer content by using the RGB Picker tool ( |Toonz71_146| ), whose Type option lets you choose the following: Normal, to pick values of a color; Rectangular, to pick the average values of the colors included in the box you define; Freehand, to pick the average values of the colors included in the area you outline by clicking and dragging; and Polyline, to pick the average values of the colors included in the area you outline by defining a series of lines. 

If the current style is a special one, the color you edit is the color used by the special style. If the special style uses more than one color, you can select the color to edit in the row of thumbnails available below the Auto and Apply buttons. (see  :ref:`Special Styles <special_styles>`  ).

.. tip:: **To pick the color from the viewer content:**

    1. Select the RGB Picker tool ().

    2. Do one of the following:

    - Click in the viewer to pick the needed color values.

    - Set the type to Rectangular, then click and drag in the viewer to define a box which picks the average values of the colors included in the box.

    - Set the type to Freehand, then click and drag in the viewer to outline an area which picks the average values of the colors included in the area.

    - Set the type to Polyline, then click in the viewer to outline an area by defining a series of lines and this will pick the average values of the colors included in the area.


.. _textures:

Textures
''''''''

|style_editor_texture|

Textures can be used both for drawing lines and filling areas. They can be selected from a list available in the Texture page, where your own textures can be added as well, or added as Custom Texture clicking the Custom Texture button.

Vector texture mapping, that is the way the texture is applied to vectors, is performed using vector parametric coordinates: this means that the texture “follows” the vector’s shape and thickness. 

Custom Textures can be loaded both on PLI and TLV levels, but their parameters can be used only on TLV levels.

Lines and areas texture mapping, applied for raster drawing, use the standard mapping: this means that the texture image is tiled to cover the lines or areas painted with the style.

.. note:: A more powerful texture mapping can be performed by using the Texture and Pinned Texture special FX (see  :ref:`Toonz Level <toonz_level>`  ).

.. tip:: **To add a new Texture:**

    1. Create the image you want to use as a texture with the following characteristics:

    - The number of pixels of the width and height of the image has to be equal to 2 to the power of any number (i.e. 2, 4, 8, 16, 32, 64, 128, 256, etc.); if not, texture images will show stretched.

    - The file has to be saved in any of the following formats: TIF, TGA, PNG, BMP, JPG, NOL, RGB and SGI.

    2. Save the texture file in the folder ``Projectroot\library\textures``  (see  :ref:`Setting up Projects <setting_up_projects>`  ).


.. _custom_textures:

Custom Textures
'''''''''''''''
Custom Textures can be used both for drawing lines and filling areas. Using Custom Textures allows to set many parameters such as: Use As Pattern, using the brightness of the loaded image to modulate the brightness of the Color index to which it is applied; choose the position between Fixed (the texture will be fixed and slide into the character), Automatic (the texture will follow the character position during the animation) and Random (the texture position change at each frame in a random way); Scale, Rotation, apply an Horizontal or Vertical offset and change the Contrast. The Custom Texture will be saved into the Palette and its icon will be replaced with an icon of the loaded texture.

.. tip:: **To add a Custom Texture:**

    1. Select a style in the palette editor.

    2. Go in the Texture tab of the Style Editor and press the Custom Texture button.

    3. Go in the Settings tab, use the Load From File field and choose the image (or the image sequence) you want to use as texture.

    4. Press the Preview button to visualize the texture.


.. _special_styles:

Generated Styles
''''''''''''''''

|style_editor_generated|

Generated styles use a number of mathematical functions to create effects that can be used either for vector strokes or for filling areas defined by vectors. They can be selected from a list available in the Generated section of the Vector tab, where styles suitable for vector strokes have a thumbnail representing how they will look as a diagonal line; styles suitable for filling have a thumbnail representing the top right corner piece of an area.

Generated styles can simulate for instance a frieze, a leaf, or a pencil stroke along a vector, or allow you to fill areas with special effects such as polka dots.

Generated styles can be customized by defining the parameters available in the Settings tab. This allows you to have many similar styles, each with a different configuration of settings.

Colors used by generated styles can be modified by using the Color tab available in the Style Editor.

The first item available in the list allows you to remove the Generated style, in order to return it to a Color style. 

.. tip:: **To change colors used by a generated style:**

    1. Move to the Color tab in the Style Editor.

    2. Edit the color using the wheel and sliders.

    3. If the generated style uses more than one color, select the color to edit in the row of swatches available below the Auto and Apply buttons. 


.. _custom_styles:

Trail Styles
''''''''''''

|style_editor_trail|

Trail styles are available for vector levels only. A trail style repeats an image or an animation level, created with OpenToonz or third party software, along the vectors of a vector level. Trail styles cannot be used to paint areas.

In the Trail section on the Vector tab you can select the image or the animation level you want to use as a style. You can add to the list your own animation levels as well: both OpenToonz animation levels (PLI) and full-color images or sequences of full-color images (BMP, JPG, NOL, PIC, PICT, PCT, PNG, RGB, SGI, TGA, TIF and TIFF) are supported.

.. note:: PLI levels are rendered according to the vector length and thickness, thus appearing jagged when zoomed in. If the output format is a vector one, then the PLI level will remain vector-based. (see  :ref:`Choosing the Output Settings <choosing_the_output_settings>`  ).

The images are repeated changing their placement and size according to the vector’s shape and thickness. If the animation levels contains different drawings, they are repeated cyclically along the vector length. 

Parameters such as the distance between subsequent images along the vector and their rotation can be defined in the Settings tab (see  :ref:`Settings <settings>`  ).

.. tip:: **To add a new custom style:**

    1. Create an image or an animation level with OpenToonz, or with third-party software.

    2. Save it in the folder ``Projectroot\library\custom styles`` (see  :ref:`Setting up Projects <setting_up_projects>`  ). 


.. _vector_brush:

Vector Brush Styles
'''''''''''''''''''

|style_editor_vectorbrush|

Vector brush styles are available for vector levels only. A vector brush applies a vector image, created with OpenToonz, along the vector strokes of a vector level. Vector brush styles cannot be used to paint areas.

In the Vector Brush section of the Vector tab, you can select the image you want to use as a style. You can add to the list your own PLI images as well.

.. note:: PLI levels are rendered according to the vector length and thickness, thus appearing jagged when zoomed in. If the output format is a vector one, then the PLI level will remain vector-based. (see  :ref:`Choosing the Output Settings <choosing_the_output_settings>`  ).

The Vector Brush image is applyed to each stroke of the drawing that use this style according to the stroke’s shape and thickness. If the animation levels used as vector Brush contains different drawings, only the first one will be taken into account.

Colors used by vector brushes can be modified by using the Color tab available in the style editor.

The first item available in the list allows you to remove the Vector Brush in order to return it to a Color style. 

.. tip:: **To add a new vector brush:**

    1. Create a PLI level with OpenToonz.

    2. Save it in the folder ``Projectroot\library\vector brushes`` (see  :ref:`Setting up Projects <setting_up_projects>`  ). 

.. tip:: **To change colors used by a vector brush style:**

    1. Move to the Color tab in the Style Editor.

    2. Edit the color using the wheel and sliders.

    3. If the vector brush uses more than one color, select the color to edit in the row of swatches available below the Auto and Apply buttons. 


.. _settings:

Settings
''''''''

|style_editor_settings|

The Settings tab is available for defining some color properties. 

For Toonz raster levels, it contains only the Autopaint for Lines option, that can be used to automatically paint border lines of an area, with the same color used to fill that area (see  :ref:`Using the Autopaint for Lines Option <using_the_autopaint_for_lines_option>`  ).

For Toonz vector levels, it contains parameters only when the style is a generated or trail one. 

When the style is a generated one, the Settings tab contains one or more sliders that allow you to finetune the predefined style to your needs. When the style is a trail one, the Settings tab contains two sliders: the Distance sets the space between two subsequent images of the animation level used as a trail; the Rotation sets the angle of all the images. 

 |Toonz71_152| 

You can add the same generated or trail style as many times as you want, each time defining different settings for it.


.. _changing_the_type_of_style:

Changing the Type of Style
''''''''''''''''''''''''''
When you select color, texture, generated, trail or vector brush in the style editor, you automatically assign it to the current style, thus changing the type of style.

The only exception is when you want to change from a generated or a vector brush style to a color one, because when the current style is a generated or a vector brush one, the Color tab is used for setting its colors. In this case you have first to remove the generated or vector brush style by using the first swatch available in the swatch list, and then move to the Color tab.

Note that when you change from a style suitable for both lines and areas to a style suitable only for lines, areas painted with that style will become invisible, and vice versa. For example if you change a style from color to trail, all areas painted with that color will become invisible. If you modify the style so that it is suitable again for lines and areas, the invisible parts will become visible again. 

.. tip:: **To change the type of style from color to any other:**

    Choose an item in the texture or vector tabs.

.. tip:: **To change the type of style back to color:**

    Choose the Color tab and start moving a slider or the selector in the color wheel.

.. tip:: **To change the type of style from generated or vector brush back to color:**

    1. In the Generated or Vector Brush sections of the Vector tab select the first style in the list (the top-left most style) to assign no special style to the current color.

    2. Choose the Color tab and start moving a slider or the selector in the color wheel.


.. _editing_several_styles_at_the_same_time:

Editing Several Styles at the Same Time
'''''''''''''''''''''''''''''''''''''''

|palette_gizmo|

You can modify several styles at the same time by using the Palette Gizmo. It allows you to scale or shift the value, saturation, hue and alpha of the selected styles, blend them, or fade them to a specific color.

.. note:: Only the color styles are affected by the Palette Gizmo editing and the blending. e.g. generated and trail styles will not be affected.

.. tip:: **To open the Palette Gizmo:**

    Right-click the selected styles and choose Palette Gizmo from the menu that opens.

.. tip:: **To change the value of the selected styles:**

    1. Set the percentage of variation or the shift magnitude you want to apply to the styles value.

    2. Do one of the following:

    - Click the + button to increase the value on the set percentage or shift magnitude.

    - Click the - button to decrease the value on the set percentage or shift magnitude.

.. tip:: **To change the saturation of the selected styles:**

    1. Set the percentage of variation or the shift magnitude you want to apply to the styles saturation.

    2. Do one of the following:

    - Click the + button to increase the saturation on the set percentage or shift magnitude.

    - Click the - button to decrease the saturation on the set percentage or shift magnitude.

.. tip:: **To change the hue of the selected styles:**

    1. Set the shift magnitude you want to apply to the styles hue.

    2. Do one of the following:

    - Click the + button to increase the hue on the set shift magnitude.

    - Click the - button to decrease the hue on the set shift magnitude.
    
.. tip:: **To change the alpha of the selected styles:**

    1. Set the percentage of variation or the shift magnitude you want to apply to the styles alpha.

    2. Do one of the following:

    - Click the + button to increase the alpha on the set percentage or shift magnitude.

    - Click the - button to decrease the alpha on the set percentage or shift magnitude.

.. tip:: **To blend selected styles:**

    1. Select a set of styles in the palette editor.
    
    2. Click the Blend button: style colors will be blended from the first to the last color of the selected styles.

.. tip:: **To fade the selected styles to a specific color:**

    1. Choose the color you want to fade the selection to by doing one of the following:

    - Set the Red, Green and Blue values.

    - Click the color thumbnail and use the Style Editor to edit it (see  :ref:`Plain Colors <plain_colors>`  ).

    2. Set the percentage of the fading you want to apply to the styles.

    3. Click the Fade button to fade styles to the set color, according to the set percentage.


.. |palette| image:: /_static/palettes_styles/palette.png
.. |studio_palette| image:: /_static/palettes_styles/studio_palette.png
.. |regular-imported-linked_style| image:: /_static/palettes_styles/regular-imported-linked_style.png
.. |style_editor_color| image:: /_static/palettes_styles/style_editor_color.png
.. |style_editor_texture| image:: /_static/palettes_styles/style_editor_texture.png
.. |style_editor_generated| image:: /_static/palettes_styles/style_editor_generated.png
.. |style_editor_trail| image:: /_static/palettes_styles/style_editor_trail.png
.. |style_editor_vectorbrush| image:: /_static/palettes_styles/style_editor_vectorbrush.png
.. |style_editor_raster| image:: /_static/palettes_styles/style_editor_raster.png
.. |style_editor_settings| image:: /_static/palettes_styles/style_editor_settings.png
.. |palette_gizmo| image:: /_static/palettes_styles/palette_gizmo.png

.. |Toonz71_127| image:: /_static/Toonz71/Toonz71_127.gif
.. |Toonz71_128| image:: /_static/Toonz71/Toonz71_128.gif
.. |Toonz71_130| image:: /_static/Toonz71/Toonz71_130.gif
.. |Toonz71_131| image:: /_static/Toonz71/Toonz71_131.gif
.. |Toonz71_132| image:: /_static/Toonz71/Toonz71_132.gif
.. |Toonz71_133| image:: /_static/Toonz71/Toonz71_133.gif
.. |Toonz71_134| image:: /_static/Toonz71/Toonz71_134.gif
.. |Toonz71_135| image:: /_static/Toonz71/Toonz71_135.gif
.. |Toonz71_136| image:: /_static/Toonz71/Toonz71_136.gif
.. |Toonz71_137| image:: /_static/Toonz71/Toonz71_137.gif
.. |Toonz71_138| image:: /_static/Toonz71/Toonz71_138.gif
.. |Toonz71_139| image:: /_static/Toonz71/Toonz71_139.gif
.. |Toonz71_140| image:: /_static/Toonz71/Toonz71_140.gif
.. |Toonz71_141| image:: /_static/Toonz71/Toonz71_141.gif
.. |Toonz71_142| image:: /_static/Toonz71/Toonz71_142.gif
.. |Toonz71_143| image:: /_static/Toonz71/Toonz71_143.gif
.. |Toonz71_144| image:: /_static/Toonz71/Toonz71_144.gif
.. |Toonz71_145| image:: /_static/Toonz71/Toonz71_145.gif
.. |Toonz71_146| image:: /_static/Toonz71/Toonz71_146.gif
.. |Toonz71_148| image:: /_static/Toonz71/Toonz71_148.gif
.. |Toonz71_149| image:: /_static/Toonz71/Toonz71_149.gif
.. |Toonz71_150| image:: /_static/Toonz71/Toonz71_150.gif
.. |Toonz71_151| image:: /_static/Toonz71/Toonz71_151.gif
.. |Toonz71_152| image:: /_static/Toonz71/Toonz71_152.gif
.. |Toonz71_154| image:: /_static/Toonz71/Toonz71_154.gif
