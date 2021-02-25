.. _managing_projects:

Managing Projects
=================
Projects are an easy way to manage scenes and files used in them. They allow you to organize your production material not only by defining default settings used throughout the production, but also default folders where files will be automatically saved, and from where they will be retrieved when needed. This means that, for example, as soon as you scan drawings, they will be saved automatically in the input default folders you specified for your project. 

The main advantage of managing the production through projects, is that a consistency of production settings and production material can be achieved.

The consistency of production settings is achieved because all the scenes of a projects, as soon as they are created, inherit all the settings from the project (see  :ref:`Setting Up a Scene <setting_up_a_scene>`  ). 

The right use of production material is achieved because once you have defined a production structure through projects, all the scenes are able to save and retrieve files by using the project default folders.

.. _setting_the_projectroot:

Setting the Projectroot
-----------------------

The projectroot is the folder where the project information and database are stored; it is displayed in the OpenToonz browser as one of the main folders with the related path in brackets.

The default value is ``C:\OpenToonz stuff\projects``  on Windows and ``/Applications/OpenToonz/OpenToonz stuff/projects``  on Macintosh.

.. note:: If your production has to be managed on more than one computer on a network, you can share the same project database on all the computers you want, by defining the same projectroot on each computer.


It is also possible to define more than one projectroot if needed: in this case projectroot folders will be visible in the OpenToonz browser, each with the related path in brackets.

 |additional_project_locations|

The projectroot information can be changed at any moment, for instance if you need to move the project database files from one computer to another.

.. tip:: **To set the projectroot on Windows:**

    1. Open the Run application dialog by selecting Run from the Start menu.

    2. Type ``regedit``  in the text box and click OK. This will open the Registry Editor application.

    3. Navigate to the ``HKEY_LOCAL_MACHINE\SOFTWARE\OpenToonz\OpenToonz`` and double-click TOONZPROJECTS in the right part of the window: the Edit String dialog opens.

    4. Enter the new path for the projectroot. 

    5. Click OK and exit from the Registry Editor application.

    6. Restart OpenToonz to make the change effective.

.. tip:: **To add a projectroot on Windows:**

    1. Open the registry editor to edit the TOONZPROJECTS registry as described above.

    2. Enter the path for the new projectroot, separated by a semicolon (e.g. ``C:\production01;D:\production02`` ). 

    3. Click OK and exit from the Registry Editor application.

    4. Restart OpenToonz to make the change effective.

.. tip:: **To set the projectroot on Macintosh:**

    1. Right-click the OpenToonz icon in the ``Applications/OpenToonz`` folder, and choose Show Package Contents from the menu that opens.

    2. In the folder that opens browse to the ``Contents/Resources``  folder and open the ``SystemVar.ini``  file with a text editor application, such as TextEdit.

    3. Look for the following line where the projectroot is defined:
    ``TOONZPROJECTS=”/Applications/OpenToonz/OpenToonz stuff/projects”`` 

    4. Change the path in inverted commas by typing a new one.

    5. Save the ``SystemVar.ini``  file.

.. tip:: **To add a projectroot on Macintosh:**

    1. Open the configuration file to edit the TOONZPROJECTS variable as described above.

    2. Change the path in inverted commas by adding a new path for the new projectroot, separated by a semicolon (e.g. ``/Applications/OpenToonz/OpenToonz stuff/production01`` ``;`` ``/Applications/OpenToonz/OpenToonz stuff/production02`` ). 

    3. Save the ``SystemVar.ini``  file.

    4. Restart OpenToonz to make the change effective.

.. _setting_up_projects:

Setting up Projects
-------------------
 |new_project| 

When you define a new project you can specify its default folders, while its default settings will be inherited from the current project. Default folders and settings can be modified at any time to satisfy new production needs.

Project information is stored in an XML file named as the project with the ``_otprj``  suffix, in a folder named as the project located in the projectroot (see  :ref:`Setting the Projectroot <setting_the_projectroot>`  ).

Projects can be organized in folders and can contain sub-projects that can be browsed in the OpenToonz file browser. This allows you to customize the project structures in order to follow your production needs, for instance creating a folder for each episode, then a project for each scene belonging to that episode. As the project browser will display the project tree and all the folders contained in the projectroot, you can also organize your folder structure in the projectroot by using the OS file system.

