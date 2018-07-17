SporPricingForcasting
=====================

A notebook that forecasts Spot Pricing for an instance in Amazon Web Services (AWS). This uses boto3 to retrieve data from Amazon Web Service, organize the data into a dataframe, predict and plot observed and future data using Prophet and Plotly.

Python requirements
-------------------

This notebook was created in Python 3 environment. Make sure the notebook's kernel is set to Python 3. It's preferable to use the latest version of Python (3.6 at the time of this readme).


Instalation
-----------

Installing Boto3
^^^^^^^^^^^^^^^^

The notebook requires boto3 in order to retrieve data from AWS. To install and configure boto, use the following command:

::

	pip install boto3


and `follow the directions <https://boto3.readthedocs.io/en/latest/guide/quickstart.html>`_ in order to setup the proper configurations.


Installing nodejs & ipywidgets
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Before installing `ipywidgets <https://ipywidgets.readthedocs.io/en/latest/user_install.html>`_, you must have `nodejs <https://nodejs.org/en>`_ installed. This is especially for JupyterLab users. To install ipywidgets with pip, use the following commands:

::

	pip install ipywidgets
	jupyter nbextension enable --py widgetsnbextension


with conda:

::

	conda install -c conda-forge ipywidgets

JupyterLab users will need to use an additional command in order for the input widgets to display:

::

	jupyter labextension install @jupyter-widgets/jupyterlab-manager

Users who are having issues installing the widgets for JupyterLab or those who aren't using the latest version should refer to `version compatiblity <https://github.com/jupyter-widgets/ipywidgets/tree/master/packages/jupyterlab-manager#version-compatibility>`_  page and select the command that is compaitible to the version of JupyterLab.

Installing fbprophet
^^^^^^^^^^^^^^^^^^^^

Before installing fbprophet, PyStan must be installed first along with a compiler. `Refer to the installation page <https://facebook.github.io/prophet/docs/installation.html>`_ for more details depending on the operating system.


Installing Plotly
^^^^^^^^^^^^^^^^^

To install Plotly, use the following command:

::

	pip install plotly


JupyterLab users will need to use an additional command in order for the graphs to display:

::

	jupyter labextension install @jupyterlab/plotly-extension
