---
title: "Tutorial: Using xarray to work with multidimensional geospatial datasets"
description: Provides hands-on tutorials on workflows to access the SCINet HPC systems and conduct geospatial research at scale and fosters geospatial research efforts.
excerpt: "In this tutorial you will learn the basic concepts of the Python library `xarray` while exploring its capabilities when working with multidimensional datasets with dimensions of time, latitude, and longitude. We will also touch on the capabilities of parallel processing using another Python library called `dask`."
 
categories: [2024 Geospatial Workshop] 

sidenav_link: /training/resources

time: 1:15 PM - 2:45 PM ET
lead: Erika Peirce
prerequisites:
  - text: Have a SCINet account and be able to login 
    url: /about/signup
  - text: Familiarity with Python and Jupyter notebooks. 
  - text: Familiarity with handling data using pandas.  
---

In this tutorial you will learn the basic concepts of the Python library `xarray` while exploring its capabilities when working with multidimensional datasets with dimensions of time, latitude, and longitude. We will also touch on the capabilities of parallel processing using another Python library called `dask`. 

Additional details and instructions for the tutorial will be added closer to the event. A recording of the tutorial will be added after the workshop concludes. 

## Tutorial setup instructions

Steps to prepare for the tutorial sessions:

1. **Login to Ceres Open OnDemand** at [https://ceres-ood.scinet.usda.gov/](https://ceres-ood.scinet.usda.gov/). For more information on login procedures for web-based SCINet access, see the [SCINet access user guide]({{site.baseurl}}/guides/access/web-based-login).

1. **Open a command-line session** by clicking on “Clusters” -> “Ceres Shell Access” on the top menu. This will open a new tab with a command-line session on Ceres' login node.

1. **Create and/or update your workshop working directory** and copy the tutorial materials into it by running the following commands. Note: you do not have to edit the commands with your username as it will be determined by the `$USER` variable. These commands will work for everyone, including if you attending previous workshop sessions or not. 

    {:.copy-code}
    ```bash
    mkdir -p /90daydata/shared/$USER/
    cd /90daydata/shared/$USER/
    cp -r /project/geospatialworkshop/2024/tutorial4 .
    source /project/geospatialworkshop/2024/grwg_2024_env/bin/activate
    ipython kernel install --name "grwg_2024_env" --user
    ```

1. **Launch a JupyterLab Server session.** Under the *Interactive Apps* menu, select *Jupyter*. Specify the following input values on the page:

    * Account: geospatialworkshop
    * Queue: short---------Max Time: 2-00:00:00
    * QOS: 400thread
    * Number of hours: 2
    * Number of cores: 8
    * Memory required: 16GB
    * Optional Slurm Arguments: \-\-reservation=workshop
    * Jupyter Notebook vs Lab: Lab
    * Working Directory: /90daydata/shared/${USER}
  
    Click *Launch*. The screen will update to the *Interactive Sessions* page. When your Jupyter session is ready, the top card will update from *Queued* to *Running* and a *Connect to Jupyter* button will appear. Click *Connect to Jupyter*.

1. For the notebook used in the tutorial, select the *grwg_2024_env* kernel.

