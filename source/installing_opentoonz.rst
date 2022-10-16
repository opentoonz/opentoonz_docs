.. _installing_opentoonz:

Installing OpenToonz
====================


.. _downloading_opentoonz:

Downloading OpenToonz
---------------------
You can download the appropriate version of OpenToonz for your operating system from the `Download page <https://opentoonz.github.io/e/download/opentoonz.html>`_ in the official OpenToonz web site. Choose either the Windows or macOS version to start downloading the installer application.

At the bottom of that same page it's also possible to find the developer's "Nightly Builds" (new versions of the software compiled each night for testing purposes), with which you will be able to try out the latest features and bug fixes, as they are being included in OpenToonz.

.. note:: WARNING: Use at you own risk! A Nightly Build version could potentially be an unstable one, so it is not adviced nor supported, for use in production environments.

.. note:: All other builds apart from the ones downloaded from the official web site ARE NOT officially supported by OpenToonz.

`Morevna Project <https://github.com/morevnaproject>`_ provides builds for `Windows 32-bit, Windows 64-bit, macOS, and appimage <https://github.com/morevnaproject/opentoonz/releases>`_ as well as `snap <https://snapcraft.io/opentoonz-morevna>`_ for Linux.

Finally, there's also an OpenToonz fork called `Tahoma2D <https://tahoma2d.org>`_ avalaible for Windows, macOS and Linux, that could represent a good alternative for certain use cases, where it could be possible to find slightly different approaches to some of the core features in the software, as well as its own new solutions and tools.

All in all, the OpenToonz ecosystem is an open, diverse and fluid one, which means that most novel features, improvements and fixes developed for one of its variants, would most probably end up appearing in the other ones too, within time.



.. _installing_on_windows:

Installing on Windows
---------------------
Execute the OpenToonzSetup.exe file and follow these steps:

.. note:: Microsoft Defender's Smart Screen might alert that the installer is not signed. Just click on the "Run anyway" button (select "More info" to make it visible) to proceed with the installation.

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


Chocolatey
''''''''''

``choco install opentoonz``

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

.. _alt:

ALT Linux
'''''''''

``# apt-get install opentoonz opentoonz-doc``

.. _arch:

Arch Linux
''''''''''

``# pacman -S opentoonz``

.. _debian:

Debian GNU/Linux
''''''''''''''''

1. Download PGP signing key package.

``wget http://www.deb-multimedia.org/pool/main/d/deb-multimedia-keyring/deb-multimedia-keyring_2016.8.1_all.deb``

2. Install PGP package.

``sudo dpkg -i deb-multimedia-keyring_2016.8.1_all.deb``

3. Add repository address to your sources list.

``echo "deb http://www.deb-multimedia.org stable main" | sudo tee -a /etc/apt/sources.list`` Builds for testing and sid also avalaible.

.. note:: Debian packages avalaible only for amd64, arm64 and i386 architectures.

4. Install OpenToonz.

``sudo apt update && apt install opentoonz opentoonz-data``

.. tip:: For updating enter ``sudo apt update && apt upgrade``.

Fedora
''''''

``# dnf install opentoonz``

Gentoo
''''''

``sudo emerge media-gfx/opentoonz``

NixOS
'''''

``nix-env -iA nixos.opentoonz``

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

.. _installing_on_freebsd:

Installing on FreeBSD
---------------------

``# cd /usr/ports/multimedia/opentoonz && make install clean``

.. _installing_on_dragonflybsd:

Installing on DragonFly BSD
---------------------------

``# pkg install opentoonz``

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

