![Description](path/to/image.png)
# 🌍 Climate-Induced Rainfall Extremes & Agricultural Risk in MENA

This capstone project explores how climate change impacts extreme rainfall patterns across the Middle East and North Africa (MENA), using CHIRPS-based exceedance probability data. The goal is to help identify risk-prone regions and support climate resilience and agricultural planning.

---

## 📁 Datasets Used

1. `subnational_anomaly_statistics.csv`  
   Contains anomaly statistics for subnational regions based on projected changes in rainfall extremes.

2. `climate_impact_pbi.csv`  
   A cleaned and clustered version of the original data, prepared for Power BI visualizations.

---

## 📌 Key Columns Explained

| Column         | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `ADM_REF`      | Name of the administrative region (e.g., district or governorate).          |
| `GID_0`        | ISO 3-letter country code (e.g., "EGY" for Egypt).                          |
| `MODEL`        | Climate model used for projections (e.g., "ACCESS-CM2").                   |
| `SCENARIO`     | Emission scenario used (e.g., "SSP3-7.0" = high-emission scenario).         |
| `VAR`          | Variable measured (e.g., `rx1day` = max 1-day rainfall).                   |
| `STATISTIC`    | Type of calculation (e.g., "mean", "stddev").                              |
| `YEAR`         | Projection year (2010–2039).                                                |
| `VALUE`        | Numeric anomaly/change value from baseline.                                |
| `UNIT`         | Unit of measurement (e.g., mm/day).                                        |
| `PERIOD`       | Projection time group (e.g., "2020-2029").                                 |

---

## ⚙️ Project Workflow

1. 📥 Data Loading & Cleaning  
   - Removed nulls and duplicates  
   - Standardized column names and formats

2. 📊 Exploratory Data Analysis (EDA)  
   - Summary statistics  
   - Outlier detection  
   - Correlation analysis

3. 🤖 Clustering with KMeans  
   - Grouped regions by climate risk using scaled anomaly data  
   - Evaluated using silhouette score

4. 💡 Innovation  
   - Added a custom “Season” column for seasonal trend exploration  
   - Created new classification logic for risk zones

5. 📈 Power BI Dashboard  
   - Interactive visuals (e.g., bar charts, slicers, cluster views)  
   - Temporal & spatial analysis of risk patterns

---

## 🧰 Tools Used

- Python (Pandas, NumPy, Seaborn, Scikit-learn, Matplotlib)
- Power BI
- CHIRPS dataset (Climate Hazards Group InfraRed Precipitation with Station data)

---

## 🌧️ About CHIRPS

CHIRPS combines satellite and ground-based station data to estimate global rainfall.  
It is especially useful in regions like MENA where weather station coverage is limited.  
This makes it ideal for agricultural and drought risk assessment.

---

## 🎯 Project Objective

To detect regional patterns of extreme rainfall anomalies and assess their potential risks for agriculture in the MENA region, based on climate model projections from 2010 to 2039.

---

## 🖼️ Screenshots

screenshots Added Here:

```md
![Data Cleaning Example](bigdata_final_exam/data cleaning process.png)
![Clustered Regions](bigdata_final_exam/classifications,regression.png)
![Clustered Regions](bigdata_final_exam/display first 5 rows.png)
![Correlation Distribute](bigdata_final_exam/distribute correlation.png)
![distubute mean](bigdata_final_exam/distribution  mean.png)
![distubute max](bigdata_final_exam/distribution_max.png)
![distubute min](bigdata_final_exam/distubute min.png)
![Power BI Dashboard](bigdata_final_exam/dashboard.png)
![Power BI Dashboard](bigdata_final_exam/dash2.png)
