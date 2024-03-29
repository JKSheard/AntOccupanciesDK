# AntOccupanciesDK

Authors: [Julie K. Sheard](https://github.com/JKSheard)

This repository contains the code for:
>Sheard, J.K., Rahbek, C., Dunn, R.R., Sanders, N.J. & Isaac, N.J.B. (2021) Long-term trends in the occupancy of ants revealed through use of multi-sourced data sets. Biology Letters 17: 20210240. https://doi.org/10.1098/rsbl.2021.0240 

## Data
We used seven sources of data: 1. pinned specimen records from the Natural History Museum of Denmark, 2. pinned specimen records from the Natural History Museum of Aarhus, 3. specimen records from the Natural History Museum of Stavanger, collected by Holger Holgersen, 4. observation records from AntWeb collected by Sämi Schär, 5. observation records from Christian Skøtt, 6. observation records from the EuroAnts course and 7. preserved specimen records from the Ant Hunt. The raw data sets are available from GBIF:

>Calabuig I (2014). Danish Ants (Formicidae). Zoological Museum, Natural History Museum of Denmark. Occurrence dataset https://doi.org/10.15468/xcwkfb

>Simonsen T, Sheard J K (2021). Natural History Museum Aarhus Ant Collection. Version 1.2. Natural History Museum Aarhus. Occurrence dataset https://doi.org/10.15468/wp3kzr

>Fiskå A (2018). MUST, Insecta. Version 9.266. Museum Stavanger. Occurrence dataset https://doi.org/10.15468/zkm8mj

>Fisher B, Fong J (2021). AntWeb. California Academy of Sciences. Occurrence dataset https://doi.org/10.15468/wqmjjt

>Sheard J K, Nielsen, M G, Pedersen, J (2020). Skoett Ant Collection. Center for Macroecology, Evolution and Climate, University of Copenhagen. Occurrence dataset https://doi.org/10.15468/2xh5fd

>Sheard J K, Nash D R (2020). Euroants. Department of Biology, University of Copenhagen. Occurrence dataset https://doi.org/10.15468/jpacce

>Sheard J K, Sanders N J, Dunn R R, Rahbek C (2021). The Danish Ant Hunt. Version 1.9. Center for Macroecology, Evolution and Climate, University of Copenhagen. Sampling event dataset https://doi.org/10.15468/dcijnc

These were manually georeferenced and cleaned so that we excluded detections of unidentified species, those without collection date or geographic coordinates and non-native species. Using ArcGIS, remaining data were binned into 10 x 10 km grid cells and 10 year time-periods (decades). The combined data set used in this study has been uploaded to Dryad. When using, please cite:

>Sheard J K, Rahbek C, Dunn R R, Sanders N J, Isaac N J (2021). Data from: Long-term trends in the occupancy of ants revealed through multi-sourced data sets. Dryad, Dataset, https://doi.org/10.5061/dryad.bnzs7h4bj

## Analysis outputs

Based on the analyses of the combined data, further data sets were created, which have been uploaded here. The full model results have been uploaded to Dryad together with the original data and can be found here: https://doi.org/10.5061/dryad.bnzs7h4bj

* ci_decades.csv
* detections_decades.csv
* first_last_record.csv
* occupancy plot.csv

## Scripts

#### Code for analyses

* 01-format-data.Rmd
* 02-run-model.Rmd
* 03-occupancy-analysis.Rmd
* 04-occupancy-change.Rmd
* 05-model-uncertainty.Rmd

#### Code for figures

* fig 1a-temporal distribution.Rmd
* fig 2-occupancy trends.Rmd
* fig S3-list lengths.Rmd
* fig S4-individual species plots.Rmd
* fig S7-uncertainty.Rmd

#### Code for functions

The following functions are used to create figure S4
* Plot_DetectionOne.R
* plot_Detection12.R

#### Not included

* Figure 1b, which was created using ArcGIS
* Figure S2, which was created using ArcGIS
