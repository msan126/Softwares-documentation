*******
Pycharm
*******

.. toctree::
   :maxdepth: 2

Installation
############

Linux
*****

Firstly, download it on the `website Jetbrains <https://www.jetbrains.com/fr-fr/pycharm/download/#section=linux>`_ and unpack it. Move it to the file ‘usr’.
Open a terminal and write :
.. code-block:: python
    cd /hpc/[UPI]/usr/pycharm-community-2019.1.3/bin
    ./pycharm.sh

Write gedit ~/.bashrc to open a file in the gedit file editor and write :
export PATH=/hpc/msan126/usr/pycharm-community-2019.1.3/bin:$PATH to add it on the existing path. Open another terminal:

.. code-block:: python
    pycharm.sh

Open another terminal :
.. code-block:: python
    ssh -X hpc6
    #- ssh is a security protocol to be connected with the other linux machines

Put yes and then write your password. Add on the gedit file editor in the top of the page :
export https_proxy=http://proxy.bioeng.auckland.ac.nz:8080
export http_proxy=http://proxy.bioeng.auckland.ac.nz:8080
Now, you can use the bash language and test the commands : uname -s, uname, uname -n to retrieve the name of your station.
Then, open another terminal :
.. code-block:: python
    uname -n

You have the name of your station.To open it the next time, you just have to write:
.. code-block:: python
    [UPI]@bn391471:/hpc_htom/msan126/usr/pycharm-community-2019.1.3$ pycharm.sh


Windows
*******

Download it on the `website Jetbrains <https://www.jetbrains.com/fr-fr/pycharm/download/#section=windows>`_ and unpack it.
Then follow the instructions on the downloading window.


Installation of complements like tensorflow, scihub...
######################################################

Go to the `website <https://www.tensorflow.org/install/pip>`_ to check the required version. Then, write in a new terminal the next steps.

.. code-block:: python
    cd PycharmProjects/tutorial/ #this is the path for the created project
    cd venv/bin/
    source activate
    pip install tensorflow==1.8
    pip install scipy
    pip install matplotlib

You can also directly enter the path and add the librairies.
.. code-block:: python
    source /hpc/[upi]]/PycharmProjects/tutorial/venv/bin/activate
    pip install nibabel
    pip install pydicom