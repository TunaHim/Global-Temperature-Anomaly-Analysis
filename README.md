# Global-Temperature-Anomaly-Analysis

## Geospatial data analysis using Xarray, Dask, NetCDF4 and Geopandas

### Description
This repository contains a Jupyter notebook serving as a project template for analyzing climate data using Xarray, Dask, and GeoPandas. The project involves loading climate data from a NetCDF file, performing various operations, calculating climatologies, and visualizing the results on maps. It also demonstrates the use of Dask for parallel computing to handle large datasets efficiently.

### Dependencies
-	xarray: A library for working with labeled multi-dimensional arrays.
- dask: A parallel computing library that integrates seamlessly with Xarray to scale computations.
-	geopandas: An extension of Pandas that provides support for geographic data types and operations.
-	netCDF4: A Python interface to the NetCDF file format for scientific data.

### Data Source & files
The climate data used in this project is sourced from the GISS Surface Temperature Analysis (GISTEMP) dataset provided by the National Aeronautics and Space Administration (NASA). The dataset contains monthly surface air temperature anomalies on a global grid with a spatial resolution of 2°x2° and covers the period from 1991 to 2020. The data can be downloaded from the NOAA Physical Sciences Laboratory. One can download the necessary files from this source. Links: https://psl.noaa.gov/data/gridded/data.gistemp.html https://downloads.psl.noaa.gov/Datasets/gistemp/combined/1200km/. 

Additionally, the data file is also available in the repository. 

### Workflow Steps
1.	Mount Google Drive (Google Colab): If using Google Colab, mount Google Drive to access the dataset folder. Alternatively, if working in a local environment, skip this step and load the NetCDF file directly from the local file system.
2.	Install Dependencies: Install necessary dependencies using pip. This step is required in both Google Colab and local environments.
3.	Load NetCDF File: Load the NetCDF file containing climate data into an xarray Dataset. If not using Google Colab, provide the path to the local file system instead.
4.	Check Dataset: Inspect the dimensions, variables, units, and metadata of the dataset.
5.	Extract Necessary Variables: Extract necessary variables such as latitude, longitude, and air temperature anomaly.
6.	Perform Operations Using Dask: Convert variables to Dask arrays for lazy loading and perform parallel computing tasks.
7.	Plotting: Visualize the data on maps using Cartopy and GeoPandas.
8.	Compute Climatology: Calculate the climatology (mean over all timestamps) and plot the results.
9.	Compare Computational Time: Compare the time taken for computations with and without Dask operations.
10.	Save Climatology Data: Save the computed climatology variable to a NetCDF file.

### Usage
1.	Clone the repository: git clone https://github.com/TunaHim/Global-Temperature-Anomaly-Analysis
2.	Open the Jupyter notebook global_temperature_analysis.ipynb in your preferred environment.
3.	Follow the instructions in the notebook to analyze climate data and visualize the results.

### Contributors
-	Himansu K Pradhan
