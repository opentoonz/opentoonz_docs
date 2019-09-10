.. _production_workflow:

Production Workflow
===================


.. _traditional_workflow:

Traditional Workflow
--------------------
The following is an example of how OpenToonz allows the management of a traditional animation production.

|traditional_workflow|


.. _scanning:

Scanning
~~~~~~~~
Hand-drawn elements are first defined in an OpenToonz Xsheet, and then acquired by using a scanner. These elements can consist of animation levels, i.e. sequences of drawings belonging to the same animation, or background images and overlays.

The scanned images then pass through a cleanup process, and are auto centered when necessary, using their pegbar holes as a guide and their related field guide setting. In the case of lineart drawings, these are further prepared for the painting process.

See  :ref:`Scanning Paper Drawings <scanning_paper_drawings>`  .


.. _paperless_drawing:

Paperless Drawing
~~~~~~~~~~~~~~~~~
Additional drawings and animation levels can be drawn directly in OpenToonz. Drawings can be an important part of the scene, such as a background or a character’s prop, or incidental elements needed to achieve a particular result, for example a mask image to create a matte effect.

See  :ref:`Drawing Animation Levels <drawing_animation_levels>`  .


.. _color_model:

Color Model
~~~~~~~~~~~
Color models are created for accurate color-referencing during production, when painting characters and props. They can be drawings made in OpenToonz, scanned images processed in OpenToonz, or images coming from a 3rd party software. 

In case of OpenToonz drawings, the color model palette can be defined by creating styles and colors to be used for painting animation levels.

See  :ref:`Managing Palettes and Styles <managing_palettes_and_styles>`  and  :ref:`Using a Color Model <using_a_color_model>`  .


.. _ink_&_painting:

Ink & Painting
~~~~~~~~~~~~~~
Animation levels scanned and cleaned up in OpenToonz, and those made directly in OpenToonz, are painted by using the styles stored in the palette and a set of tools.

Palette styles are interactively “linked” to drawn lines and filled areas by using indexes. The main advantage of this method is that if you edit a style of the palette, all the lines and filled areas using that style will be automatically updated. This allows you to change or calibrate colors also after the painting process has been done, without correcting the style line by line, or area by area.

See  :ref:`Managing Palettes and Styles <managing_palettes_and_styles>`  and  :ref:`Painting Animation Levels <painting_animation_levels>`  .


.. _compositing:

Compositing
~~~~~~~~~~~
All OpenToonz painted levels and images are exposed in the Xsheet where the timing of all the elements of a scene can be controlled. Images, animations and clips from 3rd party software can be loaded as well.

After adding and arranging the required elements to the Xsheet as layered columns, they are then animated by using interpolated keys placed on necessary parameters. Elements that can be animated in this way include the camera, columns, pegbars and the table.

Special FX, such as blurs, lights, keys, masks, warps, gradients, etc. can be applied to the content of Xsheet columns, and can also be animated by setting key value to the parameters.

Object and special FX transformations are mapped in the function editor window, where set key values and related interpolations can be controlled and modified by using function curves or numerical columns.

See  :ref:`Working in Xsheet <working_in_xsheet>` ,  :ref:`Creating Movements <creating_movements>` ,  :ref:`Applying Special FX <applying_special_fx>`  and  :ref:`Editing Using Spreadsheet and Curves <editing_curves_and_numerical_columns>`  .


.. _render_farm:

Render Farm
~~~~~~~~~~~
The scene is rendered in order to compose all the transformations and applied special FX in a sequence of frames in the format and resolution you prefer. 

The OpenToonz render farm allows you to batch-render OpenToonz scenes by using a series of computers connected on the same network using TCP/IP. 

See  :ref:`Rendering the Animation <rendering_the_animation>`  and  :ref:`Using the Toonz Farm <using_the_toonz_farm>`  .


.. _paperless_workflow:

Paperless Workflow
------------------
The following is an example of how OpenToonz allows the management of a paperless animation production.

|paperless_workflow|

.. _preproduction:_concept:

Preproduction: Concept
~~~~~~~~~~~~~~~~~~~~~~
Even if a paperless project can be run regardless of the script, the concept of a format with few settings and a stable cast of characters will ease the arrangement of libraries to be prepared before the actual episode production.


