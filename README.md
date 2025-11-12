Sierra Leone - Solar Energy Data Analysis

This section covers the data cleaning and exploratory analysis of Sierra Leone’s solar performance dataset. The goal was to assess its potential for solar power generation relative to Benin and Togo.

Workflow Overview

Data Preparation

Loaded Sierra Leone’s dataset and inspected for missing or invalid entries.

Dropped the Comments column due to null values.

Set negative irradiance values (GHI, DNI, DHI) to zero and excluded zeros (nighttime).

Imputed cleaning values to preserve data balance.

Removed outliers using the IQR method for consistent analysis.

Exploratory Data Analysis (EDA)

Analyzed irradiance patterns across different hours of the day.

Compared module performance between clean and unclean readings.

Studied temperature (Tamb) variations alongside GHI trends.

Examined wind and precipitation data to identify environmental limitations.

Key Findings

Sierra Leone showed lower overall irradiance compared to Benin and Togo.

Data stability improved after filtering and outlier removal.

Higher rainfall and humidity may affect solar reliability and energy capture.

Wind speeds were generally mild, reducing structural concerns but limiting airflow cooling benefits.

Tools Used

Python libraries: pandas, numpy, matplotlib, seaborn, sweetviz, dataprep.eda

Git and GitHub for project version control

Visual Studio Code for development and data exploration
