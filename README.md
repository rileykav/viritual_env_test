// Testing Python Virtual Enviornments

Following the guide https://serpapi.com/blog/python-virtual-environments-using-virtualenv-and-poetry/

1. Install via brew: pip install virtualenv
2. Create an enviornment named "env" by: python -m venv env 
3. This creates a sub folder named "env", activate the enviorment by
    a. Macos, Linux:    source env/bin/activate
    b. Windows:         source env/Scripts/activate
4. Now you can install via pip into this enviornment: pip install numpy
