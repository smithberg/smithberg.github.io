---
layout: default
title: Eli Smithberg
description: Earth Data Science portfolio
---

# About Me
Undergrad at CU Boulder, double major in Geography (GIS Concentration) and Atmospheric & Oceanic Science.

<img 
  src="/img/pfp.jpg" 
  height="40%"
  width="40%">

### Contact Info
- eli.smithberg@colorado.edu
- [LinkedIn](https://www.linkedin.com/in/eli-smithberg-b67bb9368/)
- [GitHub](github.com/smithberg)

***

# Portfolio

### Map of Pappajohn Sculpture Park in Des Moines, IA
<embed type="text/html" src="sculpture_park_interactive.html" width="600" height="600">

### Mean Annual High Temperatures in Des Moines, IA
The following plot displays the mean daily high temperature in Des Moines for every year from 1946 to 2024 (the full extent of the data, minus incomplete years). Data was collected from the Des Moines International Airport (<https://www.ncdc.noaa.gov/cdo-web/datasets/GHCND/stations/GHCND:USW00014933/detail>).
<iframe src="des moines temperature plot.html" width="800" height="350" style="border:none;"></iframe>

To determine the historical trend of high temperatures in Des Moines, we can perform a **linear OLS regression** on the data, as shown in the following plot:
![Linear OLS Plot](img/des moines temp ols.png)

The OLS regression line gives an average increase in mean annual high temperature of 0.0353 degrees Fahrenheit per year from 1946 to 2024. With a t-statistic of t=3.908, the data strongly suggest that the temperature in Des Moines is increasing on average. This may be evidence of global warming, although the scope of the data is limited to Des Moines.

### Mapping Red-headed Woodpecker (*Melanerpes erythrocephalus*) Migration in 2024
<iframe src="melanerpes_erythrocephalus_migration_2024_interactive.html" 
        width="100%" height="600px" 
        style="border:1px solid #ccc;">
</iframe>
This interactive map panel illustrates the density of *Melanerpes erythrocephalus* spottings by ecoregion for each month in 2024, color-coded on a logarithmic scale.
- Regions on the map are derived from [RESOLVE's *Ecoregions of the World* (2017)](https://www.resolve.ngo/projects/ecoregions-world)
- *Melanerpes erythrocephalus* migration data was downloaded from [Global Biodiversity Information Facility (GBIF)](https://www.gbif.org/species/2478130)

The data shown in this panel reveals that *Melanerpes erythrocephalus* occupy the eastern and central parts of the United States, as well as part of southern Canada, year-round. However, much of the northwestern United states and western Canada appear to be occupied by *Melanerpes erythrocephalus* primarily in summer months. The data suggest that some *Melanerpes erythrocephalus* exhibit a seasonal migration pattern in which they migrate northwest in the spring and southeast in the fall. The dry and mountainous topography of the southeastern United States is likely inhospitable to *Melanerpes erythrocephalus* and thus may help explain the migration pattern we see in the panel.

