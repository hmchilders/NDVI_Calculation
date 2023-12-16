# Calculation of the Normalized Difference Vegetation Index

## Overview

Monitoring the distribution and change in land cover types can help us understand the impacts of phenomena like climate change, natural disasters, deforestation, and urbanization. Determining land cover types over large areas is a major application of remote sensing because we are able to distinguish different materials based on their spectral reflectance.

Classifying remotely sensed imagery into landcover classes enables us to understand the distribution and change in landcover types over large areas. There are many approaches for performing landcover classification -- *supervised* approaches use training data labeled by the user, whereas *unsupervised* approaches use algorithms to create groups which are identified by the user afterward.

# Objective

In this repository, we are using a form of supervised classification, a *decision tree classifier*. [Decision trees](https://medium.com/@ml.at.berkeley/machine-learning-crash-course-part-5-decision-trees-and-ensemble-models-dcc5a36af8cd) classify pixels using a series of conditions based on values in spectral bands. These conditions (or decisions) are developed based on training data. In this lab we will create a land cover classification for southern Santa Barbara County based on multi-spectral imagery and data on the location of 4 land cover types:

-   green vegetation
-   dry grass or soil
-   urban
-   water

### Skills used in this Repo:

-   load and process Landsat scene
-   crop and mask Landsat data to study area
-   extract spectral data at training sites
-   train and apply decision tree classifier
-   plot results

```
Houston Blackouts
│   README.md
│   Rmd/Proj files    
│
└───data
    │   sb_county_south files
    │   sb_validation_points files
    |   trainingdata files
    │
    └───landsat-data
    |   │   .tiff files
```