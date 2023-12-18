# project_1
Group project for GW Bootcamp

International Monetary Fund (IMF) Data Analysis Script
Overview

Background
This script retrieves economic indicators from the International Monetary Fund (IMF) Data API, analyzes the data, and generates visualizations for selected countries. The indicators include population growth, current account balance, government net lending/borrowing, government gross debt, unemployment rate, GDP per capita, government revenue and expenditure (% of GDP), gross public debt, real GDP growth rate, and household debt. 

Setup and Configuration
The script uses the requests, json, pandas, time, matplotlib, numpy, and seaborn libraries. The following dictionaries and lists are defined for configuration:

COUNTRY_DATA: A mapping of country codes to country names.
ADV_COUNTRIES: A list of advanced countries.
EMER_COUNTRIES: A list of emerging countries.
INDICATORS: A dictionary mapping economic indicators to their corresponding IMF codes.
TIME_SPAN: A list of years for which data is collected.
BASE_URL: The base URL for the IMF API.

Data Retrieval and Processing
The script iterates through the specified indicators, countries, and time periods, fetching the data from the IMF API. The retrieved data is then parsed into a Pandas DataFrame using the parseData and mergeDFs functions.

Data Analysis
The script creates separate DataFrames for advanced and emerging economies. It then selects specific columns for analysis and visualization.

Data Visualization
The script includes examples of data visualization using Matplotlib and Seaborn. It produces line plots illustrating national debt over time and the corresponding debt growth for advanced and emerging countries.

Bar Plots
Bar plots are created for each indicator in both advanced and emerging economies, showing the values over the specified time span.

Heatmaps
Heatmaps are generated to visualize the three indicators (population growth, unemployment rate, and national debt) for each country over the specified time span.

Average Calculation and Pair Plots
Average values for each indicator are calculated for both advanced and emerging economies. Pair plots are created to visualize the relationships between the indicators for each country.

File Outputs
Bar plot images for advanced and emerging economies are saved as 'bar_plots_adv.png', 'bar_plots_emer.png', 'bar_plots_advLP.png', and 'bar_plots_emerLP.png'.
Heatmap images for advanced and emerging economies are displayed but not saved.
The script prints average values for each indicator for both advanced and emerging economies.


Note
The NaN values in the output indicate missing data.
