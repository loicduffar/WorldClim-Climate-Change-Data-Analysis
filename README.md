# WorldClim - Climate Change Data Analysis
Historical &amp; future climatologies (1970-2100) - Maps plotting and time series extraction

## MAPS

- Data: https://www.worldclim.org/data/index.html
- author: Loïc Duffar https://github.com/loicduffar

This python notebook uses data from the wordclim web site to plot future climatologies maps on a given area. The outpus are stored as image files (png) and raster files (geotif).

How to PROCEED ?

The data files must be divided into different sub-folders:

- a folder containing the 12 tif files with historical monthly interannual averages (1 file per month of the year)
- a folder with sub-folders for the various future periods (e.g. 1921-1940, 1961-1981, 1981-2100). Each subfolder contains 4 tif files for each model (and each file contains 12 bands for the the different months).
- Optionnaly, the global DEM file can be downloaded from WorldClim to plot the elevation map of the area

Run the first script, then one of the following ones:

1) Customization
2) Plot maps for one scenario, one period & one model (12 months and annual)
3) Generate a bunch of maps of all scenarios/periods/models (annual maps in png files)
4) Plot the elevation map

### GRAPHS

4 SSP scenarios and 9 Global Climatic Models

- Data: https://www.worldclim.org/data/index.html
- author: Loïc Duffar https://github.com/loicduffar

This python notebook uses data from the wordclim web site to compute the evolution of future precipitation on a given watershed (average of the pixels inside the polygon). The ouputs are stored in an excel file.

How to PROCEED ?

The data files must be divided into different sub-folders:

- a folder containing the 12 tif files of historical monthly interannual averages (1 file per month of the year)
- a folder with 4 sub-folders for the various future periods (1921-1940, 1961-1981, 1981-2100). Each folder contains 4 tif files for each model (and each file contains 12 bands for the the different months).

Then run cells in order:

1) Historical interannual monthly mean 1970-2000
2) Future precipitations
3) Multi index by Model, Scenario and Period
4) Concatenate historical and future precipitation in a single dataframe
5) Plot annual evolution of annual precipitation in future, according to all SSP scenarios and all GCM
6) Plot future evolution for each month, according to 4 SSP scenarios and 9 GCMs
7) Store statistics in a dataframe
8) Plot montly projections (all SSP scenarios and GCMs)
9) Store all outputs in an excel file
