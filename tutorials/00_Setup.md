---
title: 00. Setup for tutorials
---

We start off by getting setup and connected for the tutorials. Please login to the JupyterHub, which will take a few minutes to load. 

Please go to <https://openscapes.2i2c.cloud/hub/>. Log in with your GitHub Account, and select "Small".

You can also click this badge to launch the Hub: 

[![](https://img.shields.io/static/v1.svg?logo=Jupyter&label=Openscapes&message=AWS+us-west-2&color=orange)](https://openscapes.2i2c.cloud)

While the Hub loads, we'll:

- discuss cloud environments
- see how my Desktop is setup
- Fork the Hackathon repository at github.com
- discuss python and conda environments

Then, when the hub is loaded we'll get oriented and clone the forked repo into our cloud environment.

## Cloud environment

A brief overview about the [NASA Openscapes Cloud Environment](https://nasa-openscapes.github.io/2021-Cloud-Hackathon/clinic/jupyterhub.html) (following lessons from the Clinic).

#### Cloud infrastructure

* Cloud: AWS [`us-west-2`](https://goo.gl/maps/BYqGYxahpwJgzKwR8)
  * Data: AWS S3 (cloud) and [NASA DAAC](https://earthdata.nasa.gov/eosdis/daacs) data centers (on-prem).
  * Cloud compute environment: [2i2c Jupyterhub deployment](https://docs.2i2c.org/en/latest/)
      * IDE: [**JupyterLab**](https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html)

## This is how my desktop is setup

I'll screenshare to show and/or talk through how I have oriented the following software we're using: 

- [2i2c Jupyterhub](https://openscapes.2i2c.cloud/hub/) (our main workspace)
- [Cloud Hackathon Book](https://nasa-openscapes.github.io/2021-Cloud-Hackathon/tutorials/) (my teaching notes, your reference material)
- Zoom Chat
- Slack

## Fork the Hackathon GitHub repository

"How do I get the tutorial repository into the Hub?". There are 2 steps. The first is from GitHub.com to fork the tutorial repository so that there is a connected copy in your user account that you can edit and push changes that won't affect the nasa-openscapes copy.

Go to <https://github.com/nasa-openscapes/2021-Cloud-Hackathon> and fork the repository.

![](../clinic/img/fork-tutorials.png)

## Python and Conda environments

[**Why Python?**](https://foundations.projectpythia.org/foundations/why-python.html)

![Python Data Stack. Source: Jake VanderPlas, “The State of the Stack,” SciPy Keynote (SciPy 2015).](https://pangeo-data.github.io/img/scientific-python-28-638.jpg)

**Default Python Environment:**

We've set up the Python environment with conda. 

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

The project used to create our default environment is called **corn** (as it can include many Python kernels).

If we want to update a library or install a whole new environment we need to open an issue on this repository. We can help your teams do this during project hacktime. 

### [corn 🌽](https://github.com/NASA-Openscapes/corn)

## JupyterHub orientation

Now that the JupyterHubs have loaded, let's get oriented.

### First impressions

Reiterate a few things we just talked about (TODO - what's useful here Luis?)

- "home directory"
- big blue button
- environments we just talked about (?)

### Terminal

Open terminal: Big blue "+" button > Terminal

You'll start off in your home directory, `/home/jovyan`. To confirm this is your present working directory (pwd), type: 

```.{bash}
pwd
```


## Clone the Hackathon GitHub repository

Now we'll clone the GitHub repository, using the terminal. 

```{.bash}
git clone https://github.com/YOUR-USERNAME/2021-Cloud-Hackathon
```

These two github steps are also posted in [github workflows: first-time setup](https://nasa-openscapes.github.io/2021-Cloud-Hackathon/logistics/github-workflows.html).

## Jupyter notebooks

Let's get oriented to Jupyter notebooks, which we'll use in all the tutorials. 

Big blue button > Notebook > ...


## How to I end my session?
*(Also see [How do I end my Openscapes session? Will I lose all of my work?](https://nasa-openscapes.github.io/2021-Cloud-Hackathon/clinic/jupyterhub.html#how-do-i-end-my-openscapes-session))*

When you are finished working for the day it is important to explicitly log out of your Openscapes session. The reason for this is it will save us a bit of money! When you keep a session active it uses up AWS resources and keeps a series of virtual machines deployed.

Stopping the server happens automatically when you log out, so navigate to “File -> Log Out” and just click “Log Out”!

!!! NOTE “logging out” - Logging out will **NOT** cause any of your work to be lost or deleted. It simply shuts down some resources. It would be equivalent to turning off your desktop computer at the end of the day.
