# Ocean Superfarms: Finding the Best Spots to Grow Seafood

![](figs/AdobeStock_921645340_Preview.svg)

## Description

Marine aquaculture is an increasingly important strategy for sustainably feeding growing human populations. Aquaculture, defined as the organized cultivation and production of aquatic organisms for commercial, recreational, or public use, supports food security, conservation, and economic development (Alleway et al., 2018). In California, aquaculture accounts for approximately 6% of the total value of the U.S. aquaculture industry and includes four main sectors: finfish, shellfish, algae, and natural resource agencies (Wright et al., 2025). Finfish and shellfish comprise over 70% of production value and are primarily produced for human consumption. Oysters and the critically endangered red abalone are two commercially significant species, with oysters dominating mollusk production in California. Oysters are typically restricted to sea surface temperatures (SST) of 11–30°C and depths of 0–70 meters (Oliver, 2025), while red abalone (*Haliotis rufescens*) prefer cooler SSTs of 8–18°C and depths of 0-25 meters (SeaBase, n.d.). Identifying overlapping suitable habitats within Exclusive Economic Zones (EEZs) may help guide sustainable aquaculture development.

The purpose of this assignment is to evaluate the suitability of West Coast Exclusive Economic Zones (EEZs) for developing marine aquaculture for multiple oyster species and an additional selected species, red abalone. Suitable locations are determined based on species-specific ranges of sea surface temperature (SST) and depth. The assignment incorporates methods for working with both vector and raster data, including raster resampling and masking, as well as the application of map algebra techniques. The project consists of two components: (1) following a standardized workflow to create a final map of suitable oyster aquaculture areas in West Coast EEZs, and (2) developing a function that generates maps of suitability by EEZ based on user defined temperature ranges, depth limits, and species selection.

## Repository Structure

This repository contains:

```         
suitability-aquaculture-analysis
│   README.md
│   aquaculture_suitability_analysis.qmd
│   aquaculture_suitability_analysis.pdf
│   eds-223-hw-2.Rproj
│   figs
│   └───AdobeStock_921645340_Preview.svg
│   └───red-abalone.png
│   └───kelp_forest.png
│
└───.gitignore
     └───data
         └───wc_regions_clean.prj
         └───depth.tif
         └───average_annual_sst_2008.tif
         └───average_annual_sst_2009.tif
         └───average_annual_sst_2010.tif
         └───average_annual_sst_2011.tif
         └───average_annual_sst_2012.tif
```

## Data Description & Access

[SeaLifeBase](https://www.sealifebase.ca/search.php) is a publicly available online database that provides information on a wide range of marine species based on criteria such as commercial importance and taxonomic group. Each species profile includes details on depth range, temperature preference, geographic distribution, life history, and classification. The database is open access and does not require any downloads to use.

For this analysis, West Coast Exclusive Economic Zone (EEZ) boundaries were obtained from Marineregions.org to define maritime boundaries. The [General Bathymetric Chart of the Oceans (GEBCO)](https://www.gebco.net/data_and_products/gridded_bathymetry_data/#area) is a global terrain model that provides geospatial information, such as elevation, for both ocean and land surfaces at a 15-arc-second grid resolution (GEBCO, n.d.). Bathymetry data for this analysis were downloaded from GEBCO as a `tif` file. This analysis also used satellite-derived average sea surface temperature (SST) data from 2008–2012 to characterize mean SST within each EEZ. Although the GeoTIFF files were provided through course materials, the original data are publicly available from [NOAA’s 5 km Daily Global Satellite Sea Surface Temperature Anomaly v3.1 product](https://coralreefwatch.noaa.gov/product/5km/index_5km_ssta.php).

## Authors & Additional Contributions

This repository is maintained by Vedika Shirtekar as part of the Master of Environmental Data Science program at the University of California, Santa Barbara. Thank you to the Bren School of Environmental Science and Management for facilitating data access and documentation.

## References

[1] Alleway, H. K., Gillies, C. L., Bishop, M. J., Gentry, R. R., Theuerkauf, S. J., & Jones, R. (2018). *The ecosystem services of marine aquaculture: Valuing benefits to people and nature*. BioScience, 69(1), 59–68. <https://doi.org/10.1093/biosci/biy137>

[2] California Conservation Genomics Project. (n.d.). *Haliotis rufescens (Red Abalone)*. Retrieved November 29, 2025, from <https://www.ccgproject.org/species/haliotis-rufescens-red-abalone>

[3] *Gridded bathymetry data*. (n.d.). GEBCO. Retrieved November 30, 2025, from <https://www.gebco.net/data-products/gridded-bathymetry-data#area>

[4] *Haliotis rufescens, Red abalone: Fisheries.* (n.d.). Retrieved November 30, 2025, from <https://www.sealifebase.ca/summary/Haliotis-rufescens.html>

[5] Hausheer, J. E. (2023). *Aquaculture Could Be Conservation’s Secret Weapon.* The Nature Conservancy. Retrieved November 29, 2025, from <https://blog.nature.org/2019/01/21/aquaculture-could-be-conservations-secret-weapon/>

[6] *Marine regions.* (n.d.). Retrieved November 28, 2025, from <https://www.marineregions.org/eez.php>

[7] *Monterey Bay Abalone farm shows what sustainable aquaculture can be like.* (n.d.). Earth Island Journal. Retrieved November 29, 2025, from <https://www.earthisland.org/journal/index.php/articles/entry/monterey_bay_abalone_farm_shows_what_sustainable_aquaculture_can_be_like/>

[8] *NOAA coral reef watch daily 5km satellite coral bleaching heat stress SST anomaly product* (version 3.1). (n.d.). Retrieved November 29, 2025, from <https://coralreefwatch.noaa.gov/product/5km/index_5km_ssta.php>

[9] Oliver, R. (2025). *Homework assignment 4.* Retrieved November 28, 2025, from <https://eds-223-geospatial.github.io/assignments/HW4.html#fnref1>

[10] Wright, A., Moody, C., & Gross, J. (2025). *Composition of California’s aquaculture industry and surveying its disease challenges and management strategies.* Aquaculture Reports, 42, 102799. Retrieved November 29, 2025, from <https://doi.org/10.1016/j.aqrep.2025.102799>
