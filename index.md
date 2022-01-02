---
title: "2021 Cloud Hackathon"
subtitle: "Transitioning Earthdata Workflows to the Cloud"
 
author: "This Hackathon is co-hosted by PODAAC, NSIDC DAAC, and LPDAAC. Additional support is provided by ASDC, GESDISC, IMPACT, and Openscapes."
---

## Welcome

![](https://user-images.githubusercontent.com/2915555/133526401-b79abf6c-ab0d-438d-9927-da39b7c17b96.jpg)


Welcome to **Cloud Hackathon: Transitioning Earthdata Workflows to the Cloud,** co-hosted by the NASA EOSDIS Physical Oceanography Distributed Active Archive Center ([PO.DAAC](https://podaac.jpl.nasa.gov/)), National Snow and Ice Data Center DAAC ([NSIDC DAAC](https://nsidc.org/daac)), Land Processes Distributed Active Archive Center ([LP.DAAC](https://lpdaac.usgs.gov/)), with support provided by [ASDC DAAC](https://asdc.larc.nasa.gov/), [GES DISC](https://disc.gsfc.nasa.gov/), [IMPACT](https://impact.earthdata.nasa.gov/), and [NASA Openscapes](https://nasa-openscapes.github.io/).

The Cloud Hackathon will take place **virtually** from **November 15-19, 2021.** The event is free to attend, but an application is required. The application period (September 21 - October 12, 2021) is now closed. Those who applied will be informed of the outcome on or around October 20th, 2021.

**Post-workshop resources.** Learn about the [2021 Projects](https://nasa-openscapes.github.io/2021-Cloud-Hackathon/projects/hackathon-projects.html), and the event summary: <https://earthdata.nasa.gov/learn/articles/2021-cloud-hackathon>.

## About

The **Cloud Hackathon: Transitioning Earthdata Workflows to the Cloud** is a virtual 5-day (4 hours per day) collaborative open science learning experience aimed at exploring, creating, and promoting effective cloud-based science and applications workflows using NASA Earthdata Cloud data, tools, and services (among others), in support of Earth science data processing and analysis in the era of big data. Its goals are to:



1. **Introduce** Earth science data users to NASA Earthdata cloud-based data products, tools and services in order to increase awareness and support transition to cloud-based science and applications workflows.
2. **Enable** science and applications workflows in the cloud that leverage NASA Earth Observations and capabilities (services) from within the NASA Earthdata Cloud, hosted in Amazon Web Services (AWS) cloud, thus increasing NASA Earthdata data utility and meaningfulness for science and applications use cases.
3. **Foster community engagement** utilizing Earthdata cloud tools and services in support of open science and open data.

**Outcome**: Participants prototype their science and applications workflows (via hackathon projects) that leverage Earthdata Cloud data and services (focusing on, but not limited to, oceanography, cryosphere, hydrology and land data), which supports them in their transition to cloud-based or hybrid workflows for data processing and analysis.

This is an opportunity for researchers that might not yet have had the opportunity to work in the Cloud to explore, learn and prototype workflows with NASA Earthdata in the Cloud, but more intermediate or advanced cloud users interested in further exploring cloud workflows with Earthdata Cloud data and service are also welcome.


## Application

### Information for applicants

The Cloud Hackathon will be a virtual event held November 15-19, 2021, where participants will explore the intersection of Earth science data, cloud computing, and big data analysis through demonstration tutorials and hands-on “hacking” projects. To best benefit from the event, we recommend some familiarity or experience with:

* NASA Earthdata data (focusing on oceanography, cryosphere, hydrology, cryosphere and land data, including interdisciplinary applications); and
* Programming skills using Python. We plan to accept participants with diverse skill levels and backgrounds in programming. However, to best benefit from and contribute to the program, participants are expected to have some experience with Python programming.

No cloud computing experience is required, but we encourage both beginner and more experienced participants with AWS cloud to apply.

If selected, participants will have the option to attend a Carpentries-style github, python, shell scripting clinic ahead of the Cloud Hachathon.

### Application Form

In the application form, we encourage you to think about and provide a science use case that you would like to prototype in the cloud. At the beginning of the hackathon, participants will be able to pitch their use case to support the formation of “hack” projects - by which we mean collaboratively experiment working in with NASA Earthdata data and capabilities in the Cloud. During the hackathon, participants will get into teams of their choosing, around a common use case to “hack” in the cloud. The use cases provided in the application form will also help the organizers best prepare materials tailored to those use cases.

**The application period has now closed. Thank you for your interest.**


## What to expect

* During the Cloud Hackathon, the selected participants will have access to cloud environments in AWS through a JupyterHub interface, provided through 2i2c.
* Participants will be guided on how to log into the cloud environment, import needed data recipes and resources, and will have the opportunity to explore and develop science and applications workflows in a cloud environment (hosted in AWS) using example tutorials as building blocks.
* The Cloud Hackathon is an open science event: all tutorials and examples are developed openly and will be publicly available during and following hackathon. Participants will strengthen their practice of open science, using open source code and “hacking” their projects openly to enable further discovery and contributions by the broader open community following the hackathon.
* Throughout the hackathon, participants will learn about NASA’s Earthdata move to the cloud and Earthdata APIs for data discovery, access, and transformations to enable faster, more efficient time to science.

In the two to three weeks leading up to the hackathon, participants are encouraged to review **background resources** that will facilitate a more effective hackathon experience. These resources will be shared here leading up to the Hackathon dates, and will be accessible to all data users, whether they attend the hackathon or not.

**The following datasets are currently available from the NASA Earthdata Cloud.** Participants can choose to prototype a cloud-based science workflow using a combination of these datasets, as well as other non-Earthdata Cloud data. If your preferred dataset is not yet available in the Earthdata Cloud, consider using a current cloud-based dataset as proxy to explore prototyping.


* [https://search.earthdata.nasa.gov/search?ff=Available%20from%20AWS%20Cloud](https://search.earthdata.nasa.gov/search?ff=Available%20from%20AWS%20Cloud)

**Example** **use** **cases** to explore in the cloud (note these are for inspiration only, you are not limited to these workflows):



* Use the advanced wildcard search capabilities in Earthdata Search Client/Common Metadata Repository (CMR) to precisely search/select all cloud-archived Sentinel-6A granules
    * from a specific cycle (i.e. a sequence orbits that together provide global spatial coverage), and/or
    * from a specific pass(es) over multiple cycles (i.e. selected orbits over a series of cycles that together provide a time series coverage).
    * Then, prepare the data for gridding or for local analysis at space/time scales which are appropriate for the target analysis (and limited by default given the length of S6A data record...)
* Time series analysis across multi-mission measurements spanning data housed both within and outside of NASA Earthdata Cloud, to develop a workflow that can accommodate different data locations, as data continue to migrate to the Cloud:
    * Programmatically search for a data variable (e.g. altimetry measurements) at a single point or area of interest across multiple datasets and identify whether the data are available in the Cloud
    * Acquire the data based on archived location and combine in order to produce a homogenous time series
* Explore/leverage cloud-optimized formats (COFs) such as Zarr to compute global or regional climatology and anomalies for a large-volume dataset (e.g. 1-km MUR SST) without having to download data (in-cloud analysis).
* Subset Level 2 swath dataset of interest spatially and for specific variable and do some exploratory analysis and visualization from within the cloud.
* Use NASA’s CMR-STAC API to search and discover Harmonized Landsat Sentinel-2 (HLS) cloud assets based on cloud data products, area of interest, and date range query parameters.
* Harmonized Landsat Sentinel-2 (HLS) for land monitoring: access, explore, and visualize time series surface reflectance data in the cloud.

This event is motivated by the dawn of the era of Big Data. NASA’s Earth Observing System Data and Information System (EOSDIS) is in the process of moving EOSDIS data to the cloud, driven by a rapid rate of data ingest into the EOSDIS archive. NASA remote sensing data from both upcoming (e.g. SWOT) and existing (e.g. Terra, Aqua, ICESat-2) missions will be available in the Earthdata Cloud platform in the coming years. The paradigm shift from on-premise (local) to cloud-based data distribution, and that from “download and analyze” to “analysis in place” present opportunities and challenges. Guiding users through this transition is of the utmost importance.

## Code of Conduct 

The 2021 Cloud Hackathon is a safe learning space and all participants are required to abide by our [Code of Conduct](https://openscapes.org/code-of-conduct).

## Acknowledgements

Cloud Hackathon: Transitioning Earthdata Workflows to the Cloud is co-hosted by NASA's PO.DAAC, NSIDC DAAC, LP.DAAC, with support from ASDC DAAC, GES DISC and the NASA Openscapes Project, and cloud computing infrastructure by 2i2c. <br>
![Screen Shot 2021-09-15 at 5 22 15 PM](https://user-images.githubusercontent.com/2915555/133525653-2a2278b1-1015-4350-b2a5-160d125aaaf7.png) <br>

We thank all of the additional NASA staff that have have joined as helpers.  

Thank you to the open science community that has created software, teaching resources, and workflows that we have been able to build heavily from! These include: 

- eScience Institute, University of Washington: 
  - <https://uwhackweek.github.io/hackweeks-as-a-service/intro.html>
  - <https://snowex-hackweek.github.io/website/intro.html>
  - <https://icesat-2hackweek.github.io/learning-resources/>
  
This hackathon book is made with [quarto](https://quarto.org). See the [earthdata-cloud-cookbook](https://nasa-openscapes.github.io/earthdata-cloud-cookbook/contributing/) to learn more about how we work and contributing.
