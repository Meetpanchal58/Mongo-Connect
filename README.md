# Usage Guide

## Installation of load_MongoDB Package
You can install the `load_MongoDB` package via pip:

```bash
pip install load_MongoDB
```

## Importing the class
Import the MongoOperation class from mongodb_connect.mongo_crud module:

```python
from mongodb_connect.mongo_crud import MongoOperation
```

## Connecting to Database
Create an instance of MongoOperation class with your database credentials:

```python
client_url = "mongodb+srv://username:password@cluster0.4euesby.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0"
database_name = "Database_name"
collection_name = "Collection_name"
mongo_op = MongoOperation(client_url, database_name, collection_name)
```

## Insert Record
This Unified Insert Function can perform both insert_one() and insert_many() Operations 

```python
data_to_insert_single = {"name": "Alice", "age": 25}
mongo_op.insert(data_to_insert_single)
```

```python
data_to_insert_many = [
    {"name": "Bob", "age": 30},
    {"name": "Charlie", "age": 35}
]
mongo_op.insert(data_to_insert_many)
```

## More CRUD Operations
Similar to insert(), unified functions are provided for each CRUD operation such as Update, Delete, Find. You can find detailed information with examples in the [load_MongoDb Tutorial](https://github.com/Meetpanchal58/Mongo_Connect/blob/main/experiments/Load-MongoDB%20Tutorial.ipynb) in the experiments/load_MongoDB Tutorial directory.

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