There is always one current project selected in the project browser: when you start working on a scene, automatically it will belong to the current project, inheriting its settings and default folders. 

If you want a new scene to be part of a new project, first you have to define a new project. If you want it to be part of a previously created project, first you have to set that project as the current one.

.. note:: If you want to use the farm for rendering scenes, all the server (rendering) nodes of the farm have to share the same projectroot (see  :ref:`Installing the Toonz Farm on Windows <installing_the_toonz_farm_on_windows>`  ) and all the drives containing the projects database, have to be shared on the network.

.. tip:: **To create a new project:**

    1. Choose File  →  Project Management  →  New Project... 

    2. Select the projectroot or repository (see  :ref:`Configuring the Version Control in OpenToonz <configuring_the_version_control_in_toonz>`  ), and the project or folder where you want to create the new project.

    3. Type the name of the project and set the path to the folders you want to use as default. 

    4. Click the **OK** button.

.. tip:: **To change the current project:**

    Click the small round button on the left of the project name in the project tree available in the OpenToonz file browser. It becomes red when selected.

.. tip:: **To add a scene to a project:**

    1. Set the project as the current one.

    2. Choose File  →  New Scene.

.. tip:: **To change project default folders:**

    Select File  →  Project Management  →  Project Settings... and change default folders paths.

.. note:: When changing default folders, scenes previously created in the same project may fail retrieving used files.


.. _project_default_folders:

Project Default Folders
-----------------------
Projects have default folders where scanned drawings, painted drawings, scenes, rendered frames and palettes are automatically saved. These folders are shared by all of the scenes created for that particular project, and are labelled in the following way:

- **+inputs** is the folder where all scanned drawings are saved (as TIF files).

- **+drawings** is the folder where OpenToonz cleaned up drawings, drawings made directly in OpenToonz and imported OpenToonz drawings are saved (TLV and PLI files).

- **+scenes** is the folder where the OpenToonz scenes are saved (TNZ files).

- **+extras** is the folder where all the imported non-OpenToonz levels, images and audio files are saved.

- **+outputs** is the folder where rendered images are saved.

- **+palettes** is the folder where the project palettes of the studio palette are saved, and where the Raster Drawing Palette, shared by all the raster levels belonging to the project, is stored.

For each of these folders you can specify different locations on your computer network depending on the way you set up the storage of your production material. 

Absolute or relative paths can be specified for the default folders definition.

If you specify an absolute path, the folders will be created, when needed, where specified. For example you can set **+drawings** to be ``C:\production\drawings01`` on Windows, or ``/Volume/Macintosh HD/production/drawing01``  on Macintosh: this means that the OpenToonz drawn and cleaned up levels will be automatically saved in ``C:\production\drawings01`` on Windows, or in ``/Volume/Macintosh HD/production/drawing01``  on Macintosh.

If you specify a relative path, all the folders you specify in the path will be created, when needed, in the project folder under the selected projectroot or repository (see  :ref:`Configuring the Version Control in OpenToonz <configuring_the_version_control_in_toonz>`  ). For example, for the project myproject, you can set **+drawings** to be ``sequence01\mydrawings`` : this means that the OpenToonz drawn and cleaned up levels will be automatically saved in the ``myproject\sequence01\mydrawings``  folder located in the selected projectroot or repository. 

The $scenepath variable can also be used to automatically create specific folders according to the scene you are working on. The variable can be either appended to the specified paths, or used in the path definition.

The labels of the default folders you can find in the project settings (i.e. **+drawings**, **+extras**, etc.) can be used as aliases in OpenToonz. For example if some material is retrieved from the extras default folder, its loading path will contain the alias **+extras**. They can be also used when you need to specify a saving path, for example in the Path field of the New Level dialog.

When in a scene you load material not located in the current project folders, you can choose whether to import files, that is to say copy them in the related project folders, or to create a link with the external file. The link is defined by an absolute path. 

.. note:: Files loaded in a scene without importing can be imported later on at once by using the Collect Assets feature (see  :ref:`Collecting Assets <collecting_assets>`  ).

.. note:: All shared disks involved in the folder definitions, i.e. disks where production material has to be written and read, must be shared granting full permissions to any user, otherwise the exchange of files will not succeed. For Windows, disks must have a Share Permission set to Full Control for Everyone; for Macintosh, the sharing settings must allow any user to read from and write to disks.

