# Phase-DATASET-and-DATA-cleaning and model building
Data Preprocessing
Dropped non-numeric columns (like timestamps).
Handled missing values and outliers.
Normalized and standardized features using StandardScaler.
Created engineered features (like cyclical encoding for hours: hour_sin, hour_cos).
Exploratory Data Analysis (EDA)
Plotted line graphs of energy usage vs. time.
Histograms for temperature, humidity, and student presence.
Correlation heatmap to check feature relationships.
Observed patterns like higher usage during weekdays and semesters.
Feature Selection
Tried Forward Selection and Backward Selection.
Also experimented with PCA for dimensionality reduction.
Final features included: students_present, temperature_C, appliances_on, is_weekday, in_semester, humidity_pct, hvac_load, solar_gen_kwh, hour_sin, hour_cos.
Model Development
Implemented Linear Regression as baseline.
Compared with KNN Regression and Random Forest Regression.
Used train-test split and cross-validation for evaluation.
Evaluation
Metrics used: MAE, RMSE, R² score.
Random Forest gave the best performance with lowest error and highest R².
