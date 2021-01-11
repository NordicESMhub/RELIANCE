# Research Lifecycle Management technologies for Earth Science Communities and Copernicus users in EOSC (RELIANCE)

[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)


- INFRAEOSC-07-2020 Research and Innovation action. 
- Grant number 101017501. 
- 2 years project (01/2021 - 12/2022).


## Atmospheric and climate modelling Virtual Research Community (VRC) 

*Led by the University of Oslo, norway*

### Overview of the research community

At University of Oslo, the Department of Geosciences is heavily involved in research related to climate and the impacts of climate change to our societies and enenvironments. These encompass broad research fields which ignores the traditional boundaries between geoscience disciplines, hence many researchers contribute to international networks, centres and projects worldwide.

### Typical day of a researcher


### Walk through Nature Geoscience paper “Equilibrium climate sensitivity above 5 °C plausible due to state-dependent cloud feedback” - Jenny Bjordal,  Trude Storelvmo, Kari Alterskjær & Tim Carlsen 

[![DOI](https://img.shields.io/badge/DOI-10.1038%2Fs41561--020--00649--1-blue)](https://doi.org/10.1038/s41561-020-00649-1)

Galaxy Climate
#### (research/investigation) with demoes:

##### Data used: how was the data accessed (e.g., what repositories or locations). 

- All own CESM2 simulation outputs are available for download from Uninett Sigma: https://archive.sigma2.no/pages/public/datasetDetail.jsf?id=10.11582/2020.00028. - The standard CloudSat and CALIPSO data products (version R05) used in this study (2B-CWC-RO, 2C-ICE, ECMWF-AUX) were downloaded from the CloudSat Data Processing Center’s (at Cooperative Institute for Research in the Atmosphere, Colorado State University, Fort Collins) [website](http://www.cloudsat.cira.colostate.edu/). 

- All NCAR's CMIP6 historical surface air temperature data from CESM2 used in Fig. 1a is available through the Earth System Grid Federation (ESGF) server (https://esgf-data.dkrz.de/search/cmip6-dkrz/) under CMIP6, ‘source ID’ CESM2-FV2 and ‘experiment ID’ historical. The data used in this article were downloaded on 20 April 2020. 

- The dataset containing observed surface temperature, GISTEMP v4, was downloaded from https://data.giss.nasa.gov/gistemp/ on 6 May 2020. Source data are provided with this paper.


#### Software used: which software, give demo

- [CESM2](https://www.cesm.ucar.edu/models/cesm2/) code is available on [CESM github](https://github.com/ESCOMP/CESM) (which release ?)
- The code used to analyse satellite data is available [here](https://github.com/tim-carlsen/satellite-ecs-so) 
- The code used to calculate cloud feedbacks using radiative kernels is available [here](https://github.com/mzelinka/cloud-radiative-kernels).

#### Method used: workflows? scripts? where are they?

No specific worflow management system was used at the time, however the Department recently started to work with: 
- [Galaxy](https://galaxyproject.org/)
- [Snakemake](https://snakemake.readthedocs.io/)
- [Cylc](https://cylc.github.io/)

Workflows are then stored in [WorkflowHub](https://workflowhub.eu/) under topic Galaxy Climate.

#### Results: where results were deposited? 

- All own CESM2 simulation output is available for download from Uninett Sigma: https://archive.sigma2.no/pages/public/datasetDetail.jsf?id=10.11582/2020.00028. - [Extended data](https://www.nature.com/articles/s41561-020-00649-1#MOESM5)

#### Collaboration: how was the collaboration during this process?

- JupyterHub deployed through [NIRD toolkit](https://www.sigma2.no/nird-service-platform)


#### Challenges

#### Vision of EOSC for the community

- Synergies with [EOSC-nordic](https://www.eosc-nordic.eu/)

- More recently, researchers in the Nordics have access to [https://eosc-nordic.uiogeo-apps.sigma2.no/](https://eosc-nordic.uiogeo-apps.sigma2.no/) and [Galaxy Climate Workbench](https://climate.usegalaxy.eu/) ([JupyterLab pangeo](https://live.usegalaxy.eu/?tool_id=interactive_tool_climate_notebook), etc.).
- Soon researchers in the nordics will have access to a Nordic Galaxy Climate Workbench deployed on [https://usegalaxy.no/](https://usegalaxy.no/).

###  Case studies (WP7)

#### Multidisciplinary use case
- studies on 2020 lockdown

#### Vertical use cases introduction

- Grand Challenge 1: Sea pollution - case study 1
- Grand Challenge 2: Loss of Biodiversity and Sustainability (Biodiversity, fisheries, marine litter) – case study 2
- Grand Challenge 3: Extreme weather events and climate adaptation (biomass) – case study 3
- Grand Challenge 4: Reducing the consequences of large volcanic eruptions – case study 4 and 5


