# OGC-biomass

Data, metadata, and R code for “Taxon-specific biomass declines in a blackwater river: the importance of a community approach to understanding invertebrate loss.”
================
David Murray-Stoker
7 March 2022

Data, metadata, and all analytical code for the manuscript:

Murray-Stoker, K. M. et al. Taxon-specific biomass declines in a blackwater river: the importance of a community approach to understanding invertebrate loss.

## Abstract

1.	Around the world, researchers are reporting declines in insect fauna. Though uncommonly evaluated in such studies, the community context of population trends can facilitate interpretation of the causes and consequences of such losses. 
2.	We used a multivariate approach to compare the structure of freshwater invertebrate assemblages separated by more than 30 years in the Ogeechee River, in the southeastern US, and found biomass declines. 
3.	Overall, the biomass in the 2010s was approximately 60% of the total in the 1980s. Community analyses indicated that this decline was driven by reduced densities of large-bodied, filter-feeding insects, particularly Hydropsychidae caddisflies (Trichoptera). Conversely, predators and small-bodied primary consumers increased in density, though their contributions to overall biomass were minimal and their increased density was not sufficient to compensate for biomass declines. 
4.	The overall decline of freshwater invertebrate biomass may be driven by climate-related changes in flood dynamics: seasonal flooding that facilitates delivery of floodplain carbon to filter-feeding consumers has decreased over several decades. Water temperature had also increased and has likely had effects on the invertebrate assemblages. 
5.	Whole-community evaluations such as this one, in contrast to single-taxon and abundance-based studies, provide critical information to elucidate the dynamics of freshwater impairment and insect loss in the Anthropocene.


## Contents


The [R Project](https://github.com/dmurraystoker/OGC-biomass/blob/main/OGC-biomass.Rproj) provides a local relative directory for all data and R code.


### Data

All processed data are provided in the [data folder](https://github.com/dmurraystoker/OGC-biomass/tree/main/data), with the raw data available in the [raw data folder](https://github.com/dmurraystoker/OGC-biomass/tree/main/data_raw). Metadata are provided [here](https://github.com/dmurraystoker/OGC-biomass/blob/main/metadata.md).


### R Code & Data Analysis Summary Reports

R code and summary reports are provided in the [data analysis folder](https://github.com/dmurraystoker/OGC-biomass/tree/main/data_analysis). Data management and primary analyses were conducted using the [OGC-biomass-primary_analyses.Rmd](data_analysis/OGC-biomass-primary_analyses.Rmd) code, and the associated primary analyses workspace is also provided ([OGC-biomass-primary_analyses-workspace.RData](data_analysis/OGC-biomass-primary_analyses-workspace.RData)). Environmental comparisons were conducted using the [OGC-biomass-environmental_comparisons.Rmd](data_analysis/OGC-biomass-environmental_comparisons.Rmd) code, and the associated environmental comparisons workspace is also provided ([OGC-biomass-environmental_comparisons-workspace.RData](data_analysis/OGC-biomass-environmental_comparisons-workspace.RData))


### Using the Repository

To use the data and R code for this project:
1. `git clone` this repository or download it as a zip folder
2. Open `R Studio`, go to `file > Open project` and open the `OGC-biomass.Rproj`
R Project associated with this repository.
3. Analyses can be done using code in the [data analysis folder](https://github.com/dmurraystoker/OGC-biomass/tree/main/data_analysis)

