.. _using_the_toonz_farm:

Using the Toonz Farm
====================
The Toonz Farm allows you to process OpenToonz scenes submitted as cleanup tasks or render tasks in the task list by using a series of computers connected on the same network using TCP/IP (see  :ref:`Cleaning up Drawings in Batch Mode <cleaning_up_drawings_in_batch_mode>`  and  :ref:`Rendering Scenes in Batch Mode <rendering_scenes_in_batch_mode>`  ). 

When tasks are executed, they are automatically assigned to the computers belonging to the farm in order to balance the workload. When all computers are busy, remaining tasks are not assigned until a machine is ready to process them. 

.. note:: If you have divided a render task into *chunks*, each chunk will be assigned to a different computer of the farm, thus speeding up the rendering of a single render task (see  :ref:`Using Chunks when Rendering Tasks <using_chunks_when_rendering_tasks>`  ).

The Toonz Farm is composed by the following:

- **Controller node**: is the computer that dispatches the tasks to server (rendering) nodes. This computer runs the controller program, named ``tfarmcontroller.exe``  on Windows and ``tfarmcontrollerd``  on Macintosh. One controller node is needed for defining a farm. 

 .. note:: The controller node can also be used as a server (rendering) node.

- **Server (rendering) nodes**: are the computers that execute tasks dispatched by the controller. Each of these computers runs a server program, named ``tfarmserver.exe``  on Windows and ``tfarmserverd``  on Macintosh, that is in charge of running tasks, notifying the controller when a task has been completed, etc. 

- **Root folder** named FARMROOT: is a shared folder where a number of configuration files are stored. The controller node and all the rendering nodes must be able to access this shared folder (see  :ref:`Configuring the Toonz Farm <configuring_the_toonz_farm>`  ).

- **Client program**: is the program run by the user to queue new tasks and to monitor the Toonz Farm. OpenToonz itself is the client program of the Toonz Farm, and can be run on any computer on the network, not necessarily on a controller node or a sever (rendering) node. 

.. note:: In order to render the scenes successfully all the computers involved in the Toonz Farm, controller, servers and clients have to share the same projectroot folders (see  :ref:`Setting the Projectroot <setting_the_projectroot>`  ).


.. _installing_the_toonz_farm_on_windows:

Installing the Toonz Farm on Windows
------------------------------------
To install the Toonz Farm, you have to install the Farm Controller component on the controller node, and the Farm Server component on the server (rendering) nodes.

.. note:: If you want to use a computer both as controller and as server (rendering) node, you have to install both the components.

During the installation of any of the components you must specify the full-path of the FARMROOT folder. This path must be expressed using the UNC format, like the following:

``\\HostName\ShareName\FolderName`` 

The drive where the FARMROOT folder is located has to be shared on the network, giving full control to any user by setting the right permissions.

When you choose to install the Farm Controller component, the installation program will create for the controller program a Windows Service, named **Toonz Farm Controller**.

When you choose to install the Farm Server component, the installation program will create for the server program a Windows Service, named **Toonz Farm Server**.

.. note:: As the Toonz Farm requires exchanges of data between computers in the network by using TCP/IP protocol, any firewall system that may block access on computer ports has to be disabled.


.. _setting_the_controller_node:

