# PWWB-Mexico_City

Code for the Predict What We Breathe project. In this repository, we provide the code to run our GCN-ConvLSTM architecture to predict hourly PM2.5 spatially continuously in the Mexico City area. 

# Overview

We utilize remote-sensing satellite imagery and ground-based sensor data to predict hourly PM2.5 in a 5625 square kilometer area of Mexico City. We utilize remote-sensing wildfire imagery from the NASA MERRA-2 and MODIS products, satellite imagery of atmospheric air pollutants (NO2, PM2.5, O3, CO) from the ESA Sentinel-2 TROPOMI instrument, satellite imagery of aerosol optical depth (AOD) from the NASA MAIAC product, meteorological features from ground-based sites, and ground-level air pollution (PM2.5, PM10, NO2, SO2, CO, and O3) from ground-based sites. 

# Repository Structure

```MexicoCityGridPred.ipynb``` is the main code file. This Jupyter notebook contains the raw code and documentation of our preprocessing, training, prediction, and visualization pipeline. 

```sitelist.csv``` is a reference table of the ground-level meteorological and air pollution sensors, their latitude and longitude coordinates, and their corresponding (x,y) coordinates within the 75x75 geographical grid we construct. 

```Images``` contains various supporting description images used in the Jupyter notebook.

```Supporting Files``` contains various supporting files needed to run our Jupyter notebook.

```GeoTiff Predictions``` contains some example hourly predictions for Mexico City. We provide 168 hourly predictions for 1 week of our testing cohort (January 1 2021 - January 7 2021) over a 75km x 75km area of Mexico City with a spatial resolution of 1 pixel per square kilometer.

# Installation Instructions

To run our code, clone this repository and ensure all supporting files are within the same hierarchy structure of the Jupyter Notebook file. We also save several larger files including the raw dataset files externally, as it exceeds the Github storage limit. Ensure that these dataset files are also downloaded and included within the same directory as the Jupyter notebook.

