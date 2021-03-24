***********
Tensorboard
***********

.. toctree::
   :maxdepth: 2

Linux
*****

Tensorboard is a tool often used in machine learning. It provides measurements and visualizations during the machine
learning workflow. It could present graphs and tables for metrics like loss or accuracy.
This quickstart will show you how to quickly get dealt with these metrics.

Firstly, open a new terminal with the path associated to the code project. Then, activate the virtual environment:

.. code-block:: python
    source    hpc/user/PycharmProjects/tutorial/venv/bin/activate
    #(venv) the virtual environment is activated
    tensorboard --logdir= #path where the data is located

Then, click on the link appeared in the terminal.
