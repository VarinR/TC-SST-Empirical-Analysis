# Investigating the Impact of Sea Surface Temperature Anomalies on Tropical Cyclone Frequency: Using An Empirical Approach

This research project was conducted under the mentorship of Dr.Travis O'Brien.


## Table of Contents

1. [Project Goal](#Project-Goal)
2. [Notebooks Overview](#Notebooks-Overview)
    - [Visualise-SSTs.ipynb](#Visualise-SSTs.ipynb)
    - [Preparing-TCdata.ipynb](#Preparing-TCdata.ipynb)
    - [VisualisingTC&SST.ipynb](#VisualisingTC&SST.ipynb)
    - [TCstarts-BinnedAnalysis.ipynb](#TCstarts-BinnedAnalysis.ipynb)
    - [Conditional-Probability.ipynb](#Conditional-Probability.ipynb)


## Project Goal

The primary goal of this research project is to investigate the relationship between higher local SSTs and the probability of TCs. This will be achieved by analyzing SST data, identifying regions with higher-than-average SSTs, and examining the correlation with tropical cyclone occurrences. Additionally, I created a conditional probability model to better understand this relationship.

## Notebooks Overview

### Visualise-SSTs.ipynb

#### Objectives

- To analyze SST data within the tropics, focusing on trends since 1971.
- Identify regions with local SSTs greater than tropical mean (SST anamoly).

#### Key Findings

- **Historical SST Trends:** A clear upward trend in mean yearly SSTs in the tropics over the last fifty years was identified, highlighting a consistent increase in sea surface temperatures which sets a premise for further research into its effects on TC activity.
- **Regions with Elevated SSTs:** Visual analysis pinpointed specific regions where SSTs exceed the Tropical mean. These areas are of particular interest for investigating their contribution to an increased likelihood of TC genesis.


### Preparing-TCdata.ipynb

#### Objectives

- **Data Preparation:** The goal of this notebook is to prepare raw TC data for further analysis
- **Yearly Storm ID Extraction:** Implement a function to extract and organize storm ID data from the TC dataset annually, facilitating analysis on cyclone activity over time.
- **Data Structuring:** Create a dictionary associating storm IDs with their corresponding year of occurrence.
- **Computational Efficiency:** Serialize the structured tropical cyclone data into a pickle file, optimizing data storage and retrieval processes to enhance computational efficiency.
  

### VisualisingTC&SST.ipynb

#### Objectives

- **Data visualisation:** Visualise the relation between masked SSTs and Tropical Cyclones.
- **Yearly masked SST Extraction :** Implemented a loop to iterate over each year in the tropical data, extracting and storing masked SST data where temperatures exceed the yearly tropical mean.
- **Storm lat and lon Extraction :** Implemented a loop to systematically extract and organize latitude and longitude data for each storm, sorted annually.
- **Geospatial visualisation of SST and TCs:** Implemented a visualization loop to create a series of subplots, each representing a year from 1971 to 2022. For each subplot, the code plots the paths of TCs based on their latitude and longitude data, overlaying this with masked SST data to illustrate the correlation between SST anomalies and cyclone activity for a particular year.

#### Key Findings

- **Plot analysis:** Most tropical cyclones do form in areas with higher than average SSTs, especially in the Western North Pacific and Eastern Indian Ocean. The North Atlantic is an exception, where higher SSTs don't always correlate with cyclone formation.


### TCstarts-BinnedAnalysis.ipynb

#### Objectives

- **TC Genesis and SST Relationship:** Investigate the correlation between delta SSTs and the frequency of TC genesis, focusing on identifying SST ranges that exhibit increased cyclone activity.
- **Tropical Grid Box Analysis:** The tropics are divided into 5° x 5° grid boxes, where average SSTs exceeding the tropical mean are identified, and the number of TCs commencing within these.
- **SST Binning and TC Start Analysis:** Defined SST bins between -1°C to 4°C with increments of 0.2°C. Calculated the midpoints of these bins, and initialized an array to count TC starts within each bin. Processed annual data to aggregate the number of TC starts per SST bin, which was then visualized to illustrate the relationship between SSTs and TC initiation frequency.

#### Key Findings

- **Optimal SST Range for TC Genesis:** The SST range from 1°C to 2°C is identified as most conducive to TC formation, with a pronounced peak in TC starts observed within this interval.
- **Variability Beyond SST:** While SST is a significant factor in TC formation, suggesting additional atmospheric factors are at play in TC genesis.
- **Declining TC Formation in Higher SSTs:** The decline in TC starts at SSTs beyond the optimal range suggests where exceedingly high temperatures do not favor the development of TC.


### Conditional-Probability_model.ipynb

#### Objectives

- **TC Genesis and SST Relationship:** Investigate the correlation between delta SSTs and the frequency of TC genesis, focusing on identifying SST ranges that exhibit increased cyclone activity.
- **Tropical Grid Box Analysis:** The tropics are divided into 5° x 5° grid boxes, where average SSTs exceeding the tropical mean are identified, and the number of TCs commencing within these.
- **SST Binning and TC Start Analysis:** Defined SST bins between -1°C to 4°C with increments of 0.2°C. Calculated the midpoints of these bins, and initialized an array to count TC starts within each bin. Processed annual data to aggregate the number of TC starts per SST bin, which was then visualized to illustrate the relationship between SSTs and TC initiation frequency.

#### Key Findings

- **Optimal SST Range for TC Genesis:** The SST range from 1°C to 2°C is identified as most conducive to TC formation, with a pronounced peak in TC starts observed within this interval.
- **Variability Beyond SST:** While SST is a significant factor in TC formation, suggesting additional atmospheric factors are at play in TC genesis.
- **Declining TC Formation in Higher SSTs:** The decline in TC starts at SSTs beyond the optimal range suggests where exceedingly high temperatures do not favor the development of TC.












.




