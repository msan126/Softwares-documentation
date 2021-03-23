************
Installation
************

.. toctree::
   :maxdepth: 2

======================
Segmentation softwares
======================

MITK
----

First, install MITK.

* For Windows, follow this `link <https://www.mitk.org/download/releases/MITK-2018.04.2/Windows/MITK-v2018.04.2-windows-x86_64.exe>`_
Then, install it.
* For Linux, donwnload the `software <https://www.mitk.org/download/releases/MITK-2018.04.2/Linux/MITK-v2018.04.2-linux-x86_64.tar.gz>`_
Extract the data in the chosen folder and then open a new terminal.

.. code-block:: python
    cd /hpc/msan126/usr/MITK-v2018.04.2-linux-x86_64/
    ./MitkWorkbench.sh


ITK-Snap
--------

* For Windows, download it on the `website <http://www.itksnap.org/pmwiki/pmwiki.php?n=Downloads.SNAP2>`_.Then, install it.
* For Linux, download the `Linux Binary <http://www.itksnap.org/pmwiki/pmwiki.php?n=Downloads.SNAP3>`_(64 bit, Qt4).
Then, download this `package <https://packages.ubuntu.com/xenial/libpng12-0>`_ .Compile it and install it in a new terminal :

.. code-block:: python
    cd libpng-1.2.54
    ./autogen.sh
    ./configure
    make -j8
    make install
    ldconfig
    cd ../itksnap/
    ls
    cd itksnap-3.8.0-20190612-Linux-gcc64/
    cd bin/
    ./itksnap
    export LD_LIBRARY_PATH=/hpc/msan126/usr/libpng/libpng-1.2.54/lib:$LD_LIBRARY_PATH
    ./itksnap


Seg3D
-----

* For Windows, download it on the `website <https://www.paraview.org/download/>`_. Follow the instructions and install it.
* For Linux, download the Linux version corresponding to your Pycharm on the following `link <https://www.paraview.org/download/>`_
Then, cut it and put it on your hpc.

.. code-block:: python
    cd /hpc/msan126/usr/ParaView-5.7.0-MPI-Linux-Python3.7-64bit/bin
    ./paraview


Paraview
--------

* For Windows, download it on the `website <https://www.paraview.org/download/>`_. Follow the instructions and install it.
* For Linux, download the Linux version corresponding to your Pycharm on the following `link <https://www.paraview.org/download/>`_
Then, cut it and put it on your hpc.

.. code-block:: python
    cd /hpc/msan126/usr/ParaView-5.7.0-MPI-Linux-Python3.7-64bit/bin
    ./paraview


To read nifti files, you need to go on Tools then Manage Plugins, click on AnalyzeNIfTIReaderWriter and then select Auto
Load. To apply it, click on Load Selected. After that to add MRI, select it in the folder and click-right on it :
Extract Here. Then, you can return on the software and open the file.
If you want more information, you can find a lot of tutorials.

