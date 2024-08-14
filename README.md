# Chicago Crime Data Analysis and Forecasting
This project focuses on analyzing and predicting crime trends in Chicago using historical crime data from 2001 to the present (2024). The dataset is sourced from Kaggle and provides comprehensive information on various types of crimes committed in Chicago. The analysis aims to identify patterns, visualize crime data, and forecast future crime trends using the Facebook's Prophet model.

  

## Table of Contents

- [Dataset](#dataset)

- [Installation](#installation)

- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)

- [Data Visualization](#data-visualization)

- [Forecasting with Prophet](#forecasting-with-prophet)

- [Images](#images)

- [Conclusion](#conclusion)

  

## Dataset

The dataset used in this project is sourced from [Kaggle](https://www.kaggle.com/datasets/adelanseur/crimes-2001-to-present-chicago). It contains detailed information on crimes committed in Chicago, including the type of crime, location, date, and other relevant attributes.

  

## Installation

To run this project, you will need to have Python installed along with the following libraries:

  

- numpy

- pandas

- seaborn

- matplotlib

- Prophet

  

You can install the required libraries using pip:

  

```bash

pip  install  numpy  pandas  seaborn  matplotlib  prophet

```

  

## Exploratory Data Analysis (EDA)

The project begins by importing the dataset into a pandas DataFrame and performing an initial inspection using `head()` and `tail()` functions to get a sense of the data. Missing data is visualized using a heatmap, and unnecessary columns are dropped to streamline the dataset.

  

Key steps in EDA include:

- Converting the `Date` column to a datetime format to facilitate time-series analysis.

- Analyzing the frequency of different crime types and visualizing the top 15 crime types.

- Examining crime occurrences in different locations within Chicago and identifying areas with high crime rates.

  

## Data Visualization

Several visualizations are created to gain insights into the crime data:

- A count plot of the different crime types to see which are most prevalent.

- A count plot of crimes by location description to identify hotspots.

- A line plot showing the total number of crimes per year, helping to observe trends over time.

- Monthly and quarterly crime counts are visualized to understand seasonality and other periodic patterns in the data.

  

## Forecasting with Prophet

The project utilizes the Prophet model, a time-series forecasting tool, to predict future crime rates. The data is resampled to a monthly frequency, and the `Date` and `Crime Count` columns are renamed to `ds` and `y`, respectively, to comply with Prophet's requirements.

  

Key steps in forecasting:

- Fitting the Prophet model to the historical data.

- Making predictions for the next two years (720 days).

- Visualizing the forecast and its components to understand the trend, seasonal patterns, and other factors influencing crime rates.


## Images

Snapshots of visualizations from the notebook                
:-------------------------:
![visualization the different types of crimes and their count](/Images/01.png)     
:-------------------------:
![visualization the count of crimes in the top locations that are prone to high crime rate](/Images/02.png)  
:-------------------------:
![crime count per year](/Images/03.png)  
:-------------------------:
![predicted trend](/Images/04.png)  

## Conclusion

This project provides a comprehensive analysis of Chicago's crime data and demonstrates how machine learning models like Prophet can be used to forecast future trends. The visualizations and predictions can help policymakers and law enforcement agencies to allocate resources more effectively and develop strategies to reduce crime in Chicago.

  

---

  

*Author: Vedanta Banerjee | Date: 14.08.2024*