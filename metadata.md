Metadata for “Taxon-specific biomass declines in a blackwater river: the importance of a community approach to understanding invertebrate loss”
================
Kelly M. Murray-Stoker, Joseph V. McHugh, Arthur C. Benke, Keith A. Parsons, David Murray-Stoker, Amy D. Rosemond, Seth J. Wenger, Darold P. Batzer

# OGC-biomass

Metadata associated with the manuscript:

Murray-Stoker, K. M. et al. Taxon-specific biomass declines in a blackwater river: the importance of a community approach to understanding invertebrate loss.

# Metadata


## Raw Data

Raw data were imported into R for initial data processing and management (files = OGC\_biomass_data\-1982.csv, OGC\_biomass_data\-1983.csv, OGC\_biomass_data\-2010s.csv). Data were cast into wide biomass-by-taxa (files = OGC\_1982\_biomass\_by\_taxa.csv, OGC\_1983\_biomass\_by\_taxa.csv, OGC\_2010s\_biomass\_by\_taxa.csv) and density-by-taxa (files = OGC\_1982\_density\_by\_taxa.csv, OGC\_1983\_density\_by\_taxa.csv, OGC\_2010s\_density\_by\_taxa.csv) matrices. Final data management was conducted using Excel (see Processed Data below).


### file = OGC\_biomass_data\-1982.csv

