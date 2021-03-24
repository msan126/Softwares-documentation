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

Go to the website to see the version that you want : https://www.tensorflow.org/install/pip.
Then, you can find the different steps that you need to add on your terminal:

msan126@bn391471:/hpc/msan126$ cd PycharmProjects/tutorial/
msan126@bn391471:/hpc/msan126/PycharmProjects/tutorial$ ls msan126@bn391471:/hpc/msan126/PycharmProjects/tutorial$ cd venv/bin/
msan126@bn391471:/hpc/msan126/PycharmProjects/tutorial/venv/bin$ source activate
(venv) msan126@bn391471:/hpc/msan126/PycharmProjects/tutorial/venv/bin$ pip install tensorflow==1.8
(venv) msan126@bn391471:/hpc/msan126/PycharmProjects/tutorial/venv/bin$ pip install scipy
(venv) msan126@bn391471:/hpc/msan126/PycharmProjects/tutorial/venv/bin$ pip install matplotlib
msan126@bn391471:~$ source /hpc/msan126/PycharmProjects/tutorial/venv/bin/activate
(venv) msan126@bn391471:~$ python
(venv) msan126@bn391471:~$ pip install nibabel
(venv) msan126@bn391471:~$ pip install pydicom


msan126@bn391471:~$ ssh msan126@hpc2
Are you sure you want to continue connecting (yes/no)? y
[msan126@hpc2]nvidia-smi
[msan126@hpc5]watch -n 1 nvidia-smi