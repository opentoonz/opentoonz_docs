.. _scanning_paper_drawings:

Scanning Paper Drawings
=======================

.. note:: Currently OpenToonz DOES NOT SUPPORT the native scanning functionality, as described in this page. Instead you can use the provided GTS scanning and cleaning software, please follow `this link to download GTS <https://opentoonz.github.io/e/download/gts.html>`_ .

.. note:: This manual page is preserved in its original form, in case the scanning code of OpenToonz is reactivated in a future version.


In order to be managed by OpenToonz, paper drawings have to be scanned into OpenToonz. Paper drawings can be both animation levels, consisting of a large number of sequenced drawings, and other elements such as backgrounds and overlays.

The scan process can be done in different modes, and in case autocenter is needed it has to follow specific guidelines. 

Animation levels have to be defined first and then scanned according to a defined set of parameters.


.. _supported_scanners:

Supported Scanners
------------------
OpenToonz supports directly, by using internal drivers, some specific scanners via a USB connection; all the other scanners are supported via any type of connection by using TWAIN drivers. 

 |define_scanner|
 
.. note:: For an updated list of directly supported scanners, please visit the `OpenToonz Web site <https://opentoonz.github.io/e/>`_ .

If your scanner is supported via internal drivers, the scanning process is managed completely by OpenToonz and the Scan Settings dialog; if it is not, the scanning process is managed by the TWAIN interface.

On Windows, the TWAIN drivers provided with the scanner need to be installed. Note that if you decide to use internal drivers, you have to disable the **Windows Image Acquisition (WIA)** service on your computer; if you want to use TWAIN drivers, you have to enable it.

On macOS, you need to install the TWAIN drivers only if you are going to use them. Note that if you decide to use internal drivers, any TWAIN driver referring to that scanner has to be removed.

The driver you want to use must be selected according to your scanner before starting the scanning process. You can choose whether to use the internal or TWAIN drivers; in the latter case, you have to select which driver to use from a list based on the TWAIN drivers installed on your computer.

.. note:: When using TWAIN drivers you need to specify the driver every time you restart OpenToonz: the dialog box is automatically displayed when you select any Scan related command.

.. tip:: **To install TWAIN drivers:**

    Refer to the scanner documentation for more details.

.. tip:: **Windows only - To disable or enable the Windows Image Acquisition (WIA) service:**

    1. Open the Control Panel  →  Administrative Tools  →  **Services** dialog.

    2. Right-click the **Windows Image Acquisition (WIA)** service and choose **Properties** from the menu that opens.

    3. In the Properties dialog do one of the following:

    - Set the **Startup Type** option to **Disabled** to use internal drivers.

    - Set the **Startup Type** option to **Automatic** to use TWAIN drivers.

    4. Restart the computer.

.. tip:: **Macintosh only - To remove the scanner TWAIN drivers:**

    Refer to the scanner documentation for more details.

.. tip:: **To define the scanner:**

    1. Choose Scan & Cleanup  →  **Define Scanner...**.

    2. Do one of the following:

    - If your scanner is directly supported, choose Scanner Driver  →  **Internal**, and click the **OK** button.

    - If your scanner is not directly supported, be sure that TWAIN drivers are installed, and choose Scanner Driver  →  **TWAIN**, and click the **OK** button: in the dialog that opens, select the TWAIN driver related to your scanner.


.. _scanning_modes:

Scanning Modes
--------------
Drawings can be scanned mainly in three different modes: *black and white*, *greyscale* and *color*. 

The first two modes can be used to acquire standard lineart drawings whose outline is usually made in a single color, that during the scanning is acquired as black or dark grey. Even if the outline color is lost during the scanning, later on you can assign one or more colors to it during the painting process.

**Black and white** scanning gives you the most immediate results, and fewer parameters need to be set. Once a **Threshold:** value is set, pixels of the scanned image are considered as either black or white. Due to the simplicity of this concept, less time is required to scan the image, and scanned files are lighter to manage. Even if images show hard edges, the proper antialiasing will be added during the cleanup process.

**Greyscale** scanning, being based on a range of grey values, requires a longer scanning time. Determining **Brightness:** and **Contrast:** parameters depends considerably on the individual animated sequence and on what you want to achieve. The greyscale mode also offers **Autoadjust** options during the cleanup process, useful to even the differences between drawings made by key animators and those made by in-betweeners. See  :ref:`Autoadjusting Greyscale Lineart Drawings <autoadjusting_greyscale_lineart_drawings>`  .

**Color** scanning is for scanning colored lineart and other colored images as backgrounds and overlays. Using colors in lineart allows you to draw different lines with different colors, for example a character outline in black and its body shadow in red or in blue. As colored lines can be identified later during the cleanup process, scanning colored artwork in colors allows you to preserve different line colors with no need of intensive painting work. See  :ref:`Processing Colored Lineart Drawings <processing_colored_lineart_drawings>`  .


.. _scanning_guidelines_for_autocentering:

