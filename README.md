# 🔋 EV Battery Health Analysis

## 📌 Project Overview

Electric Vehicles (EVs) are becoming increasingly popular because of their environmental benefits and energy efficiency. The battery is one of the most important components of an electric vehicle, and its performance directly affects vehicle efficiency, reliability, and lifespan.

This project focuses on analyzing Electric Vehicle (EV) battery health using Python and Data Analytics techniques. The main objective is to understand battery degradation, identify factors affecting battery performance, and analyze battery failure risks.

The project uses an EV Battery Health dataset containing 50,000 records and 35 original columns. After data cleaning and feature engineering, the dataset contains 50,000 records and 37 columns.

## 🎯 Project Objectives

- Analyze the overall health and performance of EV batteries.
- Understand the relationship between battery age and battery degradation.
- Study how charging patterns affect battery health.
- Analyze the impact of temperature and environmental conditions on battery performance.
- Identify factors associated with battery failure risk.
- Examine battery capacity fade and State of Health (SOH).
- Explore battery manufacturers and battery chemistries.
- Generate meaningful insights to support better battery management.

## 📂 Dataset Information

**Dataset Name:** `ev_battery_health.csv`

**Total Records:** 50,000

**Original Columns:** 35

**Final Columns After Cleaning:** 37

### Important Dataset Features

| Column | Description |
|---|---|
| battery_id | Unique battery identification |
| chemistry | Battery chemistry type |
| manufacturer | Battery manufacturer |
| vehicle_model | Electric vehicle model |
| pack_capacity_kwh | Battery capacity |
| battery_age_days | Battery age in days |
| cycle_count | Number of charge cycles |
| avg_daily_distance_km | Average daily driving distance |
| avg_charging_power_kw | Average charging power |
| fast_charge_ratio | Fast charging usage ratio |
| avg_depth_of_discharge_pct | Average depth of discharge |
| avg_state_of_charge_pct | Average state of charge |
| avg_ambient_temp_c | Average ambient temperature |
| humidity_pct | Environmental humidity |
| internal_resistance_mohm | Internal battery resistance |
| capacity_fade_pct | Battery capacity degradation |
| state_of_health_pct | Battery State of Health |
| remaining_useful_life_cycles | Estimated remaining battery cycles |
| failure_risk_label | Battery failure risk classification |
| degradation_category | Battery degradation category |

## 🛠️ Tools and Technologies

- Python
- Jupyter Notebook
- Anaconda
- Pandas
- NumPy
- Matplotlib
- Seaborn

## 🧹 Data Cleaning and Preprocessing

The following data cleaning activities were performed:

1. Loaded the original EV Battery Health dataset.
2. Inspected dataset structure, columns, and data types.
3. Checked and verified duplicate records.
4. Converted date columns into datetime format.
5. Identified missing values in numerical, categorical, and date columns.
6. Handled numerical missing values using median imputation.
7. Handled categorical missing values using mode imputation.
8. Identified potential outliers using the Interquartile Range (IQR) method.
9. Checked invalid numerical values and date inconsistencies.
10. Created additional features for further analysis.
11. Verified the final dataset structure and data types.

**Note:** Missing values in the date columns were retained because their actual dates could not be reliably determined. Potential outliers were identified but not automatically removed.

## ⚙️ Feature Engineering

Two additional features were created:

### 1. Temperature Difference

Calculates the difference between peak fast-charging temperature and average ambient temperature.

`temperature_difference = peak_temp_during_fast_charge_c - avg_ambient_temp_c`

### 2. Calculated Battery Age

Calculates battery age using manufacture date and observation date.

`calculated_battery_age_days = observation_date - manufacture_date`

These features help explore battery temperature behavior and battery aging.

## 📊 Exploratory Data Analysis (EDA)

The project includes the following analysis areas:

- Descriptive Statistical Analysis
- Univariate Analysis
- Bivariate Analysis
- Multivariate Analysis
- Distribution Analysis
- Correlation Analysis
- GroupBy Analysis
- Pivot Table Analysis
- Data Visualization

## 📈 Expected Insights

The analysis aims to identify:

1. How battery age influences State of Health.
2. The relationship between cycle count and capacity fade.
3. How fast charging affects battery temperature.
4. The impact of temperature on battery degradation.
5. Differences in battery health across battery chemistries.
6. Factors associated with battery failure risk.
7. The relationship between internal resistance and battery health.

*These are investigation objectives; final findings will be added after completing the analysis.*



## 🚀 How to Run the Project

1. Clone or download this repository.
2. Install Python and Anaconda.
3. Open Jupyter Notebook.
4. Open `EV_Battery_Health_Analysis.ipynb`.
5. Make sure the dataset CSV file is in the correct folder.
6. Run the notebook cells step by step.

### Install Required Libraries

```python
pip install pandas numpy matplotlib seaborn
```

## 🏁 Conclusion

This project uses Python-based data analytics techniques to investigate EV battery health and performance. Through data cleaning, preprocessing, feature engineering, statistical analysis, and visualization, the project aims to identify important factors influencing battery degradation and failure risk.

The findings can help improve understanding of EV battery behavior and support better battery maintenance and management decisions.

## 👨‍💻 Author

**Ajmal Asharaf**

Data Analytics Project
