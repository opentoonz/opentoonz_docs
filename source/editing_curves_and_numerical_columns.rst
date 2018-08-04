.. _editing_curves_and_numerical_columns:

Editing Curves and Numerical Columns
====================================
Object and FX transformations are mapped in the function editor window, where set key values and related interpolations can be controlled and modified by using function curves or numerical columns.

Function curves display transformations as graphical curves in a graph, where frames are laid horizontally and values are laid vertically. 

Numerical columns display transformations in columns, like the ones available in xsheet, where for each frame the related transformation values are displayed.

Curves and columns are different representations of the same transformation, so any change made in one mode is reflected in the other one as well.

.. _using_the_function_editor:

Using the Function Editor
-------------------------

|function_editor_1|

The function editor window is divided into three sections. On the left there is an area where the numerical columns or curves are displayed, on the right top an area where the interpolation of the current transformation segment is displayed, and on the right bottom there is the objects/FX tree.

The tree has two main items, Stage and FX: in the first you can find folders for the defined cameras, the table, used pegbars and columns; in the second one you can find folders for each used effect. Each folder contains the related transformation parameters.

The objects/FX tree tells if the object/effect is animated and which parameter is animated, by using the following icons:

- A plain folder is for non-animated objects/FX.

- A folder with an arrow is for animated objects/FX.

- An icon with a dotted straight line is for non-animated parameters.

- An icon with a continuos curve is for animated parameters.

Clicking these icons allows you to select which object/effect and which parameters have to be displayed as curves or numerical column in the area on the right.

Transformation data can be saved and loaded as a CURVE file, to allow the exporting and importing from one scene to another, and they can be exported as well as a DAT file in order to be used in other software.

.. tip:: **To resize the function editor sections:**

    Do any of the following:

    - Click and drag the separators to resize sections. 

    - Click and drag a separator toward the window border to hide a section.

    - Click and drag the separator collapsed to the window border toward the window center to display again the hidden section.

.. tip:: **To display or hide a function curve or a numerical column:**

    1. Retrieve the object or the effect in the objects/FX tree.

    2. Do one of the following:

    - Click the folder to display or hide all curves or columns related to its parameters.

    - Click the parameter icon to display or hide its related curve or column.

    - Click a parameter icon and drag to display or hide all the curves or columns you pass upon.

    - Right-click the folder and choose Show Animated Only from the menu that opens to display or hide only the animated curves or columns related to its parameters.

    - Right-click the folder and choose Show All from the menu that opens to display or hide all curves or columns related to its parameters.

.. tip:: **To switch between curves and columns view:**

    Click the Function Editor Toggle button ( |Toonz71_520| ) in the bottom bar of the area where curves or column are displayed.



.. tip:: **To navigate the curve viewer:**

    Do one of the following:

    - Use the mouse wheel, or the zoom shortcut keys (by default + and - keys) to zoom in and zoom out.

    - Click in the horizontal ruler and drag up to zoom in horizontally, down to zoom out; click in the value vertical ruler and drag up to zoom in vertically, down to zoom out.

    - Middle-click and drag the graph area to scroll in any direction, the horizontal ruler to scroll horizontally, and the vertical ruler to scroll vertically.

    - Use the reset view shortcut (by default the 0 key) or right-click the graph area and choose Fit from the menu that opens, to display all the visible curves in the actual function editor window.

.. tip:: **To scroll the numerical columns:**

    Do one of the following:

    - Middle-click and drag to scroll in any direction.

    - Use the mouse wheel to scroll up or down.

    - Use the scrolling bars to scroll only within the actual numerical columns extent.

    - Use the Up Arrow and Down Arrow keys to move one frame up or down.

    - Use the Page Up and Page Down keys to scroll the visible frames up or down.

    - Use the Home and End keys to scroll up to the beginning or the end of the xsheet content.

.. tip:: **To save transformation data:**

    1. Right-click the relevant parameter in the objects/FX tree, and choose Save Curve from the menu that opens.

    2. Use the browser to choose a name and location for the file to be saved: the data will be saved as a CURVE file.

