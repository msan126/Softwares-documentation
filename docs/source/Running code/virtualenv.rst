*******
Vitual environment
*******

.. toctree::
   :maxdepth: 2

=======
Linux
=======

Creation
-------------------------------------------

[msan126@hpc2]virtualenv --system-site-packages -p python3 ./tensorflow1_12HPC2
[msan126@hpc2]source ./tensorflow1_12HPC2/bin/activate

(tensorflow1_12HPC2) [msan126@hpc2]pip install libconf
(tensorflow1_12HPC2) [msan126@hpc2]pip install tensorflow-gpu==1.12
(tensorflow1_12HPC2) [msan126@hpc2]python3
>>> import tensorflow
>>> quit()

If you need more information, go on the website:
https://www.tensorflow.org/install/pip

Installation of complements like tensorflow, scihub...
-------------------------------------------

Go on the site to see the version that you want : https://www.tensorflow.org/install/pip.
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

=======
Windows
=======

Creation
-------------------------------------------

To install a virtual environment for your Python, follow the next steps:

* Open the command prompt, and execute it:

```bash
pip install virtualenv
```

* If you are working on Windows, execute in the command prompt the next step:

```bash
pip install virtualenvwrapper-win (only for windows)
```

* Now, create the virtual environment:

```bash
mkvirtualenv scaffold-venv36
```

* Then, activate the virtual environment and make sure it is still activate for the entire time
you are installing the following tools. Two possibilities:

      *  If you are working on Windows, execute in the command prompt the next step:

```bash
workon scaffold-venv36
```
      *  If you are working on Linux or Mac, execute in the command prompt the next step and complete it:
```bash
source [folder]/activate
```