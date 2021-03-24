********
ITK-Snap
********

.. toctree::
   :maxdepth: 2


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
