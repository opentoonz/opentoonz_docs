.. _whats_new:

What's New in OpenToonz
=======================

In this section you can find a list of Highlights in the latest release of OpenToonz; these may include New Features, Bug Fixes or Enhancements to already existent features.
Here, you can also find links to past versions' Release Notes, to keep track of OpenToonz development history throughout time.


.. _v1.6:

v1.6
----

.. _highlights:

Highlights
''''''''''

- |new| **Rhubarb integration** for automatic lip-syncing.
- |new| Xsheet/Timeline: Ability to **Shift + drag** an exposed cell to move it, while automatically adjusting neighbouring hold cells.
- |new| Xsheet/Timeline: Restored original Toonz feature for **changing parent of a column from the XSheet header** [Tahoma2D port].
- |new| Xsheet/Timeline: **Cell Mark** feature for identifying desired cells using colored dots.
- |new| UI: Xsheet **Minimum Layout** for ultra-compact column size.
- |new| UI: Xsheet **zoom** control.
- |new| UI: Zoom in/out and fit floating panel geometry commands.
- |new| Color Display: **30bit color display** feature.
- |new| I/O: Export **Xsheet to PDF**.
- |new| I/O: Export to **TVPaint JSON** file format.
- |new| I/O: **OpenEXR** image format support.
- |new| I/O: File Path Processing Using Regular Expressions.
- |new| Cleanup: Enabled to **Cleanup without Line Processing**, allows applying Autocenter, Rotation, etc. without further processing of the images.
- |new| Rendering: **Multi-Thread FFMPEG** option for faster rendering.
- |new| Brush and Paint Brush Tools: **Lock Alpha** setting for Toonz Raster and Raster level types.
- |new| Style Editor: **Hex editbox** for color values in Style Editor.
- |new| Style Editor: Hex color names editor.
- |new| Effects: **Linear color space** option for all Layer Blending Ino effects.
- |new| Effects: **Conical Transform** option for Fractal Noise Iwa effect.
- |new| Effects: **Image Size** option for the Input Size parameter for Tile Iwa effect.
- |new| Effects: **GPU HSL Blend** shader effect.
- |new| Effects: **Bokeh Advanced Iwa** effect.
- |new| Effects: **Compass Gadget** for Radial and Spin Blur effects.
- |new| Camera Capture: **Camera calibration**.
- |enhancement| Audio: **Improved Audio Recording**.
- |enhancement| Xsheet/Timeline: Enhanced **Note level column**.
- |enhancement| Viewer: Enhanced **Flipbook playback**.
- |enhancement| Schematic: Allowed **Renaming** Pass Through Nodes (Tahoma2D port).
- |enhancement| I/O: Enabled to **set Raster level frame number format**.
- |enhancement| I/O: Enabled to **use PNG for new Raster levels**.
- |enhancement| I/O: Enhanced **FFMPEG GIF export**.
- |enhancement| File Browser: Enabled to **view palette files from the File Browser**.
- |enhancement| Palette: Enabled to **paste style's color into a color field**.
- |enhancement| Effects: **Fx Intensity** parameter for controlling global effect intensity.
- |enhancement| Effects: **Redesigned Pass Through** effect node.
- |enhancement| Camera Capture: Enabled **inputting frame with suffix** in Camera Capture.
- |enhancement| Stop-motion: Enhanced **Stop motion** feature.
- |enhancement| Packaging Opentoonz for Fedora distribution.
- |fix| Crash on showing snapshot in flipbook.
- |fix| Crash on saving scene containing missing palette level.
- |fix| Crash on undoing tool.
- |fix| Crash after starting a pen stroke from inactive window.
- |fix| Crash on Stage Schematic Column Right click.
- |fix| Crash on rendering ArtContour fx.
- |fix| Crash on rendering PaletteFilter Fx (and other fxs) with hyphen.
- |fix| Crash on cleaning up zerary column.
- |fix| Crash on creating a zerary fx in the camera column.
- |fix| Crash on creating Macro Fx from the Fx Browser.
- |fix| Crash On Inserting Fx.
- |fix| Crash on clicking shortcut tree.
- |fix| Crashes when using Type tool.
- |fix| Crash on deleting control point while dragging.
- |fix| Crash on switching scenes while selecting raster level frame.
- |fix| Undo Malfunction.
- |fix| File browser assertion failure.
- |fix| "Show Folder Contents" command for UNC path.
- |fix| Viewer playback.
- |fix| Flipbook wobbling when dragging while playing.
- |fix| Pressing Shift key loses focus when renaming cell.
- |fix| Autorenumber of Raster Level.
- |fix| Cell Selection on Click.
- |fix| GIF rendering on older versions.
- |fix| Saving TLV.
- |fix| Output file name for movie format.
- |fix| PSD loading and level format preferences.
- |fix| Backtab key to work for moving styles shortcut scope.
- |fix| FrameIDs Inconsistency in Level Strip Commands.
- |fix| Memo Popup Background Color.
- |fix| FX gadget picking.
- |fix| Margin of Directional Blur Fx Iwa.
- |fix| Zerary Fx bugs.
- |fix| Friction parameter behavior of the Particles Fx.
- |fix| Rendering Fx After Xsheet Node.
- |fix| Channel clamping behavior in Layer Blending Fxs.
- |fix| Fx Gadget Offset.
- |fix| Bokeh Fxs Artifacts.
- |fix| Schematic node placement fix.
- |fix| Shortcut loading from file.
- |fix| Tool options' shortcuts to work without opening tool options bar.
- |fix| Camera capture's level control.
- |fix| Mesh file naming.
- |fix| Wheel scrolling on the output settings popup
- |fix| Missing Checkboxes in Menu Item
- |fix| Convert to TLV Palette Saving
- |fix| Raster Deformation Slowness

...and much more!

Please see the `v1.6 Release Notes <https://github.com/opentoonz/opentoonz/releases/tag/v1.6.0>`_  hosted in GitHub, for the full list of new features, enhancements and bug fixes.



.. _previous versions:

Previous Versions of OpenToonz
------------------------------

Here you can find links to previous versions' full Release Notes, hosted in GitHub:

`v1.5 Release Notes <https://github.com/opentoonz/opentoonz/releases/tag/v1.5.0>`_

`v1.4 Release Notes <https://github.com/opentoonz/opentoonz/releases/tag/v1.4.0>`_

`v1.3 Release Notes <https://github.com/opentoonz/opentoonz/releases/tag/v1.3.0>`_

`v1.2.1 Release Notes <https://github.com/opentoonz/opentoonz/releases/tag/v1.2.1>`_

`v1.2 Release Notes <https://github.com/opentoonz/opentoonz/releases/tag/v1.2.0>`_

`v1.1.3 Release Notes <https://github.com/opentoonz/opentoonz/releases/tag/v1.1.3>`_

`v1.1.2 Release Notes <https://github.com/opentoonz/opentoonz/releases/tag/v1.1.2>`_

`v1.1 Release Notes <https://github.com/opentoonz/opentoonz/releases/tag/v1.1.0>`_

`v1.0.3 Release Notes <https://github.com/opentoonz/opentoonz/releases/tag/v1.0.3>`_

`v1.0.2 Release Notes <https://github.com/opentoonz/opentoonz/releases/tag/v1.0.2>`_

`v1.0 Release Notes <https://github.com/opentoonz/opentoonz/releases/tag/v1.0>`_




.. |new| image:: /_static/whats_new/new.png
.. |enhancement| image:: /_static/whats_new/enhancement.png
.. |fix| image:: /_static/whats_new/fix.png

.. |new_es| image:: /_static/whats_new/es/new.png
.. |enhancement_es| image:: /_static/whats_new/es/enhancement.png
.. |fix_es| image:: /_static/whats_new/es/fix.png