.. note:: When no project is defined, the ``OpenToonz stuff/sandbox`` project is used by default.

.. tip:: **To set default folders for a new project:**

    Do one of the following: 

    - Type the path to the folder you want to use as default.

    - Use the browser button on the right of each text field, to set the folder you want to use as default.


.. _adding_custom_default_folders:

Adding Custom Default Folders
'''''''''''''''''''''''''''''
Besides the basic default folders you can also add your own default folders, and use the related aliases, by defining a TXT file named ``project_folders.txt``  in the ``OpenToonz stuff\profiles``  folder. In this file you can also change the order of the folders already available to change the way they are listed in the project settings dialog. 

The following is an example of a ``projectfolders.txt``  file:

| inputs
| drawings
| backgrounds
| scenes
| extras
| outputs
| palettes
| 3D

where the **+backgrounds** and **+3D** aliases were added to the default ones.


.. tip:: **To add more default folders to projects:**

    1. Open the ``OpenToonz stuff\profiles\project_folders.txt``  file.

    2. List the default folders you want to define, one per line, and save the file.


.. _using_the_$scenepath_variable_in_folder_definition:

Using the $scenepath Variable in Folder Definition
''''''''''''''''''''''''''''''''''''''''''''''''''
The $scenepath variable can also be used in the definition of the **+inputs**, **+drawings**, and **+extras** aliases when typing the default folder path. In this case the path where you save the current scene will replace the $scenepath variable in the path definition, with the needed folders automatically created during the saving process.

For example if **+drawings** is ``$scenepath\mydrawings,`` and you save the scene scene01 in ``+scenes\seq01`` , OpenToonz drawn or cleaned up levels for that scene will be saved in ``seq01\scene01\mydrawings`` ; when you save the scene scene02, in ``seq01\scene02\mydrawings`` ; and so on. 

In this way the needed default folders are automatically created with the same given name (mydrawings), one for each scene, according to the path used when saving the scene. As a consequence, if the variable is used in this way for all the aliases, all the files related to a scene will be stored in a folder named as the scene.

 |scenepath_variable| 

A second example: if **+drawings** is ``mydrawings\$scenepath,`` when you save the scene scene01 in ``+scenes\seq01`` , OpenToonz drawn or cleaned up levels for that scene will be saved in ``mydrawings\seq01\scene01`` ; when you save the scene scene02, in ``mydrawings\seq01\scene02`` ; and so on. 

In this case the needed default folders are automatically created with the name and path of folders used when saving the scene, inside the path specified (mydrawings). As a consequence, if the variable is used in this way for all the aliases, all the files used in the project will be stored in a main folder for each alias, whose content is divided into folders named as the scenes. 

.. note:: The definition of the **+palettes** alias cannot include $scenepath, as the palettes refer to the whole project, not to specific scenes.

.. note:: It is not possible to use at the same time for an alias the $scenepath variable in folder definition and the Append $scenepath option.


.. _using_the_append_$scenepath_option:

Using the Append $scenepath Option
''''''''''''''''''''''''''''''''''
The Append $scenepath option is available for the **+inputs**, **+drawings** and **+extras** aliases. If you activate the Append $scenepath option for an alias, the path where you save the current scene will be added to the path of the alias, with the needed folders automatically created during the saving process.

For example if **+drawings** is ``mydrawings`` , and you save the scene scene01 in ``+scenes\seq01`` , OpenToonz drawn or cleaned up levels for that scene will be saved in ``mydrawings\seq01\scene01`` ; if you save the scene scene02 in ``+scenes\seq01`` , OpenToonz drawn or cleaned up levels for that scene will be saved in ``mydrawings\seq01\scene02`` ; and so on.

 |append_scenepath| 

This allows OpenToonz to create scene-related folders automatically when saving OpenToonz files or importing external files, while allowing the use of the generic aliases **+drawings**, **+inputs** and **+extras**, no matter where levels are loaded from within the current project.

.. note:: When a scene is saved in the **+scenes** folder, the value for $scenepath is the scene name; for example if you save the scene scene02 in **+scenes**, $scenepath will be scene02.

.. note:: It is not possible to use for an alias the Append $scenepath option and at the same time the $scenepath variable in defining the related folder.


