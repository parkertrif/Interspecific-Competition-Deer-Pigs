# Interspecific-Competition-Deer-Pigs

## Overview

This repository contains the data and code for analyzing temporal overlap and activity patterns among white-tailed deer (*Odocoileus virginianus*), wild pigs (*Sus scrofa*), and coyotes (*Canis latrans*). The analysis examines how the presence of wild pigs affects temporal activity patterns of white-tailed deer and their overlap with coyotes using camera trap data from July - August 2024 in eastern Texas.

## Repository Structure
```
├── data/
│   ├── bait_site_deer_pig.csv
│   └── grid_camera.csv
├── scripts/
│   └── temporal_analysis.R
└── README.md
```

## Data Description

### bait_site_deer_pig.csv

Camera trap detections from bait sites containing deer and pig observations. Used to assess foraging activity patterns.

**Columns:**

- `placename`: Unique site identifier
- `species`: Species detected
- `pig_present_at_site`: Binary indicator of whether pigs had been previously detected at that site 
- `radtime`: Detection time in radians

### grid_camera.csv

Camera trap detections from passive grid cameras. Used for diel temporal overlap analysis.

**Columns:**

- `placename`: Unique site identifier
- `species`: Species detected 
- `radtime`: Detection time in radians

## Requirements

### R Version

R version >= 4.0.0

### R Packages
```r
library(overlap)      # Temporal overlap analysis
library(gridExtra)    # Plot arrangement
library(tidyverse)    # Data manipulation and visualization
```
## Reproducibility & Publishing

This repository is prepared to be published on Dryad alongside the associated manuscript. It contains all data and code needed to reproduce key results, following best practices for reproducible open science.

