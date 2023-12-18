# Summarise EU Water Quality Data 
This repository creates a baseline water quality data for Europe as summarizing observations of total nitrogen (N) and total Phosphorous (P) concentrations, based on data from the European Environmental Agency's Waterbase - Water Quality ICM, 2022. Firstly, it performs a temporal aggregation as obtaining the 75th percentile of annual means of nutrient concentrations, based on 1,047,387 data points (collected between 2000 and 2021) from 14,931 monitoring stations, using data from the Waterbase. Secondly, it performs a spatial aggregation as obtaining the average nutrient concentrations of monitoring stations within each river basin where they are located, using in this case HydroBasins level 6 delineations (as in the SBTN State of Nature Water Layers). See code above in [summarise_water_quality_from_waterbase.qmd](https://github.com/Qnature/summarise_waterbase/blob/main/summarise_water_quality_from_waterbase.qmd)

Data Sources:
- [Waterbase - Water Quality ICM, 2022](https://www.eea.europa.eu/en/datahub/datahubitem-view/fbf3717c-cd7b-4785-933a-d0cf510542e1)
- [WISE WFD Reference Spatial Datasets reported under Water Framework Directive](https://sdi.eea.europa.eu/data/b15c7595-8e41-45ff-b657-a62f411e3f42)
- [State of Nature layers for Water Availability and Water Pollution to support SBTN Step 1](https://zenodo.org/records/7797979)

The main output is a shapefile containing baseline nutrient concentrations:

- Total Nitrogen (N) Concentration
![hydrobasins6_n_concentration](https://github.com/Qnature/summarise_waterbase/assets/136806514/447a8514-3ab7-4a7a-8d32-1382b97b54bd)

- Total Phosphorous (P) Concentration
![hydrobasins6_p_concentration](https://github.com/Qnature/summarise_waterbase/assets/136806514/555fdfb1-d2cb-461b-b5b6-5d71965ddade)
