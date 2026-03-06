# Delhivery Logistics Data Analysis 📦🚚

This project analyzes Delhivery's logistics delivery dataset to understand delivery performance, route efficiency, and operational patterns using data analytics techniques.

The analysis focuses on transforming raw segment-level logistics data into meaningful trip-level insights that can help improve delivery efficiency and route planning.

---

# Project Objective

The objective of this project is to analyze delivery operations and identify factors affecting delivery time using statistical analysis and data visualization.

Key goals include:

- Cleaning and preprocessing logistics data
- Aggregating segment-level data into trip-level insights
- Performing exploratory data analysis (EDA)
- Detecting and handling outliers
- Engineering meaningful features
- Performing hypothesis testing
- Extracting business insights and recommendations

---

# Dataset Information

The dataset contains detailed logistics delivery information including:

- Trip creation timestamps
- Source and destination centers
- Actual delivery time
- OSRM estimated time and distance
- Segment-level travel metrics

The dataset covers deliveries between **12 September 2018 and 8 October 2018**.

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy

---

# Project Workflow

## 1 Data Cleaning
- Converted time columns to datetime format
- Removed missing values
- Verified data consistency

## 2 Data Aggregation
Segment-level data was aggregated into:
- Segment-level summaries
- Trip-level summaries

---

## 3 Feature Engineering

New features created:

- Trip duration
- Month, day, weekday, hour
- Source city and state
- Destination city and state
- Average delivery speed
- Time prediction error

---

## 4 Exploratory Data Analysis

Performed:

- Univariate analysis
- Bivariate analysis
- Multivariate analysis

Key visualizations included:

- Delivery time distribution
- Distance distribution
- Route type comparison
- Correlation heatmaps

---

## 5 Outlier Detection

Outliers were identified using **boxplots** and treated using the **IQR method**.

---

## 6 Feature Encoding and Scaling

- Categorical variables encoded using **One-Hot Encoding**
- Numerical variables normalized using **MinMaxScaler**

---

## 7 Hypothesis Testing

Statistical hypothesis testing was conducted to validate relationships between aggregated delivery metrics.

Tests performed:

1. Actual delivery time vs OSRM estimated time
2. Actual time vs segment-level actual time
3. OSRM distance vs segment OSRM distance
4. OSRM time vs segment OSRM time

Paired **t-tests** were used for statistical validation.

---

# Key Insights

- Actual delivery times are significantly higher than OSRM estimated times.
- Delivery time strongly correlates with delivery distance.
- Major logistics hubs include **Bengaluru, Mumbai, and Gurgaon**.
- The highest delivery activity occurs in **Maharashtra, Karnataka, and Haryana**.
- Operational delays may occur between delivery segments due to hub processing or logistics operations.

---

# Business Recommendations

- Improve route prediction models by incorporating traffic and operational delays.
- Optimize high-volume logistics corridors.
- Improve processing efficiency at intermediate logistics hubs.
- Focus operational improvements on high-volume cities such as Bengaluru, Mumbai, and Gurgaon.

---
