# e-commerce-website
*.pyc
# Byte-compiled / optimized / DLL files
__pycache__/
media_root
*.py[cod]
*$py.class

# C extensions
*.so

# Distribution / packaging
.Python
build/
develop-eggs/
dist/
downloads/
eggs/
.eggs/
lib/
lib64/
parts/
sdist/
var/
wheels/
share/python-wheels/
*.egg-info/
.installed.cfg
*.egg
MANIFEST

# PyInstaller
#  Usually these files are written by a python script from a template
#  before PyInstaller builds the exe, so as to inject date/other infos into it.
*.manifest
*.spec

# Installer logs
pip-log.txt
pip-delete-this-directory.txt

# Unit test / coverage reports
htmlcov/
.tox/
.nox/
.coverage
.coverage.*
.cache
nosetests.xml
coverage.xml
*.cover
*.py,cover
.hypothesis/
.pytest_cache/
cover/

# Translations
*.mo
*.pot

# Django stuff:
*.log
local_settings.py
db.sqlite3
db.sqlite3-journal

# Flask stuff:
instance/
.webassets-cache

# Scrapy stuff:
.scrapy

# Sphinx documentation
docs/_build/

# PyBuilder
.pybuilder/
target/

# Jupyter Notebook
.ipynb_checkpoints

# IPython
profile_default/
ipython_config.py

# pyenv
#   For a library or package, you might want to ignore these files since the code is
#   intended to run in multiple environments; otherwise, check them in:
# .python-version

# pipenv
#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
#   However, in case of collaboration, if having platform-specific dependencies or dependencies
#   having no cross-platform support, pipenv may install dependencies that don't work, or not
#   install all needed dependencies.
#Pipfile.lock

# PEP 582; used by e.g. github.com/David-OConnor/pyflow
__pypackages__/

# Celery stuff
celerybeat-schedule
celerybeat.pid

# SageMath parsed files
*.sage.py

# Environments
.env
.venv
env/
venv/
ENV/
env.bak/
venv.bak/

# Spyder project settings
.spyderproject
.spyproject

# Rope project settings
.ropeproject

# mkdocs documentation
/site

# mypy
.mypy_cache/
.dmypy.json
dmypy.json

# Pyre type checker
.pyre/

# pytype static type analyzer
.pytype/

# Cython debug symbols
cython_debug/

static_root
env 
media_root 
 6  .vscode/settings.json 
@@ -1,13 +1,13 @@
{
  "python.pythonPath": "${workspaceFolder}/env/bin/python3",
  "editor.formatOnSave": true,
  "python.linting.pep8Enabled": true,
  "python.linting.pycodestyleEnabled": true,
  "python.linting.pylintPath": "pylint",
  "python.linting.pylintArgs": ["--load-plugins", "pylint_django"],
  "python.linting.pylintEnabled": true,
  "python.venvPath": "${workspaceFolder}/env/bin/python3",
  "python.linting.pep8Args": ["--ignore=E501"],
  "python.linting.pycodestyleArgs": ["--ignore=E501"],
  "files.exclude": {
    "**/*.pyc": true
  }
}
} 
 1  FUNDING.yml 
@@ -0,0 +1 @@
github: [mattfreire] 
 78  README.md 
@@ -1,9 +1,77 @@
# Django Ecommerce
# Django E-commerce

This is an ecommerce website built with Django. The website displays products. Users can add and remove products to/from their cart while also specifying the quantity of each item.
This is a very simple e-commerce website built with Django.

[![alt text](https://github.com/justdjango/django-ecommerce/blob/master/thumbnail.png "Logo")](https://youtu.be/z4USlooVXG0)
## Quick demo

[Watch the tutorial series here](https://youtu.be/z4USlooVXG0)
[![alt text](https://justdjango.s3-us-west-2.amazonaws.com/media/gifs/djecommerce.gif "Logo")](https://youtu.be/z4USlooVXG0)

[Become a better Django developer](https://www.justdjango.com)
---

## Deprecation warning

This project was created over two years ago. Since then, there is a newer version of the project which you can find [here](https://github.com/justdjango/django-simple-ecommerce)

---

## Project Summary

The website displays products. Users can add and remove products to/from their cart while also specifying the quantity of each item. They can then enter their address and choose Stripe to handle the payment processing.

[![alt text](https://justdjango.s3-us-west-2.amazonaws.com/media/thumbnails/djecommerce.png "Logo")](https://youtu.be/z4USlooVXG0)

---

## Running this project

To get this project up and running you should start by having Python installed on your computer. It's advised you create a virtual environment to store your projects dependencies separately. You can install virtualenv with

```
pip install virtualenv
```

Clone or download this repository and open it in your editor of choice. In a terminal (mac/linux) or windows terminal, run the following command in the base directory of this project

```
virtualenv env
```

That will create a new folder `env` in your project directory. Next activate it with this command on mac/linux:

```
source env/bin/active
```

Then install the project dependencies with

```
pip install -r requirements.txt
```

Now you can run the project with this command

```
python manage.py runserver
