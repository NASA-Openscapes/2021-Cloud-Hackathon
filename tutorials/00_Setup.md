---
title: 00. Setup for tutorials
---

::: {.callout-tip collapse="true"}
## Text to paste into Zoom Chat

Please go to https://openscapes.2i2c.cloud/hub/ - log in with your GitHub Account, and select "Small"
:::


## GitHub setup for tutorials

This will get you set up and answer the question "How do I get the tutorial repository into the Hub?""

* [Git setup](../clinic/notebooks.html): The first time we access our cloud environment we'll be asked to login with out Github account, this section will guide us to setup a Github account and setup our credentials in the Openscapes hub.

* [Git flow](../logistics/github-workflows.html): When we work in a collaborative environment we usually run into conflicts while updating the same resources, this section will guid us on the basic git operations we'll use during the hack week.


## Cloud Environment

A brief overview about the [NASA Openscapes Cloud Environment](https://nasa-openscapes.github.io/2021-Cloud-Hackathon/clinic/jupyterhub.html) (following lessons from the Clinic).

#### Cloud infrastructure

* Cloud: AWS [`us-west-2`](https://goo.gl/maps/BYqGYxahpwJgzKwR8)
  * Data: AWS S3 (cloud) and [NASA DAAC](https://earthdata.nasa.gov/eosdis/daacs) data centers (on-prem).
  * Cloud compute environment: [2i2c Jupyterhub deployment](https://docs.2i2c.org/en/latest/)
      * IDE: [**JupyterLab**](https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html)

## This is how my desktop is setup

[![Openscapes Hub](https://img.shields.io/static/v1.svg?logo=Jupyter&label=Openscapes&message=AWS+us-west-2&color=orange)](https://openscapes.2i2c.cloud)


#### Python and Conda environments

[**Why Python?**](https://foundations.projectpythia.org/foundations/why-python.html)

![Caption: The Python Data Stack. Source: Jake VanderPlas, “The State of the Stack,” SciPy Keynote (SciPy 2015).](https://pangeo-data.github.io/img/scientific-python-28-638.jpg)

Default Python Environment:

::: {.callout-note collapse="true"}

### Conda environment

```yaml
name: openscapes
channels:
  - conda-forge
dependencies:
  - python=3.9
  - pangeo-notebook
  - awscli~=1.20
  - boto3~=1.19
  - gdal~=3.3
  - rioxarray~=0.8
  - xarray~=0.19
  - h5netcdf~=0.11
  - netcdf4~=1.5
  - h5py~=2.10
  - geoviews~=1.9
  - matplotlib-base~=3.4
  - hvplot~=0.7
  - pyproj~=3.2
  - bqplot~=0.12
  - geopandas~=0.10
  - zarr~=2.10
  - cartopy~=0.20
  - shapely==1.7.1
  - pyresample~=1.22
  - joblib~=1.1
  - pystac-client~=0.3
  - s3fs~=2021.7
  - ipyleaflet~=0.14
  - sidecar~=0.5
  - jupyterlab-geojson~=3.1
  - jupyterlab-git
  - jupyter-resource-usage
  - ipympl~=0.6
  - conda-lock~=0.12
  - pooch~=1.5
  - pip
  - pip:
    - tqdm
    - harmony-py
    - earthdata
    - zarr-eosdis-store
```
:::


### Bash terminal and installed software
Libraries that are available from the terminal

* gdal 3.3 commands ( gdalinfo, gdaltransform...)
* hdf5 commands ( h5dump, h5ls..)
* netcdf4 commands (ncdump, ncinfo ...)
* jq (parsing json files or streams from curl)
* curl (fetch resources from the web)
* awscli (AWS API client, to interact with AWS cloud services)
* vim (editor)
* tree ( directory tree)
* more ...

### Updating the environment

Scientific Python is a vast space and we only included libraries that are needed in our tutorials.
Our default environment can be updated to include any Python library that's available on pip or conda.

The project used to create our default environment is called **corn** (as it can include many Python kernels)

If we want to update a library or install a whole new environment we need to open an issue on this repository

### [corn 🌽](https://github.com/NASA-Openscapes/corn)

## Open a tutorial template notebook

Navigate to `tutorials-template` folder. Our first tutorial is `Data_discovery_with_cmr.ipynb`


## How to I end my session?
*(Also see [How do I end my Openscapes session? Will I lose all of my work?](https://nasa-openscapes.github.io/2021-Cloud-Hackathon/clinic/jupyterhub.html#how-do-i-end-my-openscapes-session-will-i-lose-all-of-my-work))*

When you are finished working for the day it is important to explicitly log out of your Openscapes session. The reason for this is it will save us a bit of money! When you keep a session active it uses up AWS resources and keeps a series of virtual machines deployed.

Stopping the server happens automatically when you log out, so navigate to “File -> Log Out” and just click “Log Out”!

!!! NOTE “logging out” - Logging out will **NOT** cause any of your work to be lost or deleted. It simply shuts down some resources. It would be equivalent to turning off your desktop computer at the end of the day.
