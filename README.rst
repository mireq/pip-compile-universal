==================================================================
Compile with pip-tools for multiple python versions in single file
==================================================================

This package allows to compile ``requirements.in`` file to single
``requirements.txt`` output with support for multiple python versions
simultaneously.

Install
-------

.. code:: bash

	pip install pip-compile-universal

Usage
-----

Call this command with required python versions, first input file and rest
arguments forwarded to pip-tools.

.. code:: bash

	pip_compile_universal 3.8,3.9,3.10,3.11 requirements.in [other pip-tools arguments]

How it works
------------

This command creates virtualenvs in home directory (``~/.virtualenvs``). Then it
will compile requirements for each python version and merge to single
``requirements.txt`` file.

Example
-------


``requirements.in``:

.. code::

	workalendar


.. code:: bash

	pip_compile_universal 3.7,3.8,3.9,3.10,3.11 requirements.in

``requirements.txt``:

.. code::

	backports-zoneinfo==0.2.1 ; python_version < "3.9"
	    # via workalendar
	convertdate==2.4.0
	    # via workalendar
	importlib-metadata==6.0.0 ; python_version < "3.8"
	    # via workalendar
	lunardate==0.2.0
	    # via workalendar
	pyluach==2.0.2
	    # via workalendar
	pymeeus==0.5.12
	    # via convertdate
	python-dateutil==2.8.2
	    # via workalendar
	six==1.16.0
	    # via python-dateutil
	typing-extensions==4.4.0 ; python_version < "3.8"
	    # via importlib-metadata
	workalendar==17.0.0
	    # via -r build/requirements.in
	zipp==3.12.0 ; python_version < "3.8"
	    # via importlib-metadata
