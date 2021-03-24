********
Paraview
********

.. toctree::
   :maxdepth: 2

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