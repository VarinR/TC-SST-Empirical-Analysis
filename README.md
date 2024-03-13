# Atmospheric Science Research Project 2

This repository contains an independent research project conducted under the mentorship of Dr. Travis O'Brien over Spring 24 semester, focusing on the relationship between higher local sea surface temperatures and increased probability of tropical cyclones, using data analysis 


## Table of Contents

1. [Project Goal](#Project-Goal)
2. [Notebooks Overview](#Notebooks-Overview)
    - [First Notebook (SSTs1.ipynb)](#First-Notebook-(SSTs1.ipynb))
    - [Second Notebook (SSTs2.ipynb)](#Second-Notebook-(SSTs2.ipynb))
    - [Third Notebook (SSTs3.ipynb)](#Third-Notebook-(SSTs3.ipynb))
    - [Fourth Notebook (SSTs4.ipynb)](#Fourth-Notebook-(SSTs4.ipynb))


## Project Goal

The primary goal of this research project is to investigate the relationship between higher local sea surface temperatures (SSTs) and the probability and intensity of tropical cyclones, by analyzing SST data, identifying regions with higher than average SSTs, and examining the correlation with tropical cyclone (TC) occurrences to better understand the impact of climate change on these weather events.

## Notebooks Overview


### First Notebook (SSTs1.ipynb)

#### Objectives

- To analyze SST data within the tropics, focusing on trends since 1971.
- Identify regions with local SSTs greater than tropical mean.

#### Key Findings

- **Historical SST Trends:** A clear upward trend in mean yearly SSTs in the tropics over the last fifty years was identified, highlighting a consistent increase in sea surface temperatures which sets a premise for further research into its effects on TC activity.
- **Regions with Elevated SSTs:** Visual analysis pinpointed specific regions where SSTs exceed the Tropical mean. These areas are of particular interest for investigating their contribution to an increased likelihood of TC genesis.


### Second Notebook (SSTs2.ipynb)

#### Objectives

- **Data Preparation:** The goal of this notebook is to prepare raw TC data for further analysis
- **Yearly Storm ID Extraction:** Implement a function to extract and organize storm ID data from the TC dataset annually, facilitating analysis on cyclone activity over time.
- **Data Structuring:** Create a dictionary associating storm IDs with their corresponding year of occurrence.
- **Computational Efficiency:** Serialize the structured tropical cyclone data into a pickle file, optimizing data storage and retrieval processes to enhance computational efficiency.
  

### Third Notebook (SSTs3.ipynb)

#### Objectives

- **Data visualisation:** Visualise the relation between masked SSTs and Tropical Cyclones.
- **Yearly masked SST Extraction :** Implemented a loop to iterate over each year in the tropical data, extracting and storing masked SST data where temperatures exceed the yearly tropical mean.
- **Storm lat and lon Extraction :** Implemented a loop to systematically extract and organize latitude and longitude data for each storm, sorted annually.
- **Geospatial visualisation of SST and TCs:** Implemented a visualization loop to create a series of subplots, each representing a year from 1971 to 2022. For each subplot, the code plots the paths of TCs based on their latitude and longitude data, overlaying this with masked SST data to illustrate the correlation between SST anomalies and cyclone activity.

#### Key Findings

- **Plot analysis:** Most tropical cyclones do form in areas with higher than average SSTs, especially in the Western North Pacific and Eastern Indian Ocean. The North Atlantic is an exception, where higher SSTs don't always correlate with cyclone formation.


### Fourth Notebook (SSTs4.ipynb)

#### Objectives

- **TC Genesis and SST Relationship:** Investigate the correlation between SSTs and the frequency of TC genesis, focusing on identifying SST ranges that exhibit increased cyclone activity.
- **Tropical Grid Box Analysis:** The tropics are divided into 5° x 5° grid boxes, where average SSTs exceeding the tropical mean are identified, and the number of TCs commencing within these.
- **SST Binning and TC Start Analysis:** Defined SST bins between 26°C to 32°C with increments of 0.5°C. Calculated the midpoints of these bins, and initialized an array to count TC starts within each bin. Processed annual data to aggregate the number of TC starts per SST bin, which was then visualized to illustrate the relationship between SSTs and TC initiation frequency.

#### Key Findings

- **Optimal SST Range for TC Genesis:** The SST range from 27°C to 29°C is identified as most conducive to TC formation, with a pronounced peak in TC starts observed within this interval.
- **Variability Beyond SST:** While SST is a significant factor in TC formation, the data reveal variability and the presence of outliers, suggesting additional atmospheric factors are at play in cyclone genesis.
- **Declining TC Formation in Higher SSTs:** The decline in TC starts at SSTs beyond the optimal range suggests a complex relationship between SST and TC genesis, where exceedingly high temperatures do not favor the development of TC.












.