.. tip:: **To load transformation data:**

    1. Right-click the relevant parameter in the objects/FX tree, and choose Load Curve from the menu that opens.

    2. Use the browser to retrieve the curve to load; valid files are in CURVE format.

.. tip:: **To export transformation data:**

    1. Right-click the relevant parameter in the objects and FX tree, and choose Export Data from the menu that opens. 

    2. Use the browser to choose a name and location for the file to be saved: the data will be saved as a DAT file that can be used in other software supporting this type of information.

.. _defining_key_values:

Defining Key Values
-------------------
Key values, including those defined for object transformations with the Edit tool ( |Toonz71_521| ) and those defined for FX parameters in the FX Settings window, can be controlled and edited both using function curves and numerical columns (see 

:ref:`Animating Objects <animating_objects>`  and 

:ref:`Editing FX Settings <editing_fx_settings>`  ). 



In function curves, key values are represented as control points along the curve; in numerical columns they are displayed in specific cells. In both cases they can be added, edited, moved and deleted.

.. _using_function_curves:

Using Function Curves
'''''''''''''''''''''
Function curves display transformations as graphical curves in a graph where frames are laid horizontally, and values are laid vertically. 

Curves are defined by control points representing key values. Points can be easily added by working directly in the graph or using the Set Key button ( |Toonz71_522| ) in the bottom bar of the window. 






Control points can also be selected in order to be edited, moved or deleted. 

The Set Key button ( |Toonz71_524| ) is either grey when no key value is defined for the current curve at the current frame, or blue when a key value is defined for the current curve at the current frame.



Frames and key values can be navigated by using the related buttons in the bottom bar of the window. The Next ( |Toonz71_525| ) and Previous Key buttons (

 |Toonz71_526| ) are available only if more than one key value is defined. 



.. tip:: **To set the current curve:**

    Do one of the following:

    - Click the related parameter name in the objects/FX tree.

    - Display the curve in the function editor, then click to select it.

.. tip:: **To set the current frame:**

    Do one of the following:

    - Click in the frame horizontal ruler to set a position for the current frame marker.

    - Click and drag the current frame marker in a horizontal direction.

    - Type the frame number in the Frame text box, or use the Next and Previous Frame buttons available in the bottom bar of the window.

    - Move the current frame cursor in the xsheet.

    - Use the frame bar or the playback buttons in the bottom bar of the work area.

.. tip:: **To add a key point:**

    Do one of the following:

    - Click the Set Key button ( |Toonz71_527| ) to add a key point at the current frame.



    - Type a value in the Value text box to add a key point at the current frame.

    - Right-click and choose Set Key from the menu that opens.

    - Ctrl-click (PC) or Cmd-click (Mac) the curve where you want to add the key point.

.. tip:: **To remove a key point:**

    Do one of the following:

    - Select the key point to remove and choose Edit > Delete.

    - Set the current frame where a key point is and click the Set Key button ( |Toonz71_528| ).



.. tip:: **To select key points:**

    Do one of the following:

    - Click to select a key point.

    - Shift-click to add a key point to or remove it from the selection.

    - Click and drag to select all of the key points that are in the area you define.

.. tip:: **To select curve segments:**

    Select the control points at the ends of the segment.

.. tip:: **To move the selection:**

    Click and drag any of the selected control points.

.. tip:: **To edit curves:**

    Do one of the following:

    - Use the Copy command: the selected segments will be kept in memory for further operations.

    - Use the Cut command: the selected segments will be eliminated from the curve and will be kept in memory for further operations.

    - Use the Paste command: the segments kept in memory will be pasted starting from the selected key point, preserving any other previously defined key point not replaced by the new ones.

    - Use the Delete command: the selection will be deleted.

.. tip:: **To navigate key points for the current curve:**

    Use the Next ( |Toonz71_529| ) and Previous Key buttons (

 |Toonz71_530| ) available at the side of the Set Key button.



.. tip:: **To cycle previously created key points:**

    Right-click the curve and choose Activate Cycle from the menu that opens.

.. tip:: **To disable the cycle:**

    Right-click the curve and choose Deactivate Cycle from the menu that opens.

.. _using_numerical_columns:

Using Numerical Columns
'''''''''''''''''''''''
Numerical columns display transformations in columns like the ones available in xsheet, having one for each parameter. For each frame the column cells display the related transformation values, that can be edited as in a spreadsheet.

