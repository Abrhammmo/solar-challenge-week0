## Sierra Leone Solar Energy Data Analysis: Assessing Investment Potential

This document summarizes the **Data Preparation** and **Exploratory Data Analysis (EDA)** performed on Sierra Leone's solar performance dataset. The analysis aimed to assess Sierra Leone's potential for **solar power generation** relative to regional comparators, **Benin and Togo**.

***

### Workflow Overview

The analysis followed a standard two-phase workflow, ensuring data quality before deriving insights:

#### Data Preparation (Cleaning and Pre-processing)

The dataset was prepared for analysis through the following steps:

* **Loading and Inspection:** The Sierra Leone dataset was loaded and checked for **missing or invalid entries**.
* **Column Removal:** The `Comments` column was **dropped** due to containing only null values.
* **Irradiance Correction:** Negative irradiance values (Global Horizontal Irradiance **GHI**, Direct Normal Irradiance **DNI**, Diffuse Horizontal Irradiance **DHI**) were set to **zero**. Nighttime readings (irradiance = 0) were then **excluded**.
* **Imputation:** Missing module **cleaning status** values were imputed to ensure data balance for comparative analysis.
* **Outlier Removal:** **Outliers** were removed using the **Interquartile Range (IQR) method** to maintain consistency and robust analysis.

#### Exploratory Data Analysis (EDA)

Key variables were analyzed to understand their impact on solar performance:

* **Irradiance Patterns:** Irradiance trends were analyzed across different **hours of the day** to identify peak generation times.
* **Module Performance Comparison:** Module performance was compared between **clean and unclean readings** to quantify the effect of soiling.
* **Temperature Analysis:** Temperature variations (Ambient Temperature, $T_{amb}$) were studied alongside **GHI trends** to assess thermal efficiency impacts.
* **Environmental Factors:** Wind speed, wind gust, and **precipitation data** were examined to identify potential environmental limitations on operations and reliability.

***

### Key Findings

The exploratory analysis revealed important characteristics of the solar environment in Sierra Leone:

* **Lower Irradiance:** Sierra Leone showed **lower overall irradiance** levels compared to the regional comparators, Benin and Togo.
* **Data Stability:** The consistency and reliability of the data for analysis **improved significantly** after initial filtering and outlier removal.
* **Climate Impact:** **Higher rainfall and humidity** levels were noted, which may negatively affect solar reliability and energy capture due to increased cloud cover and soiling.
* **Wind Conditions:** Wind speeds were generally **mild**, which reduces structural concerns for installations but also limits the beneficial **airflow cooling** effect on solar panels.

***

### Tools Used

The analysis was executed using standard data science and version control tools:

* **Python libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `sweetviz`, `dataprep.eda`.
* **Version Control:** Git and GitHub.
* **Development Environment:** Visual Studio Code.

***

### Next Steps

The next phase of the project involves synthesizing the results:

* Sierra Leone's summarized metrics will be compared with those of **Benin and Togo**.
* The final investment potential will be determined using a **weighted scoring framework** applied across all three locations.

***

What aspects of the analysis would you like me to elaborate on, such as the specific effects of high humidity or the implications of lower irradiance?