Setting the Controller Node
'''''''''''''''''''''''''''
On the controller node the controller component is installed as a Windows service, named **Toonz Farm Controller**. By default a Windows Service runs under the security credentials of the Local System account. By default this account is not granted the right to access folders shared by remote hosts.

Since the **Toonz Farm Controller** needs to access the FARMROOT folder, typically shared by a remote host, please run this service as a user with the proper rights. 

.. note:: It is possible to start the service from a DOS shell by navigating to the folder where the binaries of OpenToonz are installed, and then using the following command line:``tfarmcontroller -console`` 

.. tip:: **To run the Toonz Farm Controller as a user with the proper rights:**

    1. Choose Control Panel  →  Administrative Tools  →  Services, and right-click the **Toonz Farm Controller** service to open the Properties panel.

    2. Select the Log On page, check the **This Account:** option.

    3. Choose the network where the Toonz Farm is going to work and set an account that has administrator rights on that network. Insert and confirm the related password.

    4. Click the **OK** button.


.. _setting_the_server_nodes:

Setting the Server Nodes
''''''''''''''''''''''''
On the server (rendering) nodes, the server component is installed as a Windows service, named **Toonz Farm Server**. By default a Windows Service runs under the security credentials of the Local System account. By default this account is not granted the right to access folders shared by remote hosts.

Since the **Toonz Farm Server**, for rendering purposes, needs to access one or more folders shared by remote hosts, please run this service as an user with the proper rights. 

.. note:: It is possible to start the service from a DOS shell by navigating to the folder where the binaries of OpenToonz are installed, and then using the following command line:``tfarmserver -console`` 

.. tip:: **To run the Toonz Farm Controller as an user with the proper rights:**

    1. Choose Control Panel  →  Administrative Tools  →  Services, and right-click the **Toonz Farm Server** service to open the Properties panel.

    2. Select the Log On page, check the **This Account:** option.

    3. Choose the network where the Toonz Farm is going to work and set an account that has administrator rights on that network. Insert and confirm the related password.

    4. Click the **OK** button.


.. _installing_the_toonz_farm_on_macintosh:

Installing the Toonz Farm on Macintosh
--------------------------------------
To install the Toonz Farm, you have to install the Farm Controller component on the controller node, and the Farm Server component on the server (rendering) nodes. 

.. note:: If you want to use a computer both as controller and as server (rendering) node, you have to install both the components.

After the installation of the toonz farm components, a FARMROOT folder has to be defined, and on all the computers belonging to the farm, both controller and servers, the full-path of the FARMROOT folder has to be specified.

To define the FARMROOT folder you can take as model the ``toonzfarm``  folder stored in ``OpenToonz stuff``. You can take the ``toonzfarm``  folder from any computer where OpenToonz in installed, choose the location you prefer, and share it on the network, giving full control to any user by setting the right permissions.

To specify the path to the FARMROOT on the computers, both controller and servers, belonging to the farm, you have to edit the ``configfarmroot.txt``  file by typing in it the full path to the FARMROOT folder.

To retrieve this file open the ``Applications/OpenToonz`` folder, right-click the OpenToonz icon and choose Show Package Contents from the menu that opens; in the folder that opens browse to the ``Contents/Resources``  folder and retrieve the ``configfarmroot.txt``  file.

.. note:: As the Toonz farm requires exchanges of data between computers in the network by using TCP/IP protocol, any firewall system that may block access on computer ports has to be disabled.


.. _configuring_the_toonz_farm:

Configuring the Toonz Farm
--------------------------
Once the installation has been completed, you have to configure the Toonz Farm by editing some configuration files stored in the FARMROOT folder.

The FARMROOT folder must be accessible by all the nodes that compose the Toonz Farm: the controller node, the server (rendering) nodes and the computers running OpenToonz. This means that the drive where the FARMROOT folder is located has to be shared on the network, and the permissions for users have to be maximum, in order to give full control to any users.

For the same reason the computer where the FARMROOT is located has to be started before all the other computers involved in the farm.

The FARMROOT folder contains the following:

- the ``config``  folder containing the ``servers.txt`` , the ``controller.txt`` and the ``id.txt`` .

- the ``logs``  folder.

The ``controller.txt`` and the ``servers.txt``  configuration files must be edited to define the controller node and the server (rendering) nodes before using the Render Farm.


.. _defining_the_controller_node:

Defining the Controller Node
''''''''''''''''''''''''''''
The controller node is defined in the ``controller.txt`` configuration file placed in the ``FARMROOT\config``  folder. 

The file must contain a single text line that describes the node you want to use as a controller.

For the controller node you must specify the following:

- Computer name. 

- IP address. 

- The port number you intend to use for the controller service. 

.. note:: Be sure that the port you set is not blocked by any firewall system, and is open for all the computers belonging to the Toonz farm.

Each of the above information must be separated by a single space. Here is an example of a ``controller.txt``  file:



::

    render1 10.10.0.130 10000

In the above example, ``render1``  is the controller node, its IP address is ``10.10.0.166``  and the controller program runs on the ``10000``  port.


.. _defining_the_server_nodes:

Defining the Server Nodes
'''''''''''''''''''''''''
The server (rendering) nodes are defined in the ``servers.txt``  configuration file placed in the ``FARMROOT\config``  directory.

The file must contain a text line for every computer you want to use as a server (rendering) node.

For each sever (rendering) node you must specify the following:

- Computer name.

- IP address. 

- The port number you intend to use for the server service.

.. note:: Be sure that the port you set is not blocked by any firewall system, and is open for all the computers belonging to the Toonz Farm.

The above information must be separated by a single space. Here is an example of a ``servers.txt``  file::

 render1 10.10.0.166 8002
 render2 10.10.0.195 8002
 render3 10.10.0.111 8002
 render4 10.10.0.180 8002


