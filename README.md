
## Cloud Hackathon: Transitioning Earthdata Workflows to the Cloud

&lt;any header images?>


### Welcome

Welcome to **Cloud Hackathon: Transitioning Earthdata Workflows to the Cloud,** co-hosted by the NASA EOSDIS Physical Oceanography Distributed Active Archive Center ([PO.DAAC](https://podaac.jpl.nasa.gov/)), National Snow and Ice Data Center DAAC ([NSIDC DAAC](https://nsidc.org/daac)), Land Processes Distributed Active Archive Center ([LP.DAAC](https://lpdaac.usgs.gov/)), with support provided by [ASDC DAAC](https://earthdata.nasa.gov/eosdis/daacs/asdc), [GES DISC](https://disc.gsfc.nasa.gov/) and [NASA Openscapes](https://nasa-openscapes.github.io/) Project.

The Cloud Hackathon will take place **virtually** from **November 15-19, 2021.** The event is free to attend, but an application is required. If you are interested in participating, the application period is open September 20 - October 8, 2021.



### About 

The **Cloud Hackathon: Transitioning Earthdata Workflows to the Cloud** is a virtual 5-day (4 hours per day) collaborative learning experience aimed at exploring, creating, and promoting effective cloud-based science and applications workflows using NASA Earthdata Cloud data, tools, and services (among others), in support of Earth science data processing and analysis in the era of big data. Its goals are to:



1. **Introduce** Earth science data users to NASA Earthdata cloud-based data products, tools and services in order to increase awareness and support transition to cloud-based science and applications workflows.
2. **Enable** science and applications workflows in the cloud that leverage NASA Earth Observations and capabilities (services) from within the NASA Earthdata Cloud, hosted in Amazon Web Services (AWS) cloud, thus increasing NASA Earthdata data utility and meaningfulness for science and applications use cases.
3. **Foster community engagement** utilizing Earthdata cloud tools and services in support of open science and open data.

**Outcome**: Participants prototype their science and applications workflows (via hackweek projects) that leverage Earthdata Cloud data and services (focusing on, but not limited to, oceanography, cryosphere, hydrology and land data), which supports them in their transition to cloud-based or hybrid workflows for data processing and analysis.

This is an opportunity for researchers that might not yet have had the opportunity to work in the Cloud to explore, learn and prototype workflows with NASA Earthdata in the Cloud, but more intermediate or advanced cloud users interested in further exploring cloud workflows with Earthdata Cloud data and service are also welcome. 


### Application

#### Information for applicants

The Cloud Hackathon will be a virtual event held November 15-19, 2021, where participants will explore the intersection of Earth science data, cloud computing, and big data analysis through demonstration tutorials and hands-on “hacking” projects. To best benefit from the event, we recommend some familiarity or experience with: 

* NASA Earthdata data (focusing on oceanography, cryosphere, hydrology and land data, including interdisciplinary applications); and 
* Programming skills using Python. “We plan to accept participants with diverse skill levels and backgrounds in programming. However, to best benefit from and contribute to the program, participants are expected to have some experience with Python programming.”

No cloud computing experience is required, but we encourage both beginner and more experienced participants with AWS cloud to apply.

If selected, participants will have the option to attend a Carpentries-style github, python, shell scripting clinic ahead of the Cloud Hachathon.


### Application form

In the <span style="text-decoration:underline;">application form</span>, we encourage you to think about and provide a science use case that you would like to prototype in the cloud. At the beginning of the hackweek, selected participants will be able to pitch their use case to support the formation of “hack” projects. During the hackweek, participants will get into teams of their choosing, around a common use case to “hack” in the cloud. The use cases provided in the application form will also help the organizers best prepare materials tailored to those use cases.

The Cloud Hackathon will be a virtual event held November 15-19, 2021. Participants will explore the intersection of Earth science data, cloud computing, and big data analysis through demonstration tutorials and hands-on “hacking” projects. We will form groups to experiment (“hack”) together and it is possible to do this with your own team if you indicate other team members are also applying (e.g. your research group). Both individuals and individuals as part of research groups are welcome to apply (see Application Form).

To best benefit from the event, we recommend some familiarity or experience with: 

* NASA Earthdata data (focusing on oceanography, hydrology and land data, including interdisciplinary applications)
* Programming skills using Python. 

No cloud computing experience is required, but we encourage both beginner and more experienced participants with AWS and Earthdata Cloud to apply. We will accept participants with diverse skill levels and backgrounds in programming. However, to best benefit from and contribute to the program, participants are expected to have some experience with Python programming.

If selected, participants will have the option to attend a Carpentries-style github, python, shell scripting clinic ahead of the Cloud Hackathon.


#### Application Form

In the [application form](https://forms.gle/JJNKZ6pGKxWVFzLr6), we encourage you to think about and provide a science use case that you would like to prototype in the cloud. At the beginning of the hackweek, participants will be able to pitch their use case to support the formation of “hack” projects - by which we mean collaboratively experiment working in with NASA Earthdata data and capabilities in the Cloud. During the hackweek, participants will get into teams of their choosing, around a common use case to “hack” in the cloud. The use cases provided in the application form will also help the organizers best prepare materials tailored to those use cases.

**To apply, please fill out this [application form](https://forms.gle/JJNKZ6pGKxWVFzLr6).**


### What to expect

* During the Cloud Hackathon, the selected participants will have access to cloud environments in AWS through a JupyterHub interface, provided through 2i2c. 
* Participants will be guided on how to log into the cloud environment, import needed data recipes and resources, and will have the opportunity to explore and develop science and applications workflows in a cloud environment (hosted in AWS) using example tutorials as building blocks. 
* Throughout the hackathon, participants will learn about NASA’s Earthdata move to the cloud and Earthdata APIs for data discovery, access, and transformations to enable faster, more efficient time to science. 

In the two to three weeks leading up to the hackathon, participants are encouraged to review **background resources** that will facilitate a more effective hackweek experience. These resources will be shared here leading up to the Hackathon dates, and will be accessible to all data users, whether they attend the hackathon or not.

**The following datasets are currently available from the NASA Earthdata Cloud.** Participants can choose to prototype a cloud-based science workflow using a combination of these datasets, as well as other non-Earthdata Cloud data. If your preferred dataset is not yet available in the Earthdata Cloud, consider using a current cloud-based dataset as proxy to explore prototyping.


* [https://search.earthdata.nasa.gov/portal/podaac-cloud/search](https://search.earthdata.nasa.gov/portal/podaac-cloud/search) (PO.DAAC)

**Example** **use** **cases** to explore in the cloud (note these are for inspiration only, you are not limited to these workflows):



* Use the advanced wildcard search capabilities in Earthdata Search Client/Common Metadata Repository (CMR) to precisely search/select all Sentinel-6A granules...
    * from a specific cycle (i.e. a sequence orbits that together provide global spatial coverage), and/or 
    * from a specific pass(es) over multiple cycles (i.e. selected orbits over a series of cycles that together provide a time series coverage).
    * Then, prepare the data for gridding or for local analysis at space/time scales which are appropriate for the target analysis (and limited by default given the length of S6A data record...)
* Co-locate satellite and in-situ for comparison, after spatially and temporally selecting the data of interest. E.g. Compare MODIS SST Level 2, MUR SST Level 4, and Argo measurements over a coastal region of interest, without having to download any of the data to your local machine.


This event is motivated by the dawn of the era of Big Data. NASA’s Earth Observing System Data and Information System (EOSDIS) is in the process of moving EOSDIS data to the cloud, driven by a rapid rate of data ingest into the EOSDIS archive. NASA remote sensing data from both upcoming (e.g. SWOT) and existing (e.g. Terra, Aqua, ICESat-2) missions will be available in the Earthdata Cloud platform in the coming years. The paradigm shift from on-premise (local) to cloud-based data distribution, and that from “download and analyze” to “analysis in place” present opportunities and challenges. Guiding users through this transition is of the utmost importance.

**If interested in participating in this event, please submit an [Application](https://forms.gle/JJNKZ6pGKxWVFzLr6).**


Cloud Hackathon: Transitioning Earthdata Workflows to the Cloud is co-hosted by PO.DAAC (logo), NSIDC/DAAC (logo), LP.DAAC (logo), with support from ASDC DAAC (logo), GES DISC (logo) and NASA Openscapes (logo), and cloud computing infrastructure by 2i2c (logo)?

