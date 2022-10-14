# Data and code supplement for:

# "Harnessing hyperspectral imagery to map surface water presence and hyporheic flow properties of headwater stream networks"

[![DOI](https://zenodo.org/badge/545078848.svg)](https://zenodo.org/badge/latestdoi/545078848)

This repository contains data and code used to generate analyses for the publication. Contents of this directory are:

* Colab_notebooks: a directory of Jupyter notebooks written in Google Colab 

  * wetted_channel_random_forest_data_preparation: notebook used to prepare training data for random forest model to predict whether a stream reach is wet or dry from RapidEye satellite imagery bands. This notebook cannot be run without access to the RapidEye imagery.

  * wetted_channel_random_forest.ipynb: notebook training random forest model, exploring model accuracy, and producing model outcomes

  * wetted_channel_random_forest_results_exploration.ipynb: notebook exploring and developing models from random forest predictions

* Data: a directory containing supporting data for code

  * 2015_map_paths_R1.geojson: shapefile of areas walked during first boots-on-the-ground survey of the area
 
  * 2015_map_paths_R2.geojson: shapefile of areas walked during second boots-on-the-ground survey of the area
 
  * Streamchannels_R1_2015_NAME.geojson: shapefiles market channel reaches in different wetness states during the first survey at different named portions of the area
 
  * Streamchannels_R2_2015_NAME.geojson: shapefiles market channel reaches in different wetness states during the second survey at different named portions of the area
 
  * dry_runoff.csv: CSV file of runoff at the catchment outlet
 
  * geomorphic channel points 1085 with xy and flowaccum.csv: delineated nodes for random forest training and predictions generated along the geomorphic channel network
 
  * geomorphic_pts_newarea 2.csv: Correctly calculated slope and area for geomorphic points
 
  * highs_lows.pkl: pickle file containing data for confusion matrix based on logistic regression for surface water presence at each node
 
  * predict_data_x.csv: Set of CSV files that (combined) provide input data for random forest predictions
 
  * rf_predictions_x.csv: Set of CSV files that (combined) provide random forest predictions for each node and each date
 
  * training_data_x.csv: Set of CSV files that (combined) provide training data for random forest model
  
  * temporary_training_x.csv: Set of CSV files that (combined) provide initial training data that gets added to for final training data
 
