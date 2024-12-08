# Prioritizing Potential Aquaculture
## A Functional Analysis of West Coast Economic Zones
Author: Ian Morris-Sibaja

![Image](https://i0.wp.com/calmatters.org/wp-content/uploads/2020/05/NOAA_Mussellonglines_02.jpg?fit=1200%2C799&ssl=1) A large mussel farming operation is proposed for the waters off Ventura. Photo by South Australian Research and Development Institute via NOAA [Cal Matters](https://calmatters.org/environment/2020/05/california-shellfish-farming-aquaculture/)

## About
This project takes a look at suitable habitats for marine aquaculture species along the U.S. West Coast, highlighting its potential as a sustainable protein source. Key objectives include:

-   Mapping species-specific habitats based on sea surface temperature and depth.
-   Streamlining geospatial data collection, processing, and visualization.
-   Creating a reusable workflow function.

## Repository organization
```
 suitable-habitats
|   suitable-habitats.html
|   suitable-habitats.qmd
│   README.md
|   suitable-habitats.Rproj
|   .gitignore 

```

## Data

### Suitable growing conditions
Our constants to use for our suitable growing conditions are found on the [SeaLifeBase](https://www.sealifebase.ca/search.php) interactive database.
#### Oysters:
Research has shown that oysters need the following conditions for optimal growth:
- Sea surface temperature: 11-30°C
- Depth: 0-70 meters below sea level

Therefore we use those constants for our oyster analysis. 
#### Chinese Mitten crab:
Research has shown that Chinese Mitten crabs need the following conditions for optimal growth:
- Sea surface temperature: 5-27°C
- Depth: 0-25 meters below sea level

Therefore we use those constants for our crab analysis. 
### Sea Surface Temperature
Sea surface temperature (SST) from the years 2008 to 2012 is used from [NOAA’s 5km Daily Global Satellite Sea Surface Temperature Anomaly v3.1.](https://coralreefwatch.noaa.gov/product/5km/index_5km_ssta.php)

Data files:

- average_annual_sst_2008.tif
- average_annual_sst_2009.tif
- average_annual_sst_2010.tif
- average_annual_sst_2011.tif
- average_annual_sst_2012.tif
### Bathymetry
To characterize the depth of the ocean we will use the [General Bathymetric Chart of the Oceans (GEBCO).](https://www.gebco.net/data_and_products/gridded_bathymetry_data/#area)

Data file: 
- depth.tif
### Exclusive Economic Zones
We will be designating maritime boundaries using Exclusive Economic Zones off of the west coast of US from [Marineregions.org.](https://www.marineregions.org/eez.php)

Data file: 
- wc_regions_clean.shp

## References
Suitable Conditions [SeaLifeBase](https://www.sealifebase.ca/search.php)

Sea Surface Temperature [NOAA’s 5km Daily Global Satellite Sea Surface Temperature Anomaly v3.1.](https://coralreefwatch.noaa.gov/product/5km/index_5km_ssta.php)

Exclusive Economic Zones [Marineregions.org.](https://www.marineregions.org/eez.php)

Bathymetry of the Ocean [General Bathymetric Chart of the Oceans (GEBCO).](https://www.gebco.net/data_and_products/gridded_bathymetry_data/#area)

- Hall, S. J., Delaporte, A., Phillips, M. J., Beveridge, M. & O’Keefe, M. Blue Frontiers: Managing the Environmental Costs of Aquaculture (The WorldFish Center, Penang, Malaysia, 2011).
- Gentry, R. R., Froehlich, H. E., Grimm, D., Kareiva, P., Parke, M., Rust, M., Gaines, S. D., & Halpern, B. S. Mapping the global potential for marine aquaculture. Nature Ecology & Evolution, 1, 1317-1324 (2017).
- GEBCO Compilation Group (2022) GEBCO_2022 Grid (doi:10.5285/e0f0bb80-ab44-2739-e053-6c86abc0289c).

Oliver, Ruth. Homework Assignment 4 - EDS 223- Prioritizing potential aquaculture (n.d.). https://eds-223-geospatial.github.io/assignments/HW4.html
