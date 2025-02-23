=========
toolchest
=========


.. image:: https://img.shields.io/pypi/v/toolchest.svg
        :target: https://pypi.python.org/pypi/toolchest

.. image:: https://github.com/release-depot/toolchest/actions/workflows/test.yml/badge.svg
        :target: https://github.com/release-depot/toolchest/actions

.. image:: https://readthedocs.org/projects/toolchest/badge/?version=latest
        :target: https://toolchest.readthedocs.io/en/latest/?badge=latest
        :alt: Documentation Status




Toolchest is a collection of generally useful functions that can be reused in
various settings.

Find the most recent documentation at https://toolchest.readthedocs.io.

Notes
-----

This library only supports python 3. Some features may still work with python 2.7 but not all of the
syntax and features may be compatible. Prettytable can be used, but is optional.


Installing
----------

toolchest is available on PyPI; it can be installed by running::

  pip install toolchest

Alternatively, one could also clone this repository and run::

  pip install --editable .


Development
-----------

toolchest supports both standard python virtual environment setups and pipenv,
which is integrated into our Makefile. To set up a pipenv-based development
enironment, you can simply run::

  make dev

This will install our dev environment for the package via pipenv.  It is installed
with --user, so it does not affect your site-packages.  Pipenv creates a unique virtualenv
for us, which you can activate via::

  pipenv shell

See the `pipenv documentation <https://docs.pipenv.org/>`_ for more detail.

Documentation
*************

To build the documentation on your checkout, simply run::

  make docs

Contributing
*************

All new code should include tests that exercise the code and prove that it
works, or fixes the bug you are trying to fix.  Any Pull Request without tests
will not be accepted. See CONTRIBUTING.rst for more details.

Building
********

If you wish to build a local package for testing at any time, you can simply
run::

  make dist

this will build a package with a .dev extension that you can install for testing
and verification.

Acknowledgements
----------------

This code contains a derivative work of 'rpmvercmp' from RPM 4.14.1.