Scanning Guidelines for Autocentering
-------------------------------------
To autocenter scanned drawings during the cleanup process, the pegbar holes need to be detected on the images (see  :ref:`Autocentering <autocentering>`  ). For this reason they have to be scanned in black, by properly preparing the scanner and performing the scanning process according to the following guidelines.


.. _preparing_scanners:

Preparing Scanners
''''''''''''''''''
    - If you use the scanner automatic paper feeder, you should stick a piece of thin black tape in the feeder on the opposite side of the scanner lamp. Be sure to stick the black tape in a position to face the peg holes when the paper is fed into the scanner. 

    - If you use the scanner bed, you should place a black sheet of paper under the scanner cover, so that when a drawing is scanned facing down the glass of the scanner bed, the black paper will be behind it. The black paper must be larger than your animation paper, but it does not have to cover the entire scanner bed.


.. _scanning_artwork:

Scanning Artwork
''''''''''''''''
    - It is better to use quite thick animation paper for your artwork: very thin paper may jam the scanner, and the scanner light may pass through picking up some grey from the black paper or tape placed behind it. When this happens, the process will take longer to perform and will produce a poor quality result.

    - Avoid using *black* or *colored* paper reinforcements around the pegbar holes in your drawing sheets. The scanner has to read the exact shape of the hole punches, and colored reinforcements may cause holes to be scanned larger than their actual size. If you do use *white* reinforcements, make sure they are aligned directly over the peg holes: if the holes are slightly covered by the reinforcement, the registration may fail.

    - Do not draw too close to the pegbar holes. Avoid drawing anything with the same shape or area of the pegbar hole in the pegbar holes area; leave at least 1 cm (~1/2”) of clear space between the pegbar holes and the rest of your drawings. Lines drawn near the pegbar holes may cause the registration to fail.


.. _defining_animation_levels_to_scan:

Defining Animation Levels to Scan
---------------------------------
To scan an animation level, first you have to define its name, the number of frames it is made of, and the way its drawings are numbered. Its size and resolution will be set during the scanning session.

The definition can be made drawing by drawing directly in the Xsheet/Timeline, or at once by using the **New Level** dialog. You can assign it the name and the numbering order you prefer. 

In case you use the **New Level** dialog you can set the number of drawings the level is made of, the animation step to expose the level repeating its frames, and the increment, that sets the way the level drawings are numbered. For example a **Step:** value 2 repeats each drawing twice in the Xsheet column (or Timeline layer), while an **Increment:** value 2 numbers the drawings 1, 3, 5, etc.

 |new_scan_level|

By default scanned drawings are saved in the **+inputs** directory of the current project; if the *+inputs* definition uses the $scenepath variable, they are saved only if the scene is saved (see  :ref:`Project Default Folders <project_default_folders>`  ). 

You can change the location by using either the **Path:** field in the **New Level** dialog, or the **Level Settings** window in case you define a level directly in Xsheet/Timeline. 

Settings such as the length of the level and the numbering order can be edited later, as you are free to arrange the images composing your animation level the way you prefer (see  :ref:`Editing Animation Levels <editing_animation_levels>`  ).

When an animation level is defined, the name and numbers for the drawings of the level are displayed in *red* as no level actually exists yet; the column/layer cells where the level is exposed are colored in *light blue*, the color denoting full-color images (see  :ref:`Working with Columns/Layers <working_with_xsheet_columns>`  ). 

.. tip:: **To define an animation level directly in Xsheet:**

    1. Double-click a cell, then type a name and a number; the name and the number must be separated by a space.

    2. Press **Enter** to add a new drawing, and type a different number that will be assigned to the new drawing. 

    3. Go on adding all the drawings you need.

    4. Click a different cell to end the process.

.. tip:: **To define an animation level with the New Level dialog:**

    1. Do one of the following:

    - Select a cell in the Xsheet/Timeline where you want to place your animation level to scan and choose Level  →  New  →  **New Level...**

    - Right-click the cell in the Xsheet/Timeline where you want to place your animation level to scan and choose **New Level** from the menu that opens.

    .. note:: If any level is already exposed in the cell column/layer, it will shift down/right from the cell you selected on.

    2. In the New Level dialog choose **Scan Level** from the **Type:** option menu and define its settings, then click the **OK** button.

.. tip:: **To define the saving location for the level to be scanned:**

    Do one of the following:

    - If you are using the **New Level** dialog, type in the **Path:** field, or use the browser button, to set the path for the saving location.

    - If you are defining the level directly in Xsheet/Timeline, right-click the level cells and select **Level Settings** from the menu that opens. In the Level Settings window, type in the **Path:** field, or use the browser button, to set the path for the saving location.

.. note:: If in the browser you choose any project default folder, in the **Path:** field the full path will be replace by the related default folder alias (see  :ref:`Project Default Folders <project_default_folders>`  ).


.. _scanning_drawings:

Scanning Drawings
-----------------
According to the driver you are using, internal or TWAIN, the scanning process will be controlled either by the Scan Settings dialog or the TWAIN interface.

 |scan_settings|

The Scan Settings dialog allows you to define the following:

- **Paper Format** sets the size for the drawings to be scanned. The option menu contains a list of already defined formats.

- **Reverse Order** makes the scanning process in a reverse order, starting from the last selected frame to the first one. 

- **Paper Feeder** lets the scanner use the automatic document feeder, in case the scanner has one, to scan all the selected drawings without having to insert one image at a time into the scanner.

- **Mode** is for setting the scanning mode among: **Black and White**, **Greyscale** and **Color**. 

The TWAIN interface is related to the scanner you are using and will be available only when the TWAIN drivers, provided with the scanner, are installed on your computer. Refer to the scanner documentation for more details.

.. note:: The Scan Settings dialog can be used in combination with the TWAIN interface settings to set the Reverse Order option.

The settings, either defined in the Scan Settings dialog or in the TWAIN interface, will be used to scan the drawings selected in the Xsheet/Timeline. In case you select several drawings, and you are using the scanner paper feeder, all the drawings to be scanned will be taken from the feeder; if you are not using the paper feeder, you will be prompted to replace the drawing on the scanner bed, before scanning the following drawing.

You can also select non-consecutive drawings and drawings from different animation levels. Levels will be scanned starting from the first selected column/layer. Only exposed drawings will be scanned according the level numbering order, regardless of the way the animation level is exposed in one or several Xsheet columns (or Timeline layers). The opposite order will be followed if the **Reverse Order** option is on.

As soon as a drawing is scanned, it is saved and its name and number displayed in the Xsheet/Timeline turn black, as the level now has physical drawings saved on disk. 

Images are saved as compressed TIF files with a progressive four-digits number written between the file name and the file extension, e.g. ``animation.0001.tif`` , ``animation.0002.tif`` , etc. They are displayed in the OpenToonz browser with a double dot before the file extension, e.g. ``animation..tif`` .

If you need to scan again an animation level, or a part of it, select the relevant drawings and scan them again. Drawings can be also inserted by editing the level sequence (see  :ref:`Renumbering and Adding Frames in a Level <renumbering_and_adding_frames_in_a_level>`  ).

.. tip:: **To scan an animation level:**

    1. In the Xsheet/Timeline, select the drawings you want to scan. 

    2. Choose Scan & Cleanup  →  **Scan Settings...** and use the dialog to control scan options. 

    3. Do one of the following:

    - If you are using the internal drivers, choose Scan & Cleanup  →  **Scan**: the selected drawings will be scanned and automatically saved.

    - If you are using the TWAIN drivers, choose Scan & Cleanup  →  **Scan**, and guide the scanning process by using the TWAIN interface that opens: the selected drawings will be scanned and automatically saved.

    4. In case you selected several drawings, do one of the following:

    - If you are using the scanner paper feeder, wait for all of the drawings to be scanned.

    - If you are not using the paper feeder, you will be prompted to replace the drawing on the scanner bed, before scanning the following drawing.

.. note:: After a drawing is scanned, or several drawings are scanned at once by using the paper feeder, in some TWAIN interfaces you may need to use a specific command (such as **Back to Application**) to return to OpenToonz before proceeding with the next scanning session. Refer to the scanner documentation for more details.


.. _setting_the_cropbox:

Setting the Cropbox
'''''''''''''''''''
When using directly supported scanners it is possible to define a *cropbox* smaller than the paper format to optimize the scanning process. When the *cropbox* is set the final scanned image will be the size of the selected paper format, but only the area defined by the *cropbox* is actually scanned, thus speeding up the scanning operations.

Once defined the cropbox will be used for any scanning performed for the scene. 

.. note:: The cropbox size information is not saved along with the scene file; it is also automatically reset when working on a new scene.

.. tip:: **To define the scanning cropbox:**

    1. Choose Scan & Cleanup  →  **Set Cropbox**: the drawing currently placed in the scanner is scanned and the cropbox is displayed in *red*. 

    2. Use the handles along the cropbox to set its size, and click and drag anywhere to change its position.

.. note:: The cropbox default size is the same as the size of the scanned image.

.. note:: The cropbox cannot be moved outside the area of the scanned image.

.. tip:: **To use the defined cropbox when scanning:**

    Scan drawings after defining the cropbox size (see above ).

.. tip:: **To dismiss the scanning cropbox visualization:**

    Choose Scan & Cleanup  →  **Set Cropbox**.

.. tip:: **To reset the scanning cropbox:**

    Choose Scan & Cleanup  →  **Reset Cropbox**.



.. |define_scanner| image:: /_static/scanning_paper_drawings/define_scanner.png
.. |new_scan_level| image:: /_static/scanning_paper_drawings/new_scan_level.png
.. |scan_settings| image:: /_static/scanning_paper_drawings/scan_settings.png


.. |define_scanner_es| image:: /_static/scanning_paper_drawings/es/define_scanner.png
.. |new_scan_level_es| image:: /_static/scanning_paper_drawings/es/new_scan_level.png
.. |scan_settings_es| image:: /_static/scanning_paper_drawings/es/scan_settings.png