In the above example, ``render1``  is a server node whose IP address is ``10.10.0.166``  and the server program runs on the ``8002``  port; ``render2``  is a server node whose IP address is ``10.10.0.195``  and the server program runs on the ``8002``  port; etc.

If you want to add or remove a server (rendering) node from the ``servers.txt``  file, you have to restart the controller node in order to make the changes effective.


.. _defining_the_toonz_farm_in_toonz:

Defining the Toonz Farm in OpenToonz
''''''''''''''''''''''''''''''''''''
OpenToonz is the Toonz Farm client program: it allows you to submit new tasks and monitor the status of the farm. 

If the computer where you run OpenToonz is a controller or a server (rendering) node for the Toonz Farm, no further settings are required. 

If the computer is neither a controller nor a server (rendering) node for the Toonz Farm, the FARMROOT has to be defined.

.. tip:: **To define the FARMROOT in OpenToonz:**

    1. Run OpenToonz and go to the **Farm** room.

    2. In the Batch Servers pane, set the **Process with:** option menu to **Render Farm**.

    3. In the dialog that opens specify the full path to the **FARMROOT** folder.

    4. Click the **OK** button.


Using the Toonz Farm
--------------------
In OpenToonz you can find the **Farm** room that allows you to monitor the farm processes. This room contains two main windows: the Tasks window and the Batch Servers window.

The render farm can be monitored by using both the Tasks pane, where the list of tasks can be managed and executed, and the Servers pane, where the computers executing the tasks can be managed.

.. note:: All shared disks involved in the task processing, i.e. disks where files resulting from the task execution have to be written, must be shared granting *full permissions* to any user, otherwise tasks execution will not succeed. For Windows, disks must have a Share Permission set to Full Control for Everyone; for Macintosh, the sharing settings must allow any user to read from and write to disks.


.. _monitoring_the_server_nodes:

Monitoring the Server Nodes
'''''''''''''''''''''''''''
The Batch Servers pane is divided in three areas: at the top there’s an option menu to set whether the tasks execution has to be performed with the Local computer or with the Render Farm; then there is the list of server (rendering) nodes in the farm; at the bottom you can see information about the server currently selected in the list. 

The server (rendering) nodes included in the list are those defined in the ``server.txt``  configuration file (see  :ref:`Defining the Server Nodes <defining_the_server_nodes>`  ). If a server node is down at the controller startup, it will not be available in the farm: this means that all the server nodes *must be up before* starting up the controller node. For the same reason if you want to restart or shut down a server (rendering) node, you have to restart the controller node in order to make the changes effective.

If the **Process with:** option menu is set to **Local**, all the tasks you run will be executed by the local computer; if it's set to **Render Farm**, the tasks will be executed by the Toonz Farm.

.. note:: When you select **Render Farm** you could be prompted to define the **FARMROOT** (see  :ref:`Defining the Toonz Farm in Toonz <defining_the_toonz_farm_in_toonz>`  ). 

When a server is selected in the list, the following related information are displayed in the area at the bottom of the window:

- **Name:** displays the name of the server (rendering) node. 

- **IP Address:** displays its IP address.

- **Port Number:** displays the port number used to exchange data with the farm.

- **Tasks:** displays the task being executed.

- **State:** displays if the server is **Ready**, **Busy** or **Down**. 

 .. note:: A server node state may be down if the server port you set is blocked by a firewall system, and is not open for all the computers belonging to the Toonz Farm (see  :ref:`Defining the Server Nodes <defining_the_server_nodes>`  ).

- **Number of CPU:** displays the number of CPUs available on the server.

- **Physical Memory:** displays the amount of physical memory available on the server.

.. tip:: **To use the Local computer to execute tasks:**

    Set the **Process with:** option menu to **Local**.

.. tip:: **To use the Toonz Farm to execute tasks:**

    Set the **Process with:** option menu to **Render Farm**.


.. _checking_the_toonz_farm_processing:

Checking the Toonz Farm Processing
''''''''''''''''''''''''''''''''''
When the Toonz Farm is used, any problem that may be experienced during the processing is recorded in LOG files, that can be opened and used to diagnose problems.

The LOG files are saved in the ``OpenToonz stuff\toonzfarm``  folder of the computer experiencing the problem; each LOG refers to the processing performed by that computer only.

The LOG files that may be generated by the Toonz Farm processing are the following:

- **server.log** logs all the operations concerning the server computer activity. 

- **controller.log** logs all the operations concerning the controller computer activity. 

- **tcomposer.log** logs all the operations concerning the render activity performed by the server computers. 

- **tcleanup.log** logs all the operations concerning the cleanup activity performed by the server computers. 

