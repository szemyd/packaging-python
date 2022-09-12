# python-packaging
📦 This is a template repo on how to package a python project to be distributable.

It is the copied version of https://packaging.python.org/en/latest/tutorials/packaging-projects/


# Building:

**Build the package by the following steps**
1. Optional: Activate new/existing conda environment
2. Install build: ``python3 -m pip install --upgrade build``
3. Build module: ``python3 -m build``

# Distribution

## Locally
- Run ``python3 -m pip install -e "path/to/file"`` 
    eg.: if your project is next to the module you'd like to install in one directory: ``python3 -m pip install -e "../package-name"``

## Online, to PyPi/TesPyPi
1. Install twine ``python3 -m pip install --upgrade twine``
2. Upload to testpypi ``python3 -m twine upload --repository testpypi dist/*``

# Installation
- ``python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps example-package-YOUR-USERNAME-HERE``