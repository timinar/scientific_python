# Materials for Scientific Python Course for astronomers of Moscow University

[![Build Status](https://travis-ci.org/hombit/scientific_python.svg?branch=master)](https://travis-ci.org/hombit/scientific_python)

## How to use this repository

Read files from [`scientific_python`](./scientific_python/) folder in alphabetical order and try to understand how all prints
and asserts work.

## Repository structure

This repository has a structure of <a href="https://packaging.python.org/tutorials/distributing-packages/">a Python package</a> with some additional files:
 - [`scientific_python`](./scientific_python/) folder that represents top level package of the same name. This package contains
   several sub-packages and modules. You can start with [`a_intro`](./scientific_python/a_intro) sub-package and read its 
   modules one by one in alfabetical order. All modules can be used as separate modules and scripts without package
   installation
 - [`bin`](./bin/) folder contains scripts that can be used after package installation. Now they are used for testing
 - [`doc`](./doc/) folder is used for documentation. Now it contains only MS Word file with course annotation (in Russian)
 - [`misc`](./misc/) contains two subfolders related to [`Juyter`](http://jupyter.org) notebooks used in class:
   - [`jupyter_notebooks`](./misc/jupyter_notebooks/) contains notebooks and other files used in class sorted by date
   - [`share_jupyter`](./misc/share_jupyter/) contains little [`Docker`](http://docker.com) project that runs my class `Jupyter`
     server and exposes notebook `HTML` copies to the world on [sai.homb.it](http://sai.homb.it/)
 - [`setup.py`](./setup.py) is used to install this package
 - [`requirements.txt`](./requirements.txt) file contains Python dependicies of the project.
 - [`virtualenv_activation.sh`](./virtualenv_activation.sh) is a sample shell script that can be used to activate
   [`virtualenv`](https://virtualenv.pypa.io/) and install the package. Use it by typing `. virtualenv_activation.sh` or
   `source virtualenv_activation.sh`. For exit virtualenv type `deactivate`
 - [`Dockerfile`](./Dockerfile) and [`docker-compose.yml`](./docker-compose.yml) files can be used to run the project into
   `Docker` container
 - [`.gitignore`](./.gitignore) and [`.gitattributes`](.gitattributes) are [`git`](https://git-scm.com) related files
 - [`.dockerignore`](./.dockerignore) is a link to [`.gitignore`](./.gitignore)
 - [`.travis.yml`](./.travis.yml) is a [`Travis`](https://travis-ci.org) configuration file. `Travis` is a continius 
   integration (CI) system used to test this project with various Python versions: 2.7 and 3.*
