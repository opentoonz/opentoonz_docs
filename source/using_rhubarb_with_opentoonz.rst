.. _using_rhubarb_with_opentoonz:

Using Rhubarb with OpenToonz
============================

What is Rhubarb?
----------------
| Rhubarb Lip Sync is a command-line tool that automatically creates 2D mouth animation from voice recordings. It can be used to provide automatic lip-sync capabilities inside OpenToonz, for that to be possible OpenToonz requires Rhubarb to be installed on your machine and appropriately configured in Preferences.
| For more information, please visit this page: `About Rhubarb <https://github.com/DanielSWolf/rhubarb-lip-sync>`_


Installing Rhubarb for Windows
------------------------------

Downloading
~~~~~~~~~~~

| To download Rhubarb, visit this page: `Download Rhubarb <https://github.com/DanielSWolf/rhubarb-lip-sync/releases>`_
| Download the latest **Rhubarb-Lip-Sync-x.y.z-Windows.zip** file (where 'x.y.z' represent the software version number).

Installing
~~~~~~~~~~

| Once you have downloaded the Rhubarb zip archive, extract it in the desired location of your system (**C:\\** is recomended).

|rhubarb_extracted_windows|

- Next, start OpenToonz and open the Preferences window with File  →  **Preferences...**
- Navigate to the **Auto Lip-Sync** category; at the top you will see a box with the text **Rhubarb Path**.
- Insert the path to your extracted Rhubarb folder (if you have used the recommended path, this will be **C:\\Rhubarb-Lip-Sync-x.y.z-Windows\\**):

|rhubarb_path_windows|

- Restart OpenToonz.


Installing Rhubarb for Mac
--------------------------

Downloading
~~~~~~~~~~~

| To download Rhubarb, visit this page: `Download Rhubarb <https://github.com/DanielSWolf/rhubarb-lip-sync/releases>`_
| Download the latest ** Rhubarb-Lip-Sync-x.y.z-macOS.zip ** file (where 'x.y.z' represent the software version number).

Installing
~~~~~~~~~~

| Once you have downloaded the Rhubarb zip archive, extract it in the desired location of your system.

|rhubarb_extracted_mac|

- Next, start OpenToonz and open the Preferences window with File  →  **Preferences...**
- Navigate to the **Auto Lip-Sync** category; at the top you will see a box with the text **Rhubarb Path**.
- Insert the path to your extracted Rhubarb folder:

|rhubarb_path_mac|

- Restart OpenToonz.


Installing Rhubarb for Linux
----------------------------

| To install Rhubarb, enter the following command in the shell depending on your distribution.

Arch Linux: ``# pacman -S extra/rhubarb``

Debian GNU/Linux: ``# apt install rhubarb``

Gentoo Linux: ``# emerge media-audio/rhubarb``

Solus: ``# eopkg install rhubarb``

| If you are using any other Linux distribution please refer to its documentation or visit the `Rhubarb download page <https://github.com/DanielSWolf/rhubarb-lip-sync/releases>`_ and download the latest **Rhubarb-Lip-Sync-x.y.z-Linux.zip** file (where 'x.y.z' represent the software version number).

|rhubarb_extracted_linux|

- Start OpenToonz and open the Preferences window with File  →  **Preferences...**
- Navigate to the **Auto Lip-Sync** category; at the top you will see a box with the text **Rhubarb Path**.
- Insert the path **/usr/bin**, or a path pointing to where you've extracted the downloaded zip file.

|ffmpeg_path_linux|

- Restart OpenToonz.



.. Common Images


.. Windows images
.. |rhubarb_extracted_windows| image:: /_static/using_ffmpeg_with_opentoonz/windows/rhubarb_extracted.png
.. |rhubarb_path_windows| image:: /_static/using_ffmpeg_with_opentoonz/windows/rhubarb_path.png

.. Mac images
.. |rhubarb_extracted_mac| image:: /_static/using_ffmpeg_with_opentoonz/mac/rhubarb_extracted.png
.. |rhubarb_path_mac| image:: /_static/using_ffmpeg_with_opentoonz/mac/rhubarb_path.png

.. Linux images
.. |rhubarb_extracted_linux| image:: /_static/using_ffmpeg_with_opentoonz/linux/rhubarb_extracted.png
.. |rhubarb_path_linux| image:: /_static/using_ffmpeg_with_opentoonz/linux/rhubarb_path.png

.. Note from gab3d
.. This is a work-in-progress page, please contribute to its development by adding anything you see helpful or needed.
.. Currently the Mac and Linux sections are just simple adaptations of the Windows section (Mac), or from the Linux section of Using FFmpeg page.
.. Paths to image names are there, waiting for the respective image files to be created and uploaded.

.. Credits:
.. Windows section contributed by gab3d
.. Mac section contributed by <yournamehere>
.. Linux section contributed by <yournamehere>

