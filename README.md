# Summarise EU Water Quality Data 
This notebook creates a baseline water quality data for Europe as summarizing observations of total nitrogen (N) and total Phosphorous (P) concentrations, based on data from the European Environmental Agency's [Waterbase - Water Quality ICM, 2022](https://www.eea.europa.eu/en/datahub/datahubitem-view/fbf3717c-cd7b-4785-933a-d0cf510542e1). Firstly, it performs a temporal aggregation as obtaining the 75th percentile of annual means of nutrient concentrations, based on 1,047,387 data points (collected between 2000 and 2021) from 14,931 monitoring stations, using data from the Waterbase. Secondly, it performs a spatial aggregation as obtaining the average nutrient concentrations of monitoring stations within each river basin where they are located, using in this case [HydroBasins level 6](https://www.hydrosheds.org/products/hydrobasins) delineations.