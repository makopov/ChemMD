ChemMD
======

*ChemMD is a wrapper for interpreting data and metadata `.json` files
for analysis and visualization.*

**To do:**

+ [ ] Complete `ChemMD` repository setup.
    + [ ] Apply new structure to Bokeh applications.
+ [ ] Complete query group setup.
    *These should be Drupal content types that the user selects.*
+ [ ] Complete tests setup for `ChemMD`.
+ [ ] Travis CI integration.
+ [ ] DockerHub integration.
+ [ ] Better code integration.
+ [ ] Sphinx documentation setup.
+ [ ] Add a license.
+ [ ] `io.py` see contained todo items.

Folder Descriptions
-------------------

*See the README files in each directory for a more detailed
description.*

+ `bokeh_apps` [Bokeh](https://github.com/bokeh/bokeh) web
    applications which display data / metadata sets provided
    by `ChemMD`.
+ `chemmd` The Python package which provides the data
    for the `bokeh` applications in `bokeh_apps`.
+ `scripts` Scripts used for deploying applications within
    `bokeh_apps`.
+ `tests` Tests for the contained programs.

File Descriptions
-----------------

*Files in this top-level directory.*

+ `.gitignore` Files and folders to be ignored by Git.
+ `Dockerfile` A file which defines the Docker image with
   ChemMD and associated visualizations. The image launches
   a Bokeh server by default. 
+ `LICENSE.txt` 
+ `README.md` This readme file.
+ `requirements.txt` A list of Python packages needed for
   ChemMD to function.
+ `setup.py` The installation script for the ChemMD package.


Installation Instructions
-------------------------

**Basic Installation:**

```bash
# Clone the repository.
git clone git@github.com:biggstd/ChemMD.git
# Change to the parent directory and run the installer with pip.
cd ChemMD
pip install .
```

**Run in Docker:**

*To build the image locally:*

```bash
 docker build -t ChemMD .
```

*To run the container from Docker Hub:*

```bash
#TODO: Implement me.
```

*Open a bash shell within the container:*

```bash
docker exec -it ChemMD bash
```

*Stop and delete the container:*

```bash
docker stop ChemMD && docker rm ChemMD
```
