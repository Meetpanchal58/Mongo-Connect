# Usage Guide

## Installation of load_MongoDB Package
You can install the `load_MongoDB` package via pip:

![Screenshot 2024-03-05 150547](https://github.com/Meetpanchal58/Mongo-Connect/assets/63542891/75dc95df-0bad-464c-8c4e-cb37e7e4abc5)

## Importing the class
Import the MongoOperation class from mongodb_connect.mongo_crud module:

![Screenshot 2024-03-05 150612](https://github.com/Meetpanchal58/Mongo-Connect/assets/63542891/68bcff65-f767-4ced-ae24-00fdcb3f22fa)

## Connecting to Database
Create an instance of MongoOperation class with your database credentials:

![Screenshot 2024-03-05 150647](https://github.com/Meetpanchal58/Mongo-Connect/assets/63542891/60c48470-5267-43a1-b373-7b0404d5c1fa)


## CRUD Operations
All of the CRUD operation such as Insert, Update, Delete & Find. You can find detailed information with examples in the [load_MongoDB Tutorial](https://github.com/Meetpanchal58/Mongo_Connect/blob/main/experiments/Load-MongoDB%20Tutorial.ipynb) in the experiments/load_MongoDB Tutorial directory.

---

## Usage of All files

### requirements_dev.txt for testing
It simplifies the installation and management of dependencies for development and testing, separate from the dependencies required for production.

### Difference between requirements_dev.txt and requirements.txt

`requirements.txt` specifies dependencies required to run the production code of a Python project, while `requirements_dev.txt` specifies dependencies required for development and testing purposes.

### tox.ini
It's used for testing the Python package against different versions of Python.

### How tox works: tox environment creation
1. Install dependencies and packages 
2. Run commands
3. It's a combination of virtualenvwrapper and makefile
4. It creates a .tox directory

### pyproject.toml
It's used for configuring the Python project. It's an alternative to the setup.cfg file. It contains configuration related to the build system such as the build tool used, package name, version, author, license, and dependencies.

### setup.cfg
In summary, setup.cfg is used by setuptools to configure the packaging and installation of a Python project.

### Testing python application
**Types of testing**
1. Automated testing 
2. Manual testing

**Mode of testing**
1. Unit testing
2. Integration tests

**Testing frameworks**
1. pytest
2. unittest
3. robotframework
4. selenium
5. behave
6. doctest

**Check with the code style formatting and syntax (coding standard)**
1. pylint
2. flake8 (it is best because it contains 3 libraries: pylint, pycodestyle, mccabe)
3. pycodestyle

