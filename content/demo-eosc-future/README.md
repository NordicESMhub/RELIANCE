# Demo for EOSC-Future

The two notebooks:
- RELIANCE-Datacube-featuring-EOSC_v0.2.ipynb
- RELIANCE_v0.2-France.ipynb

demonstrate the use of ADAM-API and RoHUB-API from Python Jupyter notebooks. 

During the demo, they have been executed on a "bundle" EGI-notebook + B2DROP and this is why some results in RELIANCE_v0.2-France.ipynb are saved in a folder called `b2drop`. This folder is not created by the user but is automatically available as part of the EGI-notebook + B2DROP bundle service. Everything you store in the `b2drop` folder is saved in your B2DROP account. 

1. It won't work if you are not using EGI-notebook + B2DROP bundle service. Then you can removed b2drop where saving results and store everything locally on your notebook and then as internal resource in RoHUB.
2. To make sure we do not share our credentials, username, passwords and/or API keys are stored in files. These files need to exist and contain your credentials before running the notebooks.

## What do we do on the two notebooks?

The structure of the two notebooks are very similar:

1. Authentication to ADAM-API: make sure to create a file `adam-key` with your ADAM-API key;
2. Datasets Discovery: we discover all the datasets but when going through them, we only print `EU_CAMS` results (you need to change it for your own datasets). In this step, we also get the dataset identifiers. We have selected a dataset identifier `69626:EU_CAMS_SURFACE_PM10_G`. Adapt it for your own datasets;
3. Products Discovery: we discover products over a specific area (Italy or France) and specific time range. The geometry for the spatial search is provided as `geojson` (I haven't fully understood which encoding standard to follow: some of my geojson files worked and some did not);
4. Data Access: ADAM-Api returns a `zip` file containing the results of your request. You need to unzip it to analyze your data;
5. Data Analysis and Visualization: when `geotiff`, I read all the data with `xarray`. 

In the second notebook `RELIANCE_v0.2-France.ipynb`, there is an additional step for saving the results into a code-centred Research Object in RELIANCE.

You would need to authenticate to RoHUB:
- `rohub-user` contains your username (not sure what to do when using ORCID)
- `rohub-pwd` contains your password.

When adding geolocation, I could not use the same geojson I used with ADAM-API. Your geojson needs to follow OGC EO Dataset Metadata GeoJSON(-LD) Encoding Standard (added in this repo).

