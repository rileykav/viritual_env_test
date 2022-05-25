## Testing Python Virtual Enviornments

Following the guide https://serpapi.com/blog/python-virtual-environments-using-virtualenv-and-poetry/

The initial set up:
1. Install via brew: ``pip install virtualenv``
2. Create an enviornment named "env" by: ``python -m venv env ``
3. This creates a sub folder named "env", now activate/enter the enviorment by
    1. Macos, Linux:    ``source env/bin/activate``
    2. Windows:         ``source env/Scripts/activate``
4. Now you can install via pip into this enviornment normally: pip install numpy
5. While your are in the _activated_ state with the (env) label, you can run python code using the local python install as ``python code.py`` etc.
6. When your are done, leave the environemnt with ``deactivate``

To share this enviornment with someone
1. First enter the enviornment again, and run ``pip freeze > requirments.txt``.
2. Now share your project (excluding the env/ folder, git normally ignores it, but add it to .gitignroe file otherwise) and this requirments.txt file.
3. In the second location start a new enviornment as above, and now install packages from the requirments list via ``pip install -r requirments.txt`` (inside the enviornment obviously).

Some Quirks
1. This does require the other party to have python, pip, virtualenv installed, so is not the best way to share a project that you want to just run, but its suitable for my purposes right now.
2. All python code executions do have to be done inside the enviornment,
