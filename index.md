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
<iframe src="melanerpes_erythrocephalus_migration_2024_interactive.html" width="160%" height="600px" style="border:1px solid #ccc;"> </iframe>
This interactive map panel illustrates the density of *Melanerpes erythrocephalus* spottings by ecoregion for each month in 2024, color-coded on a logarithmic scale.
- Regions on the map are derived from [RESOLVE's *Ecoregions of the World* (2017)](https://www.resolve.ngo/projects/ecoregions-world)
- *Melanerpes erythrocephalus* migration data was downloaded from [Global Biodiversity Information Facility (GBIF)](https://www.gbif.org/species/2478130)

The data shown in this panel reveals that *Melanerpes erythrocephalus* occupy the eastern and central parts of the United States, as well as part of southern Canada, year-round. However, much of the northwestern United states and western Canada appear to be occupied by *Melanerpes erythrocephalus* primarily in summer months. The data suggest that some *Melanerpes erythrocephalus* exhibit a seasonal migration pattern in which they migrate northwest in the spring and southeast in the fall. The dry and mountainous topography of the southeastern United States is likely inhospitable to *Melanerpes erythrocephalus* and thus may help explain the migration pattern we see in the panel.

### Impact of the Restoration of Water Rights to the Gila River Indian Community
In 2004, the Akimel O’otham and Tohono O’odham tribes won a US Supreme Court settlement granting them water rights. Using Normalized difference vegetation index (NDVI) data, we can observe the effects of the restoration of said water rights on vegetation health in the Gila River Reservation, located in southern Arizona. 

The average NDVI in and around the Gila River Indian Community (GRIC) from 2001-2004, alongside that from 2005-2008, are shown below:
![GRIC mean NDVI 2001-2004 2005-2008](gric-ndvi-comparison.png)

To examine the impact of the restoration of water rights to the Gila River Indian Community on vegetation health, we can subtract the 2005-2008 average for each NDVI tile by the 2001-2004 average and map the difference:
<iframe src="gric-ndvi-difference-hvplot.html"
        width="100%"
        height="600"
        frameborder="0">
</iframe>
The arrayed green circles on this map strongly suggest that center-pivot irrigation was established inside the GRIC following the 2004 settlement. This map suggests that overall vegetation health changed relatively little between the periods 2001-2004 and 2005-2008, with minor fluctuations.

To more directly assess whether restoring water rights to the GRIC led to an increase in vegetation health, we can subtract average july NDVI inside the GRIC by that in the region surrounding it (defined by the GRIC's north, south, east, and west bounds) for each year since 2001, and then graph the difference over time: 
<iframe src="ndvi-deficit-graph.html"
        width="100%" 
        height="500" 
        frameborder="0" 
        style="border: none;">
</iframe>
This graph shows a general reduction in the Gila River Indian Community's NDVI deficit compared to the surrounding areas since 2004, the year water rights were restored to the community. There is also a sharp reduction in the deficit between 2004 and 2005, though the deficit returns roughly to where it was before 2004. From this data, it can be inferred that the restoration of water rights in 2004 led to a sharp reduction in the NDVI deficit the following year, while the changes following 2005 are likely better explained by other factors.

##### Sources
https://earthdatascience.org/notebooks/05-vegetation/vegetation-eds.html
https://github.com/earthlab-education/Earth-Analytics-AY25/issues/244