Key values are displayed in different-colored cells, and can be moved along the column to different frame positions. In-between values are automatically generated according to the key values and to the set interpolation (see  :ref:`Setting Segment Interpolations <setting_segment_interpolations>`  ).

All the columns referring to the same object or FX are grouped under one single header. For example under a pegbar header you can find all the columns referring to its transformations. 

Columns cells can be used to type in directly values for keys, edit or move them. Values contained in cells can be cut, copied and pasted, so that transformations can be displaced, repeated and deleted. 




.. tip:: **To define key values directly in the transformation columns:**

    1. Double click in the column cell where you want to define a key value: the cell becomes editable.

    2. Type in the value for the key, and press Enter to confirm.

.. tip:: **To move a key value:**

    Click the dark vertical strip at the left of a key value cell, and drag it up or down to the new position; the in-between values change accordingly.

.. tip:: **To displace the channel along the column:**

    Click the dark vertical strip at the left of column cells, and drag it up or down to the new position: the whole content moves along the column.

.. tip:: **To copy/cut and paste column values:**

    Do one of the following:

    - Click and drag to perform a selection; the selection can be extended to several columns.

    - Use the Copy command: the selection will be kept in memory for further operations.

    - Use the Cut command: the selection will be eliminated from the columns and will be kept in memory for further operations. The cells elimination causes the following cells to shift up.

    - Use the Paste command: the selection kept in memory will be pasted starting from the selected insertion cell. The command causes the following cells to shift down.

    - Use the Delete command: selected cells will be deleted, causing the following cells to shift up.

.. note:: All the Edit menu commands are also available in the menu that opens when right-clicking in the xsheet cells.

.. note:: Only key values included in the selection are considered when performing copy, cut and paste operations.

.. _setting_segment_interpolations:

Setting Segment Interpolations
------------------------------
A transformation segment, that is to say the section between two key values, can have different interpolations affecting the way the value changes from one key to another. The set interpolation will be displayed graphically in the function curves, and as a series of values, one for each frame, in the numerical columns.

Available interpolations are the following: linear, speed in / speed out, ease in / ease out, ease in / ease out %, exponential, expression-based, file-based, constant and similar-shape-based. The default interpolation can be set in the Preferences > Animation dialog by choosing among linear, speed in / speed out, ease in / ease and out, ease in / ease out %, but the interpolation can be changed at any time in the interpolation area of the function editor, on the bottom right of the window.

In the same area it is also possible to define an interpolation step, that is to say the number of frames for which the interpolation values have to be repeated, for instance to match a movement with an animation level exposed at a specific step. The default animation step can be set in the Preferences > Animation dialog.

.. tip:: **To set the type of interpolation for a segment in the function curves:**

    1. Set the segment by doing one of the following:

    - Click a segment to select it.

    - Move the current frame marker to a frame belonging to a segment.

    2. Choose the interpolation from the option menu available in the interpolation area of the function editor.

.. note:: The interpolation options are also available when right-clicking a segment.

.. tip:: **To set the type of interpolation for a segment in the numerical columns:**

    1. Move the current frame cursor to a frame belonging to a segment.

    2. Choose the interpolation from the option menu available in the interpolation area of the function editor.

.. tip:: **To set the step of the interpolation:**

    Specify the Step value in the interpolation area of the function editor.

.. _using_linear_interpolations:

