.. _using_ffmpeg_with_opentoonz:

Using FFmpeg with OpenToonz
===========================

What is FFmpeg?
---------------
| To render your animation as an **mp4** or **webm**, or also as a **gif** on Mac, OpenToonz requires the FFmpeg multimedia framework to be installed on your machine.
| For more information, please visit this page: `About FFmpeg <https://www.ffmpeg.org/about.html>`_

Installing FFmpeg for Windows
-----------------------------

Downloading
~~~~~~~~~~~

| To download FFmpeg, first visit this page: `Download FFmpeg <https://www.ffmpeg.org/download.html>`_

|get_the_packages|

| Select the Windows icon and then select the **Windows builds** link:

|packages_windows|

| You will be taken to an **FFmpeg Builds** page with some options for the version of FFmpeg that you want to download:

|ffmpeg_builds_windows|

| In the majority of cases, the default choices are fine.
| Click on the blue **Download Build** button, this will begin downloading a zip archive containing FFmpeg.

Installing
~~~~~~~~~~

| Once you have downloaded the FFmpeg zip archive, open it and double-click on the first folder.

| Within the **bin** folder are the executable files that you will need.

- Create a new folder on your computer, the recommended location is **C:\\**.
- Name the new folder **FFmpeg**.
- Drag the contents of the **bin** folder from the archive into the newly created folder.

|ffmpeg_extracted_windows|

- Next, start OpenToonz and open the **Preferences** window with File  →  **Preferences...**
- Navigate to the **Import/Export** category; at the top you will see a box with the text **FFmpeg path**.
- Insert the path to your FFmpeg folder that you created earlier, if you have used the recommended path, this will be **C:\\FFmpeg\\**:

|ffmpeg_path_windows|

- Restart OpenToonz.
- Open the **Output Settings** window with Render  →  **Output Settings...**

| In the **File Settings** subsection, you should now see **mp4** and **webm**.

|output_settings_windows|

Installing FFmpeg for Mac
-------------------------

Downloading
~~~~~~~~~~~

| To download FFmpeg, first visit this page: `Download FFmpeg <https://www.ffmpeg.org/download.html>`_

|get_the_packages|

| Select the Apple icon and select the **Static and Shared builds** link.

|packages_mac|

| You will be taken to an **FFmpeg Builds** page with some options for the version of FFmpeg that you want to download:

| Make sure **macOS 64-bit** is selected under the **Architecture** column.

|ffmpeg_builds_mac|

| Click on the blue **Download Build** button, this will begin downloading a zip archive containing FFmpeg.

Installing
~~~~~~~~~~

| Once you have downloaded the FFmpeg zip archive, open it and double-click on the first folder.

| Within the **bin** folder are the executable files that you will need.

- Open Finder and create a new folder, the **Applications/OpenToonz** folder is the recommended location.

|ffmpeg_finder|

- Name the new folder **FFmpeg**.
- Drag the contents of the **bin** folder from the archive into the newly created folder.

|ffmpeg_extracted_mac|

.. tip:: For macOS 10.15 and later, each executable within the FFmpeg folder needs to be opened before using OpenToonz (this only needs to be done one time, due to security features). In Finder, right-click on each executable (ffmpeg, ffprobe, and etc.) and select ``Open With → Terminal``. Once the Terminal windows have launched successfully, Terminal can be closed.


- Next, start OpenToonz and open the **Preferences** window with File  →  **Preferences...**
- Navigate to the **Import/Export** category; at the top you will see a box with the text **FFmpeg path**.
- Insert the path to your FFmpeg folder that you created earlier, if you have used the recommended path, this will be **/Applications/OpenToonz/FFmpeg**:

|ffmpeg_path_mac|

- Restart OpenToonz.
- Open the **Output Settings** window with Render  →  **Output Settings...**

| In the **File Settings** subsection, you should now see **mp4**, **webm** and **gif**.

|output_settings_mac|

Installing FFmpeg for Linux
---------------------------

| To install FFmpeg, enter the following command in the shell depending on your distribution.

Arch Linux: ``# pacman -S extra/ffmpeg``

Debian GNU/Linux: ``# apt install ffmpeg``

Gentoo Linux: ``# emerge media-video/ffmpeg``

Solus: ``# eopkg install ffmpeg``

| If you are using a other Linux distribution please refer to its documentation or visit the `FFmpeg website <https://www.ffmpeg.org/download.html>`_.

.. tip:: To make it possible to export files in **mp4**, **webm** or **gif** formats, you need to specify the path to FFmpeg installed on your system, usually it is **/usr/bin/ffmpeg**. Enter command ``which ffmpeg`` in the shell to find out.

- Start OpenToonz and open the **Preferences** window with File  →  **Preferences...**
- Navigate to the **Import/Export** category; at the top you will see a box with the text **FFmpeg path**.
- Insert the path **/usr/bin**.

|ffmpeg_path_linux|

- Restart OpenToonz.
- Open the **Output Settings** window with Render  →  **Output Settings...**

| In the **File Settings** subsection, you should now see **mp4**, **webm** and **gif**.

|output_settings_linux|

.. Images

.. |get_the_packages| image:: /_static/using_ffmpeg_with_opentoonz/get_the_packages.png


.. Windows images
.. |packages_windows| image:: /_static/using_ffmpeg_with_opentoonz/windows/ffmpeg_packages.png
.. |ffmpeg_builds_windows| image:: /_static/using_ffmpeg_with_opentoonz/windows/ffmpeg_builds.png
.. |ffmpeg_extracted_windows| image:: /_static/using_ffmpeg_with_opentoonz/windows/ffmpeg_extracted.png
.. |ffmpeg_path_windows| image:: /_static/using_ffmpeg_with_opentoonz/windows/ffmpeg_path.png
.. |output_settings_windows| image:: /_static/using_ffmpeg_with_opentoonz/windows/output_settings.png


.. Mac images
.. |packages_mac| image:: /_static/using_ffmpeg_with_opentoonz/mac/ffmpeg_packages.png
.. |ffmpeg_builds_mac| image:: /_static/using_ffmpeg_with_opentoonz/mac/ffmpeg_builds.png
.. |ffmpeg_finder| image:: /_static/using_ffmpeg_with_opentoonz/mac/ffmpeg_finder.png
.. |ffmpeg_extracted_mac| image:: /_static/using_ffmpeg_with_opentoonz/mac/ffmpeg_extracted.png
.. |ffmpeg_path_mac| image:: /_static/using_ffmpeg_with_opentoonz/mac/ffmpeg_path.png
.. |output_settings_mac| image:: /_static/using_ffmpeg_with_opentoonz/mac/output_settings.png

.. Linux images

.. |ffmpeg_path_linux| image:: /_static/using_ffmpeg_with_opentoonz/linux/ffmpeg_path.png
.. |output_settings_linux| image:: /_static/using_ffmpeg_with_opentoonz/linux/output_settings.png

.. Note from Wolf_In_A_Bowl
.. This is a work-in-progress page, please contribute to its development by adding the guide section for and Linux.
.. Once the remaining section has been added, please remove this note.

.. Need new output_settings_mac image

.. Credits:
.. Windows section contributed by Wolf_In_A_Bowl
.. Mac section contributed by Jane Eyre

