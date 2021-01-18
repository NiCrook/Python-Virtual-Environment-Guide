# Python virtual environments in Windows
[medium python logo]

## What the guide is about
This is a simple guide about python virtual environments, from what they are to maintaining them.

## What is virtual environment (venv) is
A venv is a self-cointained directory tree for Python and additional packages.

## Why venvs are necessary
Venvs are necessary to prevent conflicts between different versions of the same module being required for different applications.

## What's needed to make a venv
What is needed to make a virtual environment in Python is python, pip, and virtualenv

https://www.python.org/ [small python logo

pip is a package manager for Python.
```py -m pip --version```

installing virtualenv:
```python3 -m pip install --user virtualenv```

## How to make a venv
```python3 -m venv /new/venv/dir```

Note: any parent directory that doesn't exist will be created.

Note: if the target directory exists, an error will be raised unless ```--clear``` is used.

## How to interact/maintain a venv
Activate the virtual environment from the CLI from the target directory ```Scripts\activate```
If successful, you should see to the left of your current directory the directory name in parentheses.

(testvenv) C:\path\to\testvenv

To deactivate, simply type in the CLI: deactivate.

Add modules with ```pip install module```, where module is your desired module.

To remove modules, user ```pip install module```.

## Resources
1. https://docs.python.org/3/tutorial/venv.html
2. https://www.python.org/dev/peps/pep-0405/
3. https://virtualenv.pypa.io/en/latest/
