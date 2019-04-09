# python_package_template

Template with high-level guidelines for making new CEDA Python packages

Also includes a sample Sphinx documentation in ``docs/`` directory.  Run
``make`` in that directory to see a list of targets.  Further instructions are
in ``docs/index.rst``.

## Based on Cookiecutter package

This is based on the `Cookiecutter PyPackage` that gets used as the template:

 https://github.com/audreyr/cookiecutter-pypackage

It gets used by the `Cookiecutter` package:

 https://github.com/audreyr/cookiecutter

Cookiecutter_ template for a Python package.

Notes on `Cookiecutter PyPackage`:

 * GitHub repo: https://github.com/audreyr/cookiecutter-pypackage/
 * Documentation: https://cookiecutter-pypackage.readthedocs.io/
 * Free software: BSD license

Features
--------

 * Testing setup with ``unittest`` and ``python setup.py test`` or ``py.test``
 * Travis-CI_: Ready for Travis Continuous Integration testing
 * Tox_ testing: Setup to easily test for Python 2.7, 3.4, 3.5, 3.6
 * Sphinx_ docs: Documentation ready for generation with, for example, ReadTheDocs_
 * Bumpversion_: Pre-configured version bumping with a single command
 * Auto-release to PyPI_ when you push a new tag to master (optional)
 * Command line interface using Click (optional)


Quickstart
----------

Install the latest Cookiecutter if you haven't installed it yet (this requires
Cookiecutter 1.4.0 or higher)::

    pip install -U cookiecutter

Generate a Python package project::

    cookiecutter https://github.com/audreyr/cookiecutter-pypackage.git

Then:

 * Create a repo and put it there.
 * Add the repo to your Travis-CI_ account.
 * Install the dev requirements into a virtualenv. (``pip install -r requirements_dev.txt``)
 * Register_ your project with PyPI.
 * Run the Travis CLI command `travis encrypt --add deploy.password` to encrypt your PyPI password in Travis config
  and activate automated deployment on PyPI when you push a new tag to master branch.
 * Add the repo to your ReadTheDocs_ account + turn on the ReadTheDocs service hook.
 * Release your package by pushing a new tag to master.
 * Add a `requirements.txt` file that specifies the packages you will need for
  your project and their versions. For more info see the `pip docs for requirements files`_.
 * Activate your project on `pyup.io`_.


For more details, see the `cookiecutter-pypackage tutorial`:

 https://cookiecutter-pypackage.readthedocs.io/en/latest/tutorial.html
  