.. _using_the_project_browser:

Using the Project Browser
-------------------------
The project browser is available at the end of the file browser tree. It lists all of the projects that have been created, whose actual location is in the projectroot that was defined in the initial installation of OpenToonz. The projectroot value is displayed in brackets.

The name of the folders which the aliases point to are displayed in blue. 

.. note:: In case more than one projectroot is defined, each will be listed with the related projectroot value in brackets (see  :ref:`Setting the Projectroot <setting_the_projectroot>`  ).

.. _default_folders_with_relative_paths:

Default Folders with Relative Paths
'''''''''''''''''''''''''''''''''''
When default folders are defined by using a relative path, in the project browser you will see all the folders specified in the path under the projectroot, and the project folders tree will be the same of the file system tree. The folders that are the target of the paths are displayed in blue.

For example, for the project Project01, with **+drawings** that is ``section01\prod drawings`` , the project browser will display the following:

Projects
   Project01
      section01
         **prod drawings**

If the option Append $scenepath is activated, and you save the scene scene01 in ``+scenes\seq01`` , the project browser will display the following:

Projects
   Project01
      section01
         prod drawings
            seq01
               **scene01**

If the $scenepath is used in the folder definition, with +drawings that is ``$scenepath\prod drawings,`` and you save the scene scene01 in ``+scenes\seq01`` , the project browser will display the following:

Projects
   Project01
      seq01
         scene01
            **prod drawings**

If the $scenepath is used in the folder definition, with +drawings that is ``mydrawings\$scenepath,`` and you save the scene scene01 in ``+scenes\seq01`` , the project browser will display the following:

Projects
   Project01
      prod drawings
         seq01
            **scene01**


.. _default_folders_with_absolute_paths:

Default Folders with Absolute Paths
'''''''''''''''''''''''''''''''''''
When default folders are defined by using an absolute path, in the project browser you will see only the related aliases, whatever their location on the network is. In this way you can quickly access the production material without browsing the computer, or the network. The aliases are displayed in blue, because they are the location the default folders paths point to.

For example, for the project Project01, with **+drawings** that is ``C:\production\prod drawings`` on Windows, or ``/Volume/Macintosh HD/production/prod drawings`` on Macintosh, the project browser will display the following:

Projects
   Project01
      **+drawings**

where **+drawings** is an alias for ``C:\production\prod drawings`` on Windows, or ``/Volume/Macintosh HD/production/prod drawings`` on Macintosh.

If the option Append $scenepath is activated, and you save the scene scene01 in ``+scenes\seq01`` , the project browser will display the following:

Projects
   Project01
      \+drawings \
         seq01
            **scene01**

If the $scenepath is used in the folder definition, with **+drawings** that is ``C:\$scenepath\prod drawings`` on Windows, or ``/Volume/Macintosh HD/$scenepath/prod drawings`` on Macintosh, and you save the scene scene01 in ``+scenes\seq01`` , the project browser will display the following:

Projects
   Project01
      \+scenes \
         scene01.tnz
            **+drawings**

with **+drawings** that is ``C:\seq01\scene01\prod drawings`` on Windows, or ``/Volume/Macintosh HD/seq01/scene01/prod drawings`` on Macintosh, and is located under the related scene file (TNZ format).

If the $scenepath is used in the folder definition, with **+drawings** that is ``C:\prod drawings\$scenepath`` on Windows, or ``/Volume/Macintosh HD/prod drawings/$scenepath`` on Macintosh, and you save the scene scene01 in ``+scenes\seq01`` , the project browser will display the same as above, but this time **+drawings** is ``C:\prod drawings\seq01\scene01`` on Windows, or ``/Volume/Macintosh HD/prod drawings/seq01/scene01`` on Macintosh.



.. |additional_project_locations| image:: /_static/managing_projects/additional_project_locations.png
.. |new_project| image:: /_static/managing_projects/new_project_dialog.png
.. |scenepath_variable| image:: /_static/managing_projects/scenepath_variable.png
.. |append_scenepath| image:: /_static/managing_projects/append_scenepath.png

.. |additional_project_locations_es| image:: /_static/managing_projects/es/additional_project_locations.png
.. |new_project_es| image:: /_static/managing_projects/es/new_project_dialog.png
