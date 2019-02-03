.. _using_ffmpeg_with_opentoonz:

Using FFmpeg with OpenToonz
===========================

What is FFmpeg?
---------------
| To render your animation as an **mp4** or **webm**, OpenToonz requires the FFmpeg multimedia framework to be installed on your machine.
| For more information, please visit this page: `About FFmpeg <https://www.ffmpeg.org/about.html>`_

Downloading FFmpeg
------------------
| To download FFmpeg, first visit this page: `Download FFmpeg <https://www.ffmpeg.org/download.html>`_

|get_the_packages|

| Next, choose your operating system to be taken to the appropriate section:
| `Windows <Downloading FFmpeg for Windows_>`_
| `Mac <Downloading FFmpeg for Mac_>`_
| `Linux <Downloading FFmpeg for Linux_>`_

Downloading FFmpeg for Windows
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
| For Windows users, click the Windows logo and then select the **Windows builds** section:

|windows_packages|

| You will be taken to an **FFmpeg Builds** page with some options for the version of FFmpeg that you want to download:

|ffmpeg_builds_windows|

| In the majority of cases, the default choices are fine.
| Hit the blue **Download Build** button, this will begin downloading a zip archive containing FFmpeg.

| You can now proceed to the next section: `Installing FFmpeg for Windows`_.

Downloading FFmpeg for Mac
~~~~~~~~~~~~~~~~~~~~~~~~~~

| Yet to be added, please contribute if you are able

| You can now proceed to the next section: `Installing FFmpeg for Mac`_.

Downloading FFmpeg for Linux
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

| Yet to be added, please contribute if you are able

| You can now proceed to the next section: `Installing FFmpeg for Linux`_.

Installing FFmpeg
-----------------

Installing FFmpeg for Windows
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
| Once you have downloaded the FFmpeg zip archive, open it and double-click on the first folder, you should be presented with three folders:

|ffmpeg_archive_windows|

| Within the **bin** folder are the executable files that you will need.
| Create a new folder on your computer, the recommended location is **C:\\**, name the new folder **FFmpeg**.
| Then, drag the **bin** folder from the archive into the newly created folder.

| Next, start OpenToonz and open the **User Preferences** window with ``File > Preferences...``
| Navigate to the **Import/Export** category; at the top you will see a box with the text **FFmpeg path**.
| Insert the path to your FFmpeg's bin folder that you extracted earlier, if you have used the recommended path, this will be **C:\\FFmpeg\\bin**:

|ffmpeg_path_windows|

| Finally, restart OpenToonz, start a new project or open an existing one and open the **Output Settings** window with ``File > Output Settings...``
| In the **File Settings** subsection, you should see mp4 and webm as file formats.

|output_settings_windows|


Installing FFmpeg for Mac
~~~~~~~~~~~~~~~~~~~~~~~~~

| Yet to be added, please contribute if you are able

Installing FFmpeg for Linux
~~~~~~~~~~~~~~~~~~~~~~~~~~~

| Yet to be added, please contribute if you are able

.. Images

.. |get_the_packages| image:: /_static/using_ffmpeg_with_opentoonz/get_the_packages.png

.. Windows images
.. |windows_packages| image:: /_static/using_ffmpeg_with_opentoonz/windows/windows_packages.png
.. |ffmpeg_builds_windows| image:: /_static/using_ffmpeg_with_opentoonz/windows/ffmpeg_builds.png
.. |ffmpeg_archive_windows| image:: /_static/using_ffmpeg_with_opentoonz/windows/ffmpeg_archive.png
.. |ffmpeg_path_windows| image:: /_static/using_ffmpeg_with_opentoonz/windows/ffmpeg_path.png
.. |output_settings_windows| image:: /_static/using_ffmpeg_with_opentoonz/windows/output_settings.png

.. Mac images

.. Linux images


.. Note from Wolf_In_A_Bowl
.. This is a work-in-progress page, please contribute to its development by adding guide sections for Mac and Linux.
.. Once these sections have been added, please remove this note.