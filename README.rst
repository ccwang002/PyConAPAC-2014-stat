PyCon APAC 2014 Statistics
**************************

Use this data prudently. **Any privacy info MUST NOT be included**.


Python Env Setup
================

Originally on OSX 10.9 homebrewed Python 3.4. Make a clean virtual environment (by either pyvenv or virtualenv is good) before you start.

.. code-block:: bash

    pip install -r requirements.txt
    # This takes a while, since it needs numpy compiled.


Custom IPy Notebook Theme
-------------------------
Ref: <https://github.com/nsonnad/base16-ipython-notebook>

.. code-block:: bash

    # Create a new IPy Notebook profile
    ipython profile create pyconapac

    # Move to that folder
    cd `ipython profile locate pyconapac`/static/custom
    # for fish, change `...` into (...)

    # Link your favored PyCon APAC custom theme.
    # Don't forget to change the filename back to custom.css
    ln -s git_repo/ipynb_profile/custom_solarized_light.css custom.css

    # Start IPy Notebook server and the awesomeness!
    ipython notebook --profile=pyconapac
