# Natural Disasters Data Analysis

## Team Members
- Andrew Lane
- Riley Laughlin
- Ivan Manzi
- Chris Prada

## Overview

This project analyzes natural disasters datasets, providing insights into the locations, frequency, and costs of such events. The project leverages pandas and data visualisations to show whether the frequency of natural disasters increase over time.

## Datasets
1. Geocoded Disasters (GDIS) Dataset, v1 (1960 – 2018). NASA Socioeconomic Data and Applications Center (SEDAC). Available at: [https://sedac.ciesin.columbia.edu/data/set/pend-gdis-1960-2018/data-download](https://sedac.ciesin.columbia.edu/data/set/pend-gdis-1960-2018/data-download)

    This dataset contains 39,953 locations for 9,924 global disasters from 1960 to 2018, including floods, storms, earthquakes, landslides, droughts, volcanic activity, and extreme temperatures.

2. U.S. Billion-dollar Weather and Climate Disasters, 1980 - present (NCEI Accession 0209268). National Centers for Environmental Information (NCEI), NOAA. Available at: [https://www.ncei.noaa.gov/access/metadata/landing-page/bin/iso?id=gov.noaa.nodc:0209268](https://www.ncei.noaa.gov/access/metadata/landing-page/bin/iso?id=gov.noaa.nodc:0209268)

    This dataset contains U.S. disaster cost assessments of the total, direct losses ($ in millions) inflicted by: tropical cyclones, inland floods, drought & heat waves, severe local storms, wildfires, crop freeze events, and winter storms.

### Key Tasks
- **Data Collection & Cleaning**: Converted datasets using `pandas`.
- **Summary Statistics**: Calculates mean, median, variance, standard deviation, and SEM of natural disasters.
- **Geoplots**: Generate geographical plots using `hvplots` using longitude and latitude data for first dataset
    - Heatmap of Impacted Regions: Grouped by disaster type and decade.
    - All Locations Affected by Natural Disasters: Grouped by disaster type and decade.
    
- **Linear Regression**: Generate scatter plots with regression line and equation to analyze:
    - Time vs. Number of Floods
    - Time vs. Number of Storms
    - Time vs. Number of Earthquakes
    - Time vs. Number of Volcanic Activities
- **Boxplot**: Displays the distribution of inflation adjusted cost across seven types of natural disaster (Flooding, Tropical Cyclone, Drought, Freeze, Severe Storm, Winter Storm, Wildfire), highlighting any outliers.

### Analysis
Based our analysis, we found:
- The frequency of natural disasters does increase over time. 
- There is no correlation between duration of a natural disaster and CPI-adjusted cost.


## Presentation
Slide deck is located in the repository for reference.

## Setup and Dependencies

Before starting, ensure you have the following libraries installed:

```python
# Dependencies
# !pip install jupyter_bokeh bokeh hvplot pandas matplotlib scipy citipy

import pandas as pd
import hvplot.pandas
import matplotlib.pyplot as plt
import scipy.stats as st
from citipy import citipys
```

## Running the Analysis
- Clone the repository and navigate to the project directory.
- Install dependencies as shown above.
- Run the Jupyter Notebook or Python script to generate the analysis and visualizations