Using Linear Interpolations
'''''''''''''''''''''''''''
When the interpolation is linear the curve segment turns to a straight line and the speed of the transformation is constant.

.. tip:: **To set a linear interpolation:**

    Do one of the following:

    - Choose Linear from the option menu available in the interpolation area of the function editor.

    - Right-click the curve you want to set the interpolation for, and choose Linear Interpolation from the menu that opens.

.. _using_speed_in_/_speed_out_interpolations:

Using Speed In / Speed Out Interpolations
'''''''''''''''''''''''''''''''''''''''''
When the interpolation is speed in / speed out, both control points at the ends of the segment have handles whose direction and length define the slope of the curve, therefore the speed of the transformation. The handles direction and length can be set by entering values in the interpolation area of the function editor, or by dragging the handles themselves.

By default the handles are linked, making their degree of movement dependent on adjacent segments in order to define a smooth curve, but the link can be broken in order to move the handle freely. For example if subsequent segments have the speed in / speed out interpolation, the handles of the shared points share the same direction, but breaking the link each handle can have a different direction. 

Handles can also be collapsed in control points in order to turn them into corner points; in this case to retrieve the handles it is possible to reset their length and direction.

.. tip:: **To set a speed in / speed out interpolation:**

    Do one of the following:

    - Choose Speed In / Speed Out from the option menu available in the interpolation area of the function editor.

    - Right-click the curve you want to set the interpolation for, and choose Speed In / Speed Out Interpolation from the menu that opens.

.. tip:: **To set the speed of the interpolation:**

    1. Select the key point at the beginning or at the end of the curve segment you want to edit, or the curve segment itself.

    2. Set the slope of the curve after or before the key point by doing one of the following:

    - Enter the Speed In and Speed Out direction and length values in the interpolation area of the function editor.

    - Click and drag the end of the handles to move them freely.

    - Shift-click and drag the end of the handles to move them with a constraint in the horizontal or vertical direction.

.. tip:: **To move a control point handle free from the adjacent segments:**

    Right-click the control point and choose Unlink Handles from the menu that opens.

.. tip:: **To link back handles to adjacent segments:**

    Right-click the control point and choose Link Handles from the menu that opens.

.. tip:: **To turn a control point into a corner point:**

    1. Select the control point.

    2. Move the handle ends to the control point, in order to collapse them.

.. tip:: **To retrieve handles from a corner point:**

    Right-click the control point and choose Reset Handles from the menu that opens.

.. _using_ease_in_/_ease_out_interpolations:

Using Ease In / Ease Out Interpolations
'''''''''''''''''''''''''''''''''''''''
When the interpolation is ease in / ease out, the segment is divided into three sections by two vertical lines: the first section is an acceleration, the second is at constant speed, the third is a deceleration. The duration in frames of each section can be set by entering values in the interpolation area of the function editor, or by dragging the vertical lines available on the segment.

.. tip:: **To set an ease in / ease out interpolation:**

    Do one of the following:

    - Choose Ease In / Ease Out from the option menu available in the interpolation area of the function editor.

    - Right-click the curve you want to set the transformation for, and choose Ease In / Ease Out Interpolation from the menu that opens.

.. tip:: **To set the ease in / ease out of the interpolation:**

    1. Select the key point before or after the ease in / ease out curve segment you want to edit, or the curve segment itself.

    2. Do one of the following:

    - Enter the Ease In and Ease Out values in the interpolation area of the function editor.

    - Move the vertical line setting the ease in or ease out section of the segment, to change the curve after or before the key point.

.. _using_ease_in_/_ease_out_%_interpolations:

Using Ease In / Ease Out % Interpolations
'''''''''''''''''''''''''''''''''''''''''
The ease in / ease out % interpolation is similar to the ease in / ease out one, but the ease in and ease out sections of the segments are expressed as a percentage of the segment frame duration.

.. tip:: **To set an ease in / ease out % interpolation:**

    Do one of the following:

    - Choose Ease In / Ease Out % from the option menu available in the interpolation area of the function editor.

    - Right-click the curve you want to set the transformation for, and choose Ease In / Ease Out % Interpolation from the menu that opens.

