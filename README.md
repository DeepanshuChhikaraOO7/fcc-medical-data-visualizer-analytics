# 🏥 Medical Data Visualizer

### 🚀 Project Overview
A data analytics project that visualizes and explores the relationship between lifestyle choices (activity, smoking, alcohol) and cardiac disease. Using **Python**, **Pandas**, and **Seaborn**, this project processes medical examination data to identify key indicators of heart health.

**Key Objective:** Normalize, clean, and visualize a dataset of 70,000+ patient records to produce production-grade categorical plots and heatmaps.

### 📊 Visualizations Generated
This project generates two complex visualizations to analyze patient health:

#### 1. Categorical Feature Analysis (Cardio vs. Lifestyle)
* **Technique:** Data Melting & Categorical Plotting (`sns.catplot`).
* **Insight:** Compares the counts of active/inactive, smokers/non-smokers, and cholesterol levels across patients with and without cardiovascular disease.
* **Metric:** Properly normalized values (0=Good, 1=Bad) for consistent analysis.

#### 2. Correlation Heatmap (Health Metrics)
* **Technique:** Correlation Matrix with Upper Triangle Masking (`sns.heatmap`).
* **Insight:** Reveals relationships between systolic/diastolic blood pressure, weight, and cholesterol.
* **Data Cleaning:** Implemented strict filtering logic to remove outliers (e.g., diastolic pressure > systolic, invalid height/weight percentiles).

### 🛠️ Tech Stack
* **Language:** Python 3.x
* **Data Manipulation:** Pandas (Filtering, Normalization, BMI Calculation)
* **Visualization:** Seaborn (Catplots, Heatmaps), Matplotlib
* **Mathematics:** Numpy (Mask generation)

### 🔑 Key Data Engineering Steps
* **Feature Engineering:** Calculated a new `overweight` feature based on BMI (Weight / Height²).
* **Data Normalization:** Standardized Glucose and Cholesterol levels into binary classifications (0: Normal, 1: High).
* **Outlier Removal:** Filtered patient segments falling outside the 2.5th and 97.5th percentiles for height and weight to ensure statistical accuracy.

### 🏆 Certification
This project is part of the **FreeCodeCamp Data Analysis with Python Certification**.
