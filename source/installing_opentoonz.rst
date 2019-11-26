.. _installing_opentoonz:

Installing OpenToonz
====================


.. _downloading_opentoonz:

Downloading OpenToonz
---------------------
You can download the appropriate version of OpenToonz for your operating system from the `Download page <https://opentoonz.github.io/e/download/opentoonz.html>`_ in the official OpenToonz web site. Choose either the Windows or macOS version to start downloading the installer application. It's possible to find the official "nightly" builds `here <https://github.com/opentoonz/opentoonz_nightlies>`_. Other builds ARE NOT officially supported.

Also, the `MorevnaProject <https://github.com/morevnaproject>`_ provides experimental builds for `Windows 32-bit, Windows 64-bit, macOS, appimage <https://github.com/morevnaproject/opentoonz/releases>`_ and `snap <https://snapcraft.io/opentoonz-morevna>`_ for Linux. Moreover, there are OTX (OpenToonz eXperimental) releases by `manongjohn <https://github.com/manongjohn>`_ avalaible for `Windows 64-bit, macOS and in appimage format <https://github.com/manongjohn/OTX/releases>`_.


.. _installing_on_windows:

Installing on Windows
---------------------
Execute the OpenToonzSetup.exe file and follow these steps:


1. Choose the language for the installer messages.

 |win_setup_1|
 

2. Accept OpenToonz Terms of Use.

 |win_setup_2| 
 

3. Decide where to install the **OpenToonz stuff** folder and if you wish to overwrite any settings in a preexisting OpenToonz stuff folder in the chosen location (except for user's personal settings, which will always be preserved). 

 |win_setup_3| 
 

4. Decide whether or not to create a desktop icon during the installation process. 

 |win_setup_4| 
 

5. Press the Install button to start the installation process with the chosen settings. 

 |win_setup_5| 
 

6. Decide whether or not to Launch OpenToonz right away after closing the installer. 

 |win_setup_6| 



.. _installing_on_os_x:

Installing on OS X
------------------
Follow these steps:


1. Right-click on the OpenToonz.pkg file in Finder & select Open.


2. Press the Continue button.

 |osx_setup_2| 
 

3. Choose a language and press the Continue button. 

 |osx_setup_3| 
 

4. Press the Agree button to accept the OpenToonz Terms of Use. 

 |osx_setup_4| 
 

5. Select the install destination (will be Macintosh HD unless multiple disks are available) and press the Continue button. 

 |osx_setup_5| 
 

6. Press the Install button to start the installation process with the chosen settings. 

 |osx_setup_6| 


7. Press the Close button to exit the installer. 

 |osx_setup_7| 

Homebrew
''''''''

``brew cask install opentoonz``

.. _installing_on_linux:

Installing on Linux
-------------------

.. _arch:

Arch Linux
''''''''''

``sudo pacman -S base-devel git``

``git clone https://aur.archlinux.org/superlu.git``

``cd superlu``

``makepkg -si``

``cd ..``

``git clone https://aur.archlinux.org/opentoonz.git``

``cd opentoonz``

``makepkg -si``

``export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/lib/opentoonz/``

``echo "export LD_LIBRARY_PATH=\$LD_LIBRARY_PATH:/usr/lib/opentoonz" >> ~/.bashrc``

.. _debian:

Debian GNU/Linux
''''''''''''''''

1. Download PGP signing key package.

``wget http://www.deb-multimedia.org/pool/main/d/deb-multimedia-keyring/deb-multimedia-keyring_2016.8.1_all.deb``

2. Install PGP package.

``sudo dpkg -i deb-multimedia-keyring_2016.8.1_all.deb``

3. Add repository address to your sources list.

``sudo echo "deb http://www.deb-multimedia.org stable main" | tee -a /etc/apt/sources.list`` Builds for testing and sid also avalaible.

.. note:: Debian packages avalaible only for amd64, arm64 and i386 architectures.

4. Install OpenToonz.

``sudo apt update && apt install opentoonz opentoonz-data``

.. tip:: For updating enter ``sudo apt update && apt upgrade``.

Gentoo, Funtoo
''''''''''''''

``sudo emerge media-gfx/opentoonz``

openSUSE
''''''''

``sudo zypper install opentoonz``

Solus
'''''

``sudo eopkg install opentoonz``

Void Linux
''''''''''

``sudo xbps-install -S opentoonz``

.. _universal_binaries:

Universal binaries
''''''''''''''''''

Flatpak
~~~~~~~

1. Installing.

``flatpak install flathub io.github.OpenToonz``

2. Run.

``flatpak run io.github.OpenToonz``

.. _snap:

Snap
~~~~

``sudo snap install opentoonz``

.. |win_setup_1| image:: /_static/installing/windows_setup_1.png
.. |win_setup_2| image:: /_static/installing/windows_setup_2.png
.. |win_setup_3| image:: /_static/installing/windows_setup_3.png
.. |win_setup_4| image:: /_static/installing/windows_setup_4.png
.. |win_setup_5| image:: /_static/installing/windows_setup_5.png
.. |win_setup_6| image:: /_static/installing/windows_setup_6.png
.. |osx_setup_2| image:: /_static/installing/osx_setup_2.png
.. |osx_setup_3| image:: /_static/installing/osx_setup_3.png
.. |osx_setup_4| image:: /_static/installing/osx_setup_4.png
.. |osx_setup_5| image:: /_static/installing/osx_setup_5.png
.. |osx_setup_6| image:: /_static/installing/osx_setup_6.png
.. |osx_setup_7| image:: /_static/installing/osx_setup_7.png

