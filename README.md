# Geospatial Data Analysis - Visualizing Fire Scars Through False Color Imagery and Assessing Air Quality Using Python.

Author: Eva Newby (https://github.com/evajnewby)

## About

The following repository was created for edicational purposes for EDS 220 - Environmental Data, for the Masters of Environmental Data Science program at the Bren School of Environmental Science and Management at the University of California, Santa Barbara. 

The purpose of this repository is to hold both data and code necessary for the completion of the two maps and one plot, one showing a fire-perimeter for the 2017 Thomas fire and the other of a false-color image with the 2017 Thomas fire boundary laid ontop. The plot shows the Air Quality Index (AQI) 

This repository contains 3 jupyter notebooks, one named "fire-perimeter", one named "false-color", and the last named "air-quality-index", and a data folder. 

"fire-perimeter" contains the code necessary to filter California fire data to the 2017 Thomas fire, and save as a geoJSON.

"false-color" contains the code necessary to read in landsat data (using the rioxarray package). This notebook also contains the code and visualization outputs for a true color image, false color image, and a map of the 2017 Thomas fire boundary over the false color image. 

"air-quality-index" contains the code necessay to create a plot of AQI from 2017-2018, including the Thomas fire timeframe. 

The data folder contains the data California fire shapefile (along with .cpg, .dbf, .prj, and .shx), the Thomas fire geoJSON created in the "fire-perimeter" notebook, and the landsat8 imagery from the server. This folder was added to the gitignore to prevent any pushing issues or delays.

## Highlights
- Wrangling geospatial raster data using the `rioxarray` package
- Saving geospatial data as a GeoJSON
- Creating a true color image using the RGB (red, green, and blue) bands
- Creating a false color image by rearranging bands to incorporate near-infrared and short-wave-infrared
- Visualize the 2017 Thomas fire's effect on AQI

## Data
The landsat data is housed on the server, and was accessed using the provided file path (/courses/EDS220/data/hwk4_landsat_data landsat8-2018-01-26-sb-simplified.nc)

The California fires data was found online from the USGS, and contains fire data for all recent California fires, including the 2017 Thomas fire. The shapefile (and other associated files) were downloaded from USGS' website, and placed into the data folder. 

## Repository Structure
```bash
eds220-hwk4
├── README.md
├── .gitignore
     └── data
│        ├── California_Fire_Perimeters_(all).shp[1].xml
│        ├── California_Fire_Perimeters_(all)[1].cpg
│        ├── California_Fire_Perimeters_(all)[1].dbf
│        ├── California_Fire_Perimeters_(all)[1].prj
│        ├── California_Fire_Perimeters_(all)[1].shp
│        ├── California_Fire_Perimeters_(all)[1].shx
│        └── landsat8-2018-01-26-sb-simplified.nc
├── false-color.ipynb
├── fire-perimeter.ipynb
└── air-quality-index.ipynb
```
## References
Microsoft. Landsat C2 L2 dataset. Planetary Computer. Retrieved November 19, 2024, from https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2

U.S. Environmental Protection Agency. Outdoor air quality data. U.S. Environmental Protection Agency. Retrieved December 3, 2024, from https://www.epa.gov/outdoor-air-quality-data

U.S. Geological Survey (USGS). (2020). California Fire Perimeters (ALL). Data.gov. Retrieved November 19, 2024, from https://catalog.data.gov/dataset/california-fire-perimeters-all-b3436