| Variable   | Description                                                                    |
|:-----------|:-------------------------------------------------------------------------------|
| Date       | Sampling date in the format YYYYMMDD 																					|
| Snag       | Numerical identifier for the snag from which invertebrates were collected      |
| Order      | Order classification based on morphological identification 										|
| Family     | Family classification based on morphological identification										|
| Genus      | Genus classification based on morphological identification 										|
| Head       | Head capsule width (mm) for use in biomass estimates 													|
| Length     | Body length (mm) for use in biomass estimates																  |
| Density    | Number of individuals standardized by snag area																|
| a          | Taxon-specific constant for biomass estimates based on Benke et al. 1999 (JNABS) |
| b          | Taxon-specific constant for biomass estimates based on Benke et al. 1999 (JNABS) |
| Individual_Biomass    | Biomass estimate for that specific taxon in the sample								|
| Section 							| Body section from which biomass was estimated following Benke et al. 1999 (JNABS |
| Biomass_Estimate      | Density $\times$ Individual_Biomass 																	|



### file = OGC\_biomass\_data\-1983.csv

| Variable   | Description                                                                    |
|:-----------|:-------------------------------------------------------------------------------|
| Date       | Sampling date in the format YYYYMMDD 																					|
| Snag       | Numerical identifier for the snag from which invertebrates were collected      |
| Order      | Order classification based on morphological identification 										|
| Family     | Family classification based on morphological identification										|
| Genus      | Genus classification based on morphological identification 										|
| Head       | Head capsule width (mm) for use in biomass estimates 													|
| Length     | Body length (mm) for use in biomass estimates																  |
| Density    | Number of individuals standardized by snag area																|
| a          | Taxon-specific constant for biomass estimates based on Benke et al. 1999 (JNABS) |
| b          | Taxon-specific constant for biomass estimates based on Benke et al. 1999 (JNABS) |
| Individual_Biomass    | Biomass estimate for that specific taxon in the sample								|
| Section 							| Body section from which biomass was estimated following Benke et al. 1999 (JNABS |
| Biomass_Estimate      | Density $\times$ Individual_Biomass 																	|



### file = OGC\_biomass\_data\-2010s.csv

| Variable   | Description                                                                    |
|:-----------|:-------------------------------------------------------------------------------|
| Date       | Sampling date in the format YYYYMMDD 																					|
| Snag       | Numerical identifier for the snag from which invertebrates were collected      |
| Order      | Order classification based on morphological identification 										|
| Family     | Family classification based on morphological identification										|
| Genus      | Genus classification based on morphological identification 										|
| Head       | Head capsule width (mm) for use in biomass estimates 													|
| Length     | Body length (mm) for use in biomass estimates																  |
| Density    | Number of individuals standardized by snag area																|
| a          | Taxon-specific constant for biomass estimates based on Benke et al. 1999 (JNABS) |
| b          | Taxon-specific constant for biomass estimates based on Benke et al. 1999 (JNABS) |
| Individual_Biomass | Biomass estimate for that specific taxon in the sample								    |
| Section 					 | Body section from which biomass was estimated following Benke et al. 1999 (JNABS |
| Biomass_Estimate   | Density $\times$ Individual_Biomass 																	    |



### file = OGC\_1982\_biomass\_by\_taxa.csv

| Variable(s) | Description                                                          |
|:------------|:---------------------------------------------------------------------|
| UID         | Unique identifier for the sample, in the data format YYYYMMDD        |
| Acroneuria:Shipsa | Biomass estimate for each taxon in the sample; taxa were primarily identified to genus |



### file = OGC\_1983\_biomass\_by\_taxa.csv

| Variable(s) | Description                                                          |
|:------------|:---------------------------------------------------------------------|
| UID         | Unique identifier for the sample, in the data format YYYYMMDD        |
| Acroneuria:Tipulidae | Biomass estimate for each taxon in the sample; taxa were primarily identified to genus |



### file = OGC\_2010s\_biomass\_by\_taxa.csv

| Variable(s) | Description                                                          |
|:------------|:---------------------------------------------------------------------|
| UID         | Unique identifier for the sample, in the data format YYYYMMDD        |
| Acroneuria:Tipulidae | Biomass estimate for each taxon in the sample; taxa were primarily identified to genus |



### file = OGC\_1982\_density\_by\_taxa.csv

| Variable(s) | Description                                                          |
|:------------|:---------------------------------------------------------------------|
| UID         | Unique identifier for the sample, in the data format YYYYMMDD        |
| Acroneuria:Shipsa | Density estimate for each taxon in the sample; taxa were primarily identified to genus |



### file = OGC\_1983\_density\_by\_taxa.csv

| Variable(s) | Description                                                          |
|:------------|:---------------------------------------------------------------------|
| UID         | Unique identifier for the sample, in the data format YYYYMMDD        |
| Acroneuria:Tipulidae | Density estimate for each taxon in the sample; taxa were primarily identified to genus |



### file = OGC\_2010s\_density\_by\_taxa.csv

| Variable(s) | Description                                                          |
|:------------|:---------------------------------------------------------------------|
| UID         | Unique identifier for the sample, in the data format YYYYMMDD        |
| Acroneuria:Tipulidae | Density estimate for each taxon in the sample; taxa were primarily identified to genus 



## Processed Data

Raw data were initially processed in R using `reshape2` and the `tidyverse`, with finally processing and management on biomass, density, and long-term environmental data conducted in Excel.

Note: Environmental comparisons between sampling periods and season (i.e. ANOVAs) were conducted using environmental variables in the OGC\_final\_biomass\_data.csv file, while longer-term comparisons, including time before and between sampling periods, were conducted using environmental variables in the OGC\_long\_term\_environmental\_data.csv file.



### file = OGC\_final\_biomass\_data.csv

| Variable       | Description                                                          |
|:---------------|:---------------------------------------------------------------------|
| UID            | Unique sample identifier following the date format YYYYMMDD          |
| Year           | Sampling year in the study (character)                               |
| Year_Recoded   | Sampling year in the study (ordinal)                                 |
| Season         | Season in which the sample was collected (character)                 |
| Season_Recoded | Season in which the sample was collected (ordinal)                   |
| Period         | Indicates whether the sample was from the 1980s or 2010s (character) |
| CaCO           | Calcium carbonate (mg/L) from a single grab-sample each month (numeric); USGS Oliver Gage 02202190            |
| Carbon         | Dissolved organic carbon (mg/L) from a single grab-sample each month (numeric; USGS Oliver Gage 02202190)     |
| Conductivity   | Conductivity (microsiemens per cm) from a single grab-sample each month (numeric); USGS Oliver Gage 02202190  |
| DO             | Dissolved oxygen (mg/L) from a single grab-sample each month (numeric); USGS Oliver Gage 02202190             |
| pH             | pH from a single grab-sample each month (numeric); USGS Oliver Gage 02202190                                  |
| Water_Temperature | Water temperature (&deg;C) on the sampling date (numeric); USGS Oliver Gage 02202190                       |
| Precipitation     | Monthly sum of precipitation (cm) (numeric); NOAA Louisville                                               |
| Air_Temperature   | Monthly avergage of air temperature (&deg;C) (numeric); NOAA Louisville                                    |
| Mean_Discharge    | Mean daily discharge (m^3^ s^-1^) in the 2-weeks preceding the sampling date (numeric); USGS Eden Gage 02202500 |
| Amphinemura:Plecoptera | Biomass estimates for each taxon in the sample; taxa were primarily identified to genus (numeric)     |
| Summed_Biomass | Summed biomass estimates across all taxa present in the sample (numeric)                                      |



### file = OGC\_final\_density\_data.csv

| Variable       | Description                                                          |
|:---------------|:---------------------------------------------------------------------|
| UID            | Unique sample identifier following the date format YYYYMMDD          |
| Year           | Sampling year in the study (character)                               |
| Year_Recoded   | Sampling year in the study (ordinal)                                 |
| Season         | Season in which the sample was collected (character)                 |
| Season_Recoded | Season in which the sample was collected (ordinal)                   |
| Period         | Indicates whether the sample was from the 1980s or 2010s (character) |
| CaCO           | Calcium carbonate (mg/L) from a single grab-sample each month (numeric); USGS Oliver Gage 02202190            |
| Carbon         | Dissolved organic carbon (mg/L) from a single grab-sample each month (numeric; USGS Oliver Gage 02202190)     |
| Conductivity   | Conductivity (microsiemens per cm) from a single grab-sample each month (numeric); USGS Oliver Gage 02202190  |
| DO             | Dissolved oxygen (mg/L) from a single grab-sample each month (numeric); USGS Oliver Gage 02202190             |
| pH             | pH from a single grab-sample each month (numeric); USGS Oliver Gage 02202190                                  |
| Water_Temperature | Water temperature (&deg;C) on the sampling date (numeric); USGS Oliver Gage 02202190                       |
| Precipitation     | Monthly sum of precipitation (cm) (numeric); NOAA Louisville                                               |
| Air_Temperature   | Monthly avergage of air temperature (&deg;C) (numeric); NOAA Louisville                                    |
| Mean_Discharge    | Mean daily discharge (m^3^ s^-1^) in the 2-weeks preceding the sampling date (numeric); USGS Eden Gage 02202500 |
| Amphinemura:Plecoptera | Density estimates for each taxon in the sample; taxa were primarily identified to genus (numeric)     |
| Summed_Density | Summed density estimates across all taxa present in the sample (numeric)                                      |



### file = OGC\_long\_term\_environmental\_data.csv

| Variable       | Description                                                            |
|:---------------|:-----------------------------------------------------------------------|
| ID	               | Unique identifier in the format YY_MMM (e.g., 70_Dec)                                       |
| Year              | Year associated with the calculated environmental variable measurements                      |
| Month	            | Month associated with the calculated environmental variable measurements                     |
| Season_Year       | Flooding season (summer-fall = SF, winter=spring = WS) and year to identify the measurements |
| Season            | Season associated with the calculated environmental variable measurements                    |
| Season_Group      | Flooding season (summer-fall = SF, winter=spring = WS) group to identify the measurements    |
| Mean_Discharge    | Mean monthly discharge (m^3^ s^-1^); USGS Eden Gage 02202500                                 |
| Precipitation	    | Mean monthly precipitation (cm); NOAA Louisville                                             |
| Air_Temperature	  | Mean monthly air temperature (&deg;C); NOAA Louisville                                       |
| Water_Temperature | Monthly water temperature (&deg;C) from a single grab-sample; USGS Oliver Gage 02202190      |



