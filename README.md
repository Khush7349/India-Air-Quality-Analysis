# India-Air-Quality-Analysis
End-to-end analysis of Indian air pollution data, featuring time-series analysis, data cleaning, and visualization with Python.

# Analysis of Air Quality in Major Indian Cities

### Overview

This project conducts a comprehensive analysis of air quality across various cities in India using a time-series dataset spanning from 2016 to 2023. The objective was to perform an end-to-end data science project, including data cleaning, exploratory analysis, statistical modeling, and visualization. The entire analysis was performed in Python within a Kaggle Notebook environment.

### Project Goals

* To clean and prepare a large, multi-file time-series dataset for analysis.
* To identify the most and least polluted cities from a sample of 30+ monitoring stations.
* To analyze and compare the seasonal patterns of various pollutants.
* To understand the relationships between different pollutants and local weather conditions using correlation analysis.
* To visualize the key findings in a series of summary dashboards.

### Dataset

The data used in this project is the "Air Quality Data in India (2010-2023)" dataset, available on Kaggle. It contains hourly readings from hundreds of monitoring stations across the country.

[Link to the Dataset on Kaggle](https://www.kaggle.com/datasets/abhisheksjha/time-series-air-quality-data-of-india-2010-2023)

### Analysis Pipeline

The project followed these key steps:
1.  Data Loading & Environment Setup: Utilized a Kaggle Notebook to efficiently handle the large, multi-file dataset.
2.  Data Cleaning & Preprocessing: Parsed date/time columns into the correct `datetime` format. Handled missing values using linear interpolation, a suitable method for time-series data.
3.  Exploratory Data Analysis (EDA): Performed initial analysis and visualization on a single station to understand the data structure.
4.  Scaled Analysis: Developed an automated loop to process and clean data from over 30 stations, combining them into a master DataFrame.
5.  Comparative Analysis:
    * Created a ranked "leaderboard" of stations based on average PM2.5 levels.
    * Generated correlation heatmaps to compare the pollution dynamics between high and low-pollution cities.
6.  Time-Series Decomposition: Used `statsmodels` to separate a city's pollution data into its underlying trend, seasonal, and residual components.
7.  Dashboard Creation: Visualized the final insights using Matplotlib and Seaborn to create summary dashboards.

### Key Findings

* Geographical Disparity: A significant difference in air quality exists across India, with stations in northern states like Bihar and Delhi consistently showing much higher pollution levels than stations in southern states.
* Strong Seasonality: All cities exhibit a strong seasonal pattern, with pollution levels peaking during the winter months and decreasing significantly during the monsoon season.
* Pollutant Correlations: Highly polluted cities show a strong correlation between combustion-related pollutants (PM2.5, PM10, CO), indicating traffic and industrial activity as primary drivers.
* Long-Term Trends: Time-series decomposition revealed the underlying long-term pollution trend for specific cities, separate from the seasonal effects.

### Tools and Libraries

* Language: Python
* Libraries: Pandas, Matplotlib, Seaborn, Statsmodels
* Environment: Kaggle Notebooks
