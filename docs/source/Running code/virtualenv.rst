******************
Virtual environment
******************

.. toctree::
   :maxdepth: 2


Linux
######

To create a new virtual environment, you have two possibilities. A new virtual environment can be created on hpc or
on your local machine. Select the place you want it, then open a new terminal and follow the next steps.

.. code-block:: python
    virtualenv --system-site-packages -p python3 ./tensorflow[version]
    source ./tensorflow[version]/bin/activate

Then, add the libraries needed to run your project, for example:

.. code-block:: python
    pip install libconf
    pip install tensorflow-gpu==1.12
    python3
    >>> import tensorflow
    >>> quit()

If you need more information, go on the `website <https://www.tensorflow.org/install/pip>`_.


Windows
#######

To install a virtual environment for your Python, follow the next steps. It is supposed Python is already installed, if
it is not already done, go to the Pycharm Section.

* Open the command prompt, and execute it:

.. code-block:: python
    pip install virtualenv

* If you are working on Windows, execute in command prompt the next step:

.. code-block:: python
    pip install virtualenvwrapper-win

* Now, create the virtual environment:

.. code-block:: python
    mkvirtualenv scaffold-venv36

* Then, activate the virtual environment and make sure it is still activated for the entire time, you need it. Execute
in the command prompt the next step:

.. code-block:: python
    workon scaffold-venv36