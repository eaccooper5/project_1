# project_1
Group project for GW Bootcamp

# Project Name:
Fiscal Sustainability of Advanced and Emerging Economies

## Table of Contents
  - [Project Name](#Fiscal Sustainability of Advanced and Emerging Economies)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Prerequisites](#prerequisites)
  - [Getting Started](#getting-started)
  - [Usage](#usage)
  - [Contributing](#contributing)
  - [License](#license)
    
## Introduction
International Monetary Fund (IMF) Data Analysis Script Overview
This script retrieves economic indicators from the International Monetary Fund (IMF) Data API, analyzes the data, and generates visualizations for selected countries. The indicators include population growth, current account balance, government net lending/borrowing, government gross debt, unemployment rate, GDP per capita, government revenue and expenditure (% of GDP), gross public debt, real GDP growth rate, and household debt. 

## Setup and Configuration
The script uses the requests, json, pandas, time, matplotlib, numpy, and seaborn libraries. The following dictionaries and lists are defined for configuration:

## Prerequisites
​
- **Python:** Your project requires Python 3.7 or later. You can download it from [python.org](https://www.python.org/downloads/).
- **Jupyter Notebook:** For running and interacting with Jupyter Notebooks. You can install Jupyter using:
  #### ```bash
    pip install notebook
    pip install requests
    pip install pandas
    pip install seaborn
    pip install matplotlib
    pip install numpy
​
## Getting Started
git clone https://github.com/eaccooper5/project_1.git 
cd yourproject 
jupyter notebook

## Usage
### 1. Running the Jupyter Notebook: to run the Jupyter Notebook containing the project code
  #### ```bash
jupyter notebook
​
### 2. Running in Visual Studio Code (some worked using it)
Alternatively, you can use Visual Studio Code to work with the project. Open the project folder in VSCode and run the code cells interactively.
​
### 3. Explore Data and Visualizations
The project includes data analysis from IMF API and visualizations. Explore the data frames, charts, and graphs to gain insights into the selected economic indicators.
​
### 4. Modifying and Extending
Feel free to modify the code and experiment with different variables or data sources. Extend the analysis or add new visualizations based on your requirements.
​
### Examples
Here are a few examples of common tasks:
​
### Importing specific dataset from public API (and several ENDPOINTS) to collect specific data.
​
### Changing Variables:
Modify the notebook to analyze different economic indicators to filter the countries list into two groups based on the category.
​
### Custom Visualizations:
Experiment with creating custom visualizations using Seaborn and Matplotlib to convey specific insights.
​
### Comparative Analysis:
Conduct a comparative analysis between advanced and emerging economies, focusing on specific economic indicators.
COUNTRY_DATA: A mapping of country codes to country names.
ADV_COUNTRIES: A list of advanced countries.
EMER_COUNTRIES: A list of emerging countries.
INDICATORS: A dictionary mapping economic indicators to their corresponding IMF codes.
TIME_SPAN: A list of years for which data is collected.
BASE_URL: The base URL for the IMF API.

### Data Retrieval and Processing
The script iterates through the specified indicators, countries, and time periods, fetching the data from the IMF API. The retrieved data is then parsed into a Pandas DataFrame using the parseData and mergeDFs functions.

### Data Analysis
The script creates separate DataFrames for advanced and emerging economies. It then selects specific columns for analysis and visualization.

### Data Visualization
The script includes examples of data visualization using Matplotlib and Seaborn. It produces line plots illustrating national debt over time and the corresponding debt growth for advanced and emerging countries.

### Bar Plots
Bar plots are created for each indicator in both advanced and emerging economies, showing the values over the specified time span.

### Heatmaps
Heatmaps are generated to visualize the three indicators (population growth, unemployment rate, and national debt) for each country over the specified time span.

### Average Calculation and Pair Plots
Average values for each indicator are calculated for both advanced and emerging economies. Pair plots are created to visualize the relationships between the indicators for each country.

### File Outputs
Bar plot images for advanced and emerging economies are saved as 'bar_plots_adv.png', 'bar_plots_emer.png', 'bar_plots_advLP.png', and 'bar_plots_emerLP.png'.
Heatmap images for advanced and emerging economies are displayed but not saved.
The script prints average values for each indicator for both advanced and emerging economies.

## Contributing 
Thank you for considering contributing to this project! Contributions are welcomed and encouraged.

### Note
The NaN values in the output indicate missing data.