.. tip:: **To set the ease in / ease out % of the interpolation:**

    1. Select the key point before or after the ease in / ease out curve segment you want to edit, or the curve segment itself.

    2. Do one of the following:

    - Enter the Ease In and Ease Out values in the interpolation area of the function editor.

    - Move the vertical line setting the ease in or ease out section of the curve segment, to change the curve after or before the key point.

.. _using_exponential_interpolations:

Using Exponential Interpolations
''''''''''''''''''''''''''''''''
When the interpolation is exponential the curve segment turns to a a curve that continually becomes steeper, because the higher the frame, the faster the related value grows. Only positive values are significant for this interpolation.

.. tip:: **To set an exponential interpolation:**

    Do one of the following:

    - Choose Exponential from the option menu available in the interpolation area of the function editor.

    - Right-click the curve you want to set the transformation for, and choose Exponential Interpolation from the menu that opens.

.. _using_interpolations_based_on_expressions:

Using Interpolations Based on Expressions
'''''''''''''''''''''''''''''''''''''''''
When the interpolation is defined by an expression, the segment values come from a mathematical formula that can be typed by using algebra notations. In this case the key values at the end of the segment may change values as well according to the typed expression.

While typing the expression, if the syntax is recognized, a menu automatically opens suggesting you the possible terms: from the menu you can select the term both to display in a tooltip box its correct syntax, and to insert it in the expression.

As soon as terms are recognized, different colors are used to highlight them: operators and functions are displayed in dark blue, variables in light blue, constants in green. When the expression is entered any syntax error will be displayed in red.

The unit used for the function is displayed in a box next to the expression; in case the unit refers to a movement, the default unit can be changed, and the values will be automatically converted to the default one.

Apart from the standard operators and functions, some variables and predefined functions can also be used in expressions. 

Supported terms are the following:

===============================  ==============================================================================  
**Operators**                                                                                                    
===============================  ==============================================================================  
``+`` ,`` -`` ,`` *`` ,`` /``                                                                                    
``%``                            Modulus: ``10%6=4`` .                                                           
``^``                            Exponentiation: ``a^2``  means ``a*a`` ; ``a^0.5``  is square root of ``a`` .   
===============================  ==============================================================================  



==========================================  ==========================================================================================================================================================================================  ========================================================================================================================================  
**Functions**                                                                                                                                                                                                                           
==========================================  ==========================================================================================================================================================================================  ========================================================================================================================================  
``sin(), cos(), tan(), atan(), atan2()``    Angles are expressed in degrees.                                                                                                                                                            
``sinh()`` ,`` cosh()`` ,`` tanh()``        Hyperbolic functions.                                                                                                                                                                       
``log()`` ,`` exp()``                                                                                                                                                                                                                   
``floor(value)``                            The greatest whole number less or equal than ``value`` .                                                                                                                                    
``ceiling(value)``                          The smallest whole number less or equal than ``value`` .                                                                                                                                    
``round(value)``                            The integer closest to ``value`` .                                                                                                                                                          
``abs()``                                   Absolute value: ``abs(a)``  is ``a``  without the sign.                                                                                                                                     
``sign(value)``                             Returns 0 if ``value``  is 0; -1 if negative; 1 if positive.                                                                                                                                
``sqrt(value)``                             Returns square root of ``value`` .                                                                                                                                                          
``min(a,b,c,...)``                          Returns argument with minimum value.                                                                                                                                                        
``max(a,b,c,...)``                          Returns argument with maximum value.                                                                                                                                                        
``clamp(value,min,max)``                    ``crop(value,min,max)``                                                                                                                                                                     Returns ``min``  if ``value``  is less than ``min`` ; ``max``  if ``value``  is greater than ``max`` ; otherwise it returns ``value`` .   
``step(value,min)``                         Returns 0 if ``value``  is less than ``min`` , otherwise it returns 1.                                                                                                                      
``smoothstep(value,min,max)``               Returns 0 if ``value``  is less than ``min`` , 1 if ``value``  is greater than or equal to ``max`` , and perform a smooth interpolation between 0 and 1 in interval ``min``  to ``max`` .   
==========================================  ==========================================================================================================================================================================================  ========================================================================================================================================  



======================  ===============  
**Logical Operators**                    
======================  ===============  
``<``                   Less             
``<=``                  Less or equal.   
``>``                   More             
``>=``                  More or equal.   
``==``                  Equal.           
``!=``                  Not equal.       
======================  ===============  



======================  =====  
**Boolean Operators**          
======================  =====  
``&&``                  And.   
``||``                  Or.    
``!``                   Not.   
======================  =====  



========================================  ==============================================================================================  
**Conditional Expression**                                                                                                                
========================================  ==============================================================================================  
``(logical_expression)?value1:value2``    If ``logical_expression``  is true, it returns ``value1`` , otherwise it returns ``value2`` .   
========================================  ==============================================================================================  



====================  ==============================================================================================  
**Variables**                                                                                                         
====================  ==============================================================================================  
``t``                 Ranges from 0.0 to 1.0 along the transition allowing position/lenght-independent transitions.   
``f`` ,`` frame``     The current frame number.                                                                       
``r`` ,`` rframe``    It is relative to the transition.                                                               
====================  ==============================================================================================  



=================  ================  
**Constants**                        
=================  ================  
``pi``             3.141593...       
numeric constant   E.g. 1, 2, 4.3.   
=================  ================  



===============================================================================================  ==========================================================================================================================================================================  
**Predefined Functions**                                                                                                                                                                                                                                                     
===============================================================================================  ==========================================================================================================================================================================  
``cycle(period)``                                                                                Cycles the transition of the ``period``  previous frames.                                                                                                                   
``pulse(pos)`` , ``bump(pos)`` , ``pulse(pos,length)`` , ``bump(pos,length)``                    Generates a bump ranging from 0.0 to 1.0 set at position ``pos`` , with a different breadth depending on the ``length``  of the bump itself.                                
``random``                                                                                       Generates random sequences between 0.0 and 1.0.                                                                                                                             
``random(max)``                                                                                  Generates a random number between 0.0 and ``max`` .                                                                                                                         
``random(min,max)``                                                                              Generates a random number between ``min``  and ``max`` .                                                                                                                    
``random_s(seed)``                                                                               Works like random, but allows the user to specify the ``seed``  to modify the value of the ``random``  function.                                                            
``random_s(seed,max)``                                                                           Like above, with ``max``  as the maximum value of the transition.                                                                                                           
``random_s(seeed,min,max)``                                                                      Like above, with ``min``  and ``max``  as the minimum and maximum values of the transition.                                                                                 
``saw(length)`` , ``saw(length,height)`` , ``sawtooth(length)`` ,`` sawtooth(length,height)``    Generates a periodic sawtooth shaped curve according to the ``length``  and ``height``  values; if ``height``  is not expressed it is assumed to be equal to ``length`` .   
``wave(length)``                                                                                 The same as ``sin(f*2*pi/length)`` .                                                                                                                                        
===============================================================================================  ==========================================================================================================================================================================  



.. note:: The predefined function ``saw`` , ``wave``  and ``pulse``  use implicitly a variable independent from the frame number. You can provide explicitly a variable using the form: fun (var; argument...).

.. tip:: **To set an interpolation based on an expression:**

    Do one of the following:

    - Choose Expression from the option menu available in the interpolation area of the function editor.

    - Right-click the curve you want to set the transformation for, and choose Expression Interpolation from the menu that opens.

.. tip:: **To set the expression:**

    1. Type the expression in the interpolation area of the function editor. As you type, if the syntax is recognized, a menu automatically opens suggesting you the possible terms.

    2. Press Enter to submit the expression and check its syntax.

    3. If the expression refers to a movement, change the unit if needed.

.. tip:: **To select a suggested term:**

    Do one of the following:

    - Use the Up Arrow and Down Arrow keys to select the term in the menu that opens, then press Enter.

    - Click the term in the menu that opens.

.. note:: When selecting a term with the Arrow keys a tooltip box displays the term correct syntax.

.. _using_transformation_references:

Using Transformation References
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
It is possible to use in expressions references to any object or effect transformation. In this way expressions can be used to create some relationships between different transformations belonging to different items that can be both objects or FX.

The syntax to create a reference to an object transformation is the following:

``object.transformation`` 

where ``object``  is the ID name of a camera, column, pegbar or the table, as can be read in the stage and FX schematic nodes tooltips, and ``transformation``  any of the available transformation.

For example ``camera1.ns``  refers to the N/S position of the Camera1.

Supported terms are the following:

=========================  =============================  
**Objects**                                               
=========================  =============================  
``camn`` ,`` cameran``     Refer to the camera ``n`` .    
``coln``                   Refers to the column ``n`` .   
``pegn`` , ``pegbarn`` ,   Refer to pegbar ``n`` .        
``tab`` , ``table``        Refer to the table.            
=========================  =============================  



=====================================  ======================================================  
**Transformations**                                                                            
=====================================  ======================================================  
``ns`` , ``ew``                        Refer to the vertical and horizontal position.          
``path`` , ``pos``                     Refer to the position along the motion path.            
``rot``                                Refers to the rotation.                                 
``scale`` , ``scaleh`` , ``scalev``    Refer to the global, horizontal and vertical scaling.   
``shearh`` , ``shearv``                Refer to the horizontal and vertical shear.             
``z``                                  Refers to the position along the z axis.                
=====================================  ======================================================  



The syntax to create a reference to an effect transformation is the following:

``fx.name.setting`` 

where ``name``  is the ID name of a special effect, as can be read in the FX schematic nodes tooltips, and ``setting``  any of the available effect settings. 

When an effect setting has multiple sub-settings, for example the center settings has X and Y sub-settings, the syntax has to be the following:

``fx.name.setting.subsetting`` 

where ``name``  can be any used effect, ``setting``  the main effect setting, and ``subsetting``  is the effect sub-setting.

For example ``fx.blur2.value``  refers to the Value setting of the effect Blur2; ``fx.raylit1.center.x``  refers to the X setting of the Center of the effect Raylit1.

.. note:: If the effect setting name consists of several words, they have to be typed in expressions without blank spaces.

.. _using_interpolations_based_on_file_data:

Using Interpolations Based on File Data
'''''''''''''''''''''''''''''''''''''''
When an interpolation is based on file data, the segment values are retrieved from the file content. In this case the key values at the end of the segment may change values as well according to the file data.

