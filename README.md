## Testing Python Virtual Enviornments

Following the guide https://serpapi.com/blog/python-virtual-environments-using-virtualenv-and-poetry/

1. Install via brew: ``pip install virtualenv``
2. Create an enviornment named "env" by: ``python -m venv env ``
3. This creates a sub folder named "env", activate the enviorment by
    1. Macos, Linux:    ``source env/bin/activatei``
    2. Windows:         ``source env/Scripts/activatei``
4. Now you can install via pip into this enviornment normally: pip install numpy
5. While your are in the _activated_ state with the (env) label, you can run python code using the local python install as ``python code.py`` etc.
6. When your are done, leave the environemnt with ``deactivate``