.. _preproduction:_graphic_design:

Preproduction: Graphic Design
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
The graphic design of characters, props and locations is equally important, in order to find out a style that will fit well both with the drawing capabilities of the software and with the cutout animation technique. 

In particular when designing character models and props, for which you could develop a specific line style to apply to vectors, or use very neat lines typical of vector animations, you should consider a design where the model animation pivot points can be easily disguised under drawings features (for example the pivot point of a ponytail linked to the character’s head can be disguised under a ribbon). 


.. _preproduction:_storyboard:

Preproduction: Storyboard
~~~~~~~~~~~~~~~~~~~~~~~~~
While usually the storyboard is used by the director to control the rhythm of the action, in case of a paperless production it also identifies all the elements needed for the production of each scene, by listing all of the character animations and poses, and identifying all of the props and backgrounds that are needed to implement the story.


.. _animatic:

Animatic
~~~~~~~~
The animatic is created starting from the scanned storyboard drawings. In OpenToonz, or in a third-party software, the storyboard drawings are imported, timing is adjusted and camera movements are set. Audio files too can be imported for reference.

In case the animatic is created in OpenToonz, it can also be split so that each cut can be used as a starting point for the final compositing of each scene.


.. _libraries:

Libraries
~~~~~~~~~
Libraries are prepared by drawing directly in OpenToonz all of the elements composing the scenes, such as locations, characters, props, etc. 

As far as the characters are concerned, they will be decomposed in multiple levels (i.e. head, torso, arms etc.) used as skeleton components rejoined through a hierarchy which at the end will make models available to the animators. 

According to the storyboard analysis, the drawings needed both for the canonical turn-around model (i.e. a collection of models as seen from different points of view: front, back, side and three-quarter views) and for additional movements are prepared. Starting from these reference animations, such as running or walking cycles, jumping, may be stored as well in order to be re-used in the scene production.

Props and backgrounds can be also created with third-party software, including rendered images from 3D software. 

See  :ref:`Drawing Animation Levels <drawing_animation_levels>`  and  :ref:`Creating Cutout Animation <creating_cutout_animation>`  .


.. _layout:

Layout
~~~~~~
In the layout phase, all of the elements that are necessary for the scene (backgrounds, props, characters, reference animations) are loaded from the library in Xsheet, usually as Sub-Xsheets. They are put in place according to the animatic. Basic animation is achieved by setting key positions for animated characters or importing reference animations.

Camera movements and animation timing previously set in the animatic are refined. 

See  :ref:`Working in Xsheet <working_in_xsheet>`  and  :ref:`Using Sub-Xsheets <using_sub-xsheets>`  .


.. _animation:

Animation
~~~~~~~~~
The animation for the scene defined in the layout is refined by adding key position to the character movements. Character poses are added by tweaking the model to achieve a more fluid animation.

The right speed for all the movements is set by controlling interpolation mode in the function editor.

See  :ref:`Animating Objects <animating_objects>`  and  :ref:`Using the Function Editor <using_the_function_editor>`  .


.. _special_fx:

Special FX
~~~~~~~~~~
Special FX, such as blur, glow, color corrections, particles, are applied to the scene elements. 

Additional animation elements related to special FX, for example masks or images for the particles effect, are drawn directly in the scene, or imported from external files.

See  :ref:`Applying Special FX <applying_special_fx>`  .


.. _render:

Render
~~~~~~
The scene has to be rendered in order to compose all the transformations and applied special FX in a sequence of frames in the format and resolution you prefer. 

The OpenToonz render farm allows you to batch-render OpenToonz scenes by using a series of computers connected on the same network using TCP/IP. 

See  :ref:`Rendering the Animation <rendering_the_animation>`  and  :ref:`Using the Toonz Farm <using_the_toonz_farm>`  .


.. |traditional_workflow| image:: /_static/production_workflow/traditional_workflow.png
.. |paperless_workflow| image:: /_static/production_workflow/paperless_workflow.png
.. |traditional_workflow_es| image:: /_static/production_workflow/es/traditional_workflow.png
