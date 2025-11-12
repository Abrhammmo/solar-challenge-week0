# Benin - Solar Energy Data Analysis

This section covers the data cleaning and exploratory data analysis (EDA) performed on Benin’s solar performance dataset as part of the Solar Challenge Week 0 project. The goal was to evaluate Benin’s potential for solar investment based on irradiance and environmental factors.

---

## Workflow Overview

1. **Data Preparation**

   * Loaded the Benin dataset and checked for missing or invalid values.
   * Removed the `Comments` column since it contained only null values.
   * Replaced negative irradiance values (GHI, DNI, DHI) with zero.
   * Filtered out nighttime readings where irradiance was zero.
   * Imputed missing cleaning values instead of dropping them entirely.
   * Removed outliers using the Interquartile Range (IQR) method.

2. **Exploratory Data Analysis (EDA)**

   * Converted timestamps and extracted hourly and daily trends.
   * Analyzed irradiance variables (GHI, DNI, DHI) and their distributions.
   * Compared irradiance during cleaning and non-cleaning periods.
   * Investigated the relationship between ambient temperature (Tamb) and GHI.
   * Examined how wind speed (WS), gust (WSgust), and precipitation affected solar performance.

3. **Key Findings**

   * Benin recorded high average GHI and DNI values, indicating strong solar potential.
   * Clean modules produced more stable and accurate irradiance readings.
   * Moderate wind and low precipitation make Benin suitable for solar panel installation.
   * Outlier removal confirmed data consistency and reliability.

4. **Tools Used**

   * Python libraries: pandas, numpy, matplotlib, seaborn, sweetviz, dataprep.eda
   * Git and GitHub for version control
   * Visual Studio Code as the main development environment

---

## Next Steps

Benin’s cleaned and summarized data will be compared against Togo and Sierra Leone using a weighted scoring model to determine the best country for solar panel investment.

