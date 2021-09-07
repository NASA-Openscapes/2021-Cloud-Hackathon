
## Cloud Hackathon: Transitioning Earthdata Workflows to the Cloud

&lt;any header images?>


### Welcome

Welcome to **Cloud Hackathon: Transitioning Earthdata Workflows to the Cloud,** co-hosted by the NASA EOSDIS Physical Oceanography Distributed Active Archive Center ([PO.DAAC](https://podaac.jpl.nasa.gov/)), National Snow and Ice Data Center DAAC ([NSIDC DAAC](https://nsidc.org/daac)), Land Processes Distributed Active Archive Center ([LP.DAAC](https://lpdaac.usgs.gov/)), with support provided by [ASDC DAAC](https://earthdata.nasa.gov/eosdis/daacs/asdc), [GES DISC](https://disc.gsfc.nasa.gov/) and [NASA Openscapes](https://nasa-openscapes.github.io/).

The Cloud Hackathon will be taking place **virtually** from **November 15-19, 2021.** The event is free to attend. If you are interested in participating, the application period is open September 15 - October 13, 2021.


### About 

The **Cloud Hackathon: Transitioning Earthdata Workflows to the Cloud **is a virtual 5-day (4 hours per day) collaborative learning experience aimed at exploring, creating, and promoting effective cloud-based science and applications workflows using NASA Earthdata Cloud data, tools, and services (among others), in support of Earth science data processing and analysis in the era of big data. Its goals are to:



1. **Introduce** Earth science data users to NASA Earthdata cloud-based data products and tools and services in order to increase awareness and support transition to cloud-based science and applications workflows.
2. **Enable** science and applications workflows in the cloud that leverage NASA Earth Observations from the NASA Earthdata Cloud, hosted in Amazon Web Services (AWS) cloud, thus increasing NASA Earthdata data utility and meaningfulness for science and applications use cases.
3. **Foster/enable community engagement** utilizing Earthdata cloud tools and services in support of open science and open data.

**Outcome**: Participants prototype their science and applications workflows (via hackweek projects) that leverage Earthdata Cloud data and services (focusing on, but not limited to, oceanography, cryosphere, hydrology and land data), which supports them in their transition to cloud-based or hybrid workflows for data processing and analysis.


#### Information for applicants

The Cloud Hackathon will be a virtual event held November 15-19, 2021, where participants will explore the intersection of Earth science data, cloud computing, and big data analysis through demonstration tutorials and hands-on “hacking” projects. To best benefit from the event, we recommend some familiarity or experience with: 



* NASA Earthdata data (focusing on oceanography, cryosphere, hydrology and land data, including interdisciplinary applications); and 
* Programming skills using Python. “We plan to accept participants with diverse skill levels and backgrounds in programming. However, to best benefit from and contribute to the program, participants are expected to have some experience with Python programming.”

No cloud computing experience is required, but we encourage both beginner and more experienced participants with AWS cloud to apply.

If selected, participants will have the option to attend a Carpentries-style github, python, shell scripting clinic ahead of the Cloud Hachathon.


### Application form

In the <span style="text-decoration:underline;">application form</span>, we encourage you to think about and provide a science use case that you would like to prototype in the cloud. At the beginning of the hackweek, selected participants will be able to pitch their use case to support the formation of “hack” projects. During the hackweek, participants will get into teams of their choosing, around a common use case to “hack” in the cloud. The use cases provided in the application form will also help the organizers best prepare materials tailored to those use cases.


### What to expect



* During the Cloud Hackathon, the selected participants will have access to cloud environments in AWS through the JupyterHub interface. 
* Participants will be guided on how to log into the cloud environment, import needed data recipes and resources, and will have the opportunity to explore and develop science and applications workflows in a cloud environment (hosted in AWS) using example tutorials as building blocks. 
* Throughout the hackathon, participants will learn about NASA’s Earthdata move to the cloud and Earthdata APIs for data discovery, access, and transformations to enable faster, more efficient time to science. 

Two-three weeks leading up to the hackathon, selected participants are encouraged to review **background resources** that will facilitate a more effective hackweek experience. These resources will be shared here leading up to the Hackathon dates, and will be accessible to all users, whether they attend the hackathon or not.

**The following datasets are currently available from the NASA Earthdata Cloud.** Participants can choose to prototype a cloud-based science workflow using a combination of these datasets, as well as other non-Earthdata Cloud data. 

&lt;Insert cloud datasets>

**Example** **use** **cases** to explore in the cloud (note these are for inspiration only, you are not limited to these workflows):



* Ex 1
* Ex 2
* Ex 3


### Pre-requisites

Participants should have the following set up ahead of the event:



* An Earthdata Login account
* A slack account
* A github account (for access to 2i2c AWS JupyterHub)
* Reviewed [Intro to JupyterHub](https://snowex-hackweek.github.io/website/preliminary/jupyterhub.html) if not familiar 
* Optional: python setup


### Hackathon Schedule

**Day 1 **(4 hours)**:** **_Welcome, interactive lectures, introduction of Earthdata tools & datasets _**



* **Introductions, logistics **
    * Welcome, motivation for hackathon/goals 
    * Overview of hackweek agenda
    * ‘Tools’ we’ll be using during hackathon
    * Code of conduct
    * Introduction of the instructors
    * Introduction to projects - how the hackathon is set up
* **Break** 
* **Icebreaker** 
* **Getting set up and connected - Github, JupyterHub**
    * Connecting to our shared (Openscapes 2i2c AWS) JupyterHub environment
    * Learn how to clone the cloud hackathon tutorials into your working environment
    * Check everyone has a working Earthdata Login
* **Break**
* **Introduction to Earthdata Cloud, data, tools**
    * What is Earthdata Cloud? And what does it mean to the user? 
    * Reminder of _current_ existing datasets in the Eathdata Cloud
    * Introduction to Earthdata tools and services - GUI, API
* **Break** 
* **Projects: Introduction and Pitching**
    * pitching of project ideas
    * breakout groups to learn more about which team to join
* **Project team breakout**
    * Form teams (of 3-4 per team) 
    * Identify team lead 
    * Define problem statement for team project (working off of the ideas pitched earlier) 

**Day 2 **(4 hours) -**_ Data Discovery and NASA Earthdata APIs_**



* **Demos**  
    * Demo 2.1: search programmatically using CMR API
    * Q&A 
    * Demo 2.2: search programmatically using CMR-STAC API
    * Q&A 
* **Break** 
* **Demos **
    * Demo 2.3: EDL/authentication/S3credentials 
    * Q&A
    * Demo 2.4: in-cloud big data analysis example 
* **Team hack time** (2 hours)
* Virtual Happy Hour - optional 

**Day 3 **(4 hours) - **_In-Cloud Access_**



* **Demos  **
    * Demo 4.1: direct S3 access
    * Q&A 
    * Demo 4.2: access COF data via Harmony netCDF-to-Zarr 
    * Q&A 
* Break
* **Demos** 
    * Demo 4.3: access COF data via Zarr EOSDIS Store
    * Q&A 
    * Demo 4.4: search and direct access
* **Team hack time **(2 hours)

**Day 4 **(4 hours) - **_Transformations and data match-up_**



* **Demos **
    * Demo 3.1: subset with Opendap in the cloud (hyrax)
    * Q&A
    * Demo 3.2: subset L2 data with Harmony L2SS-py (spatial, variable) 
    * Q&A 
* Break
* **Demos**
    * Demo 3.3: search, co-locate with in-situ, subset workflow
    * Q&A
* **Team hack time **(2 hours)

**Day 5 **(2.5-3.5 hours) 



* **Project Team time / Office hours**
* **Teams Report-Out** (10 min each x ~10 teams of 4)
    * _What was the use case? What capabilities, tools and datasets did you use? What questions do you still have? _
    * **Part 1: Teams 1-5 **
    * Break
    * **Post-hackathon survey**
    * **Part 2: Teams 6-10** 
* **Close-out remarks** and any remaining **Q&A**
