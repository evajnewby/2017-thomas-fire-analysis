# Geospatial Data Analysis - Visualizing Fire Scars Through False Color Imagery Using Python.

Author: Eva Newby (https://github.com/evajnewby)

This repository contains 2 jupyter notebooks, one named "fire-perimeter" and the other named "false-color" and a data folder. 

"fire-perimeter" contains the code necessary to filter California fire data to the 2017 Thomas fire, and save as a geoJSON.

'false-color' contains the code necessary to read in landsat data (using the rioxarray package). This notebook also contains the code and visualization outputs for a true color image, false color image, and a map of the 2017 Thomas fire boundary over the false color image. 

The data folder contains the data California fire shapefile (along with .cpg, .dbf, .prj, and .shx), the Thomas fire geoJSON created in the "fire-perimeter" notebook, and the landsat8 imagery from the server. This folder was added to the gitignore to prevent any pushing issues or delays. 

## Data
The landsat data is housed on the server, and was accessed using the provided file path (/courses/EDS220/data/hwk4_landsat_data landsat8-2018-01-26-sb-simplified.nc)

The California fires data was found online from the USGS, and contains fire data for all recent California fires, including the 2017 Thomas fire. The shapefile (and other associated files) were downloaded from USGS' website, and placed into the data folder. 

## Repository Structure
├── LICENSE
├── README.md
├── data
│   ├── California_Fire_Perimeters_(all).shp[1].xml
│   ├── California_Fire_Perimeters_(all)[1].cpg
│   ├── California_Fire_Perimeters_(all)[1].dbf
│   ├── California_Fire_Perimeters_(all)[1].prj
│   ├── California_Fire_Perimeters_(all)[1].shp
│   ├── California_Fire_Perimeters_(all)[1].shx
│   └── landsat8-2018-01-26-sb-simplified.nc
├── .ipynb
└──

## Sources
Microsoft. (n.d.). Landsat C2 L2 dataset. Planetary Computer. Retrieved November 19, 2024, from https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2

U.S. Geological Survey (USGS). (2020). California Fire Perimeters (ALL). Data.gov. Retrieved November 19, 2024, from https://catalog.data.gov/dataset/california-fire-perimeters-all-b3436