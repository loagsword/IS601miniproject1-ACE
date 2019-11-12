# Python Virtual Environment FAQ

### Is there a way to use the same virtualenv on both Windows and Mac OS?
Answer found in [Stack Overflow.](https://stackoverflow.com/questions/42733542/how-to-use-the-same-python-virtualenv-on-both-windows-and-linux)

There are several reasons why venvs cannot be shared across OSes:
* Some packages contains C extensions, and the OS' .dlls are not compatible with each other.
* venvs contain scripts with hardcoded paths. Windows and Linux paths are different.

The following is a workaround:
1. `pip freeze` all libraries to a `requirements.txt file`.

```
pip freeze > requirements.txt
```

2. Create the venv on each OS:
```
python -m venv env
source env/bin/activate
pip install -r requirements.txt  # Install all the libs.
```

**Note:**
To keep similar venvs in the same folder, another option is to create the venvs with different names.    
For example, you will have the resulting tree structure:
```
Folder/
    - virtualenv/
        - Include
        - Lib
        - Scripts
    - venv/
       - bin
       - include
       - lib
    - pythonscript.py
    - requirements.txt

```



