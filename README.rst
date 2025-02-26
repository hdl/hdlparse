
========
Hdlparse
========

Hdlparse is a simple package implementing a rudimentary parser for VHDL and Verilog. It is not capable of fully parsing the entire language. Rather, it is meant to extract enough key information from a source file to create generated documentation.

This library is forked from `kevinpt <https://github.com/kevinpt/hdlparse>`_ via `zhelnio <https://github.com/zhelnio/hdlparse>`_. The aim of this fork is to provide some bug fixes and additional features to zhelnio's version of Hdlparse. A list of changes is included at the bottom of this README.

For VHDL this library can extract component, subprogram, type, subtype, and constant declarations from a package. For Verilog it can extract module declarations (both 1995 and 2001 syntax).


Requirements
------------

Hdlparse requires Python 3.x and no additional libraries. This version of Hdlparse is not compatible with Python2.


Download
--------

You can access the Hdlparse Git repository from `Github
<https://github.com/hdl/pyhdlparser>`_. You can install direct from PyPI with the "pip"
command if you have it available.

Installation
------------

Hdlparse is a Python library. You must have Python installed first to use it. Most modern Linux distributions and OS/X have it available by default. There are a number of options available for Windows. If you don't already have a favorite, I recommend getting one of the `"full-stack" Python distros <http://www.scipy.org/install.html>`_ that are geared toward scientific computing such as Anaconda or Python(x,y).

You need to have the Python setuptools installed first. If your OS has a package manager, it may be preferable to install setuptools through that tool. Otherwise you can use Pip:

.. code-block:: sh

  > pip install setuptools

If you don't have ``pip`` you may have the ``easy_install`` command available which can be used to install ``pip`` on your system:

.. code-block:: sh

  > easy_install pip

You can use ``pip`` to get the latest development code from Github:

.. code-block:: sh

  > pip install --upgrade https://github.com/hdl/pyhdlparser/tarball/master

If you manually downloaded a source package or created a clone with Git you can install with the following command run from the base Hdlparse directory:

.. code-block:: sh

  > python setup.py install

On Linux systems you may need to install with root privileges using the *sudo* command.

After a successful install the Hdlparse library will be available.


Documentation
-------------

The full documentation is available online at the `main Hdlparse site
<http://kevinpt.github.io/hdlparse/>`_.


Changes
-------

A list of changes compared to the upstream is listed here:

* Improved support for VHDL and Verilog generics
* PEP8 compatible formatting
* Remove Python2 support
* Provide debugging information using the Python logging module