The file can be created by an external device or other applications, such as motion-control camera or 3D software; supported file formats are BAT, DAT, RTF and TXT.

The value for each frame is taken from the file content, that must consist of a series of numbers listed in several lines. 

In case the file contains several values in each line, it is possible to define which value in each line has to be used by specifying a column number. For example, if you have a file like this:

100, 200, 300

101, 201, 301

102, 202, 302

the value 2 will cause 200, 201, 202 to be loaded.

The unit used for the data is displayed in a box next to the file path; in case the unit refers to a movement, the default unit can be changed, and the values will be automatically converted to the default one.

.. tip:: **To set an interpolation based on file data:**

    Do one of the following:

    - Choose File from the option menu available in the interpolation area of the function editor.

    - Right-click the curve you want to set the transformation for, and choose File Interpolation from the menu that opens.

.. tip:: **To set the file information:**

    1. Type in the File Path field, or use the browser button, to set the path to the data file.

    2. Specify which value in each line has to be used by specifying the Column number.

    3. If the expression refers to a movement, change the unit if needed.

.. note:: If in the browser you choose any project default folder, in the path field the full path will be replace by the related default folder alias (see  :ref:`Project Default Folders <project_default_folders>`  ).

.. _using_constant_interpolations:

Using Constant Interpolations
'''''''''''''''''''''''''''''
When an interpolation is constant, the segment values are always equal to the value of the first key defining the segment.

.. tip:: **To set a constant interpolation:**

    Do one of the following:

    - Choose Constant from the option menu available in the interpolation area of the function editor.

    - Right-click the curve you want to set the interpolation for, and choose Constant Interpolation from the menu that opens.

.. _using_interpolations_based_on_similar_shapes:

Using Interpolations Based on Similar Shapes
''''''''''''''''''''''''''''''''''''''''''''
When the interpolation is based on a similar shape, the segment values changes according to the shape of the curve you specify as reference (see  :ref:`Using Transformation References <using_transformation_references>`  ). As soon as the interpolation is set, whenever the reference curve is edited, the segment will change accordingly.

This interpolation proves useful when you want to control at once several curves: if all of them share the same reference curve, by modifying the reference curve you will modify automatically all the curves referring to it.

It is also possible to set a frame offset value so that the interpolation will refer not to the same frame range of the reference curve, but to a different one.

.. tip:: **To set an interpolation based on a similar shape:**

    Do one of the following:

    - Choose Similar Shape from the option menu available in the interpolation area of the function editor.

    - Right-click the curve you want to set the transformation for, and choose Similar Shape Interpolation from the menu that opens.

.. tip:: **To set the reference curve:**

    1. Set the Reference Curve in the interpolation area of the function editor by typing the reference to an object or an effect transformation by using the appropriate syntax (see  :ref:`Using Transformation References <using_transformation_references>`  ). 

    2. Set a Frame Offset in the interpolation area of the function editor if you want the interpolation to refer not to the same frame range of the reference curve, but to a different one.

.. _controlling_several_function_curves_at_the_same_time:

Controlling Several Function Curves at the Same Time
----------------------------------------------------
It is possible to control the keys and the interpolations of all the function curves visualized in the Function Editor by using widgets available in a strip at the top of the window, below the frame ruler.




This allows you to define keys and control the interpolation speed for different curves at the same time, such as a camera truck and pan, or a special FX transformation and a pegbar movement.

As concerning keys, a key point is visible in the strip for each key point defined for any curve visible in the function editor; a line connects the key points for all the frames where there is a transformation going on. The key point can be moved, automatically moving the key point it refers to; in case the key point refers to key points at the same frame in several curves, all the key points will move along. 

As concerning interpolation, if all the visible curves have a key at the same specific frame, and the segment on the side of the key has the same ease in / ease out value or the same speed in / speed out horizontal component, a marker will be visible in the strip on the side of the key points. In particular the marker shaped as right square bracket is for the segment on the right of the key point, the one shaped like a left square bracket is for the segment on the left of the key point. The markers can be moved, automatically changing the ease in / ease out value or the speed in / speed out of all the segments they refer to. 

.. tip:: **To set which curves have to be controlled:**

    Display the function curves in the function editor (see  :ref:`Using the Function Editor <using_the_function_editor>`  ). 

.. tip:: **To add a key point:**

    Ctrl-click (PC) or Cmd-click (Mac) the frame ruler where you want to add the key point: a key point will be added to all the visible curves.

.. tip:: **To move a key point:**

    Click and drag it: all the key points it refers to will move along.

.. tip:: **To control the speed of the interpolation:**

    Move the markers visible on the sides of the key points.

.. |function_editor_1| image:: /_static/function_editor_1.png
.. |Toonz71_520| image:: /_static/Toonz71/Toonz71_520.gif
.. |Toonz71_521| image:: /_static/Toonz71/Toonz71_521.gif
.. |Toonz71_522| image:: /_static/Toonz71/Toonz71_522.gif
.. |Toonz71_524| image:: /_static/Toonz71/Toonz71_524.gif
.. |Toonz71_525| image:: /_static/Toonz71/Toonz71_525.gif
.. |Toonz71_526| image:: /_static/Toonz71/Toonz71_526.gif
.. |Toonz71_527| image:: /_static/Toonz71/Toonz71_527.gif
.. |Toonz71_528| image:: /_static/Toonz71/Toonz71_528.gif
.. |Toonz71_529| image:: /_static/Toonz71/Toonz71_529.gif
.. |Toonz71_530| image:: /_static/Toonz71/Toonz71_530.gif
