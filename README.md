Predicting-Stress-through-Digital-Habit-Analysis

This project leverages Machine Learning techniques to analyze and predict user stress levels based on digital footprints (smartphone usage) and health indicators (sleep quality, physical activity).
Developed as part of the Intelligent Systems Laboratory, the project focuses on the end-to-end Data Science lifecycle: from handling "dirty" raw data (outliers and missing values) to evaluating and comparing advanced regression algorithms.

📊 Dataset
The dataset comprises 15,000 records, featuring variables such as:
Digital Metrics: daily_screen_time_hours, phone_usage_before_sleep_minutes, notifications_received.
Health Metrics: sleep_duration_hours, sleep_quality_score, physical_activity_minutes.
Target Variable: stress_level (numeric scale from 1–10).

🛠️ Preprocessing Pipeline
To ensure model robustness, an automated pipeline was implemented to handle:
Robust Imputation: Missing values (NaN) are filled using the Median (for numerical data) and Mode (for categorical data).
Outlier Treatment: Applied Standardization (Z-score) to prevent extreme values from distorting model performance.
Encoding: Categorical variables (e.g., gender, occupation) are transformed via One-Hot Encoding.
Scaling: Features are brought to a common scale to optimize algorithmic convergence and performance.

🤖 Implemented Models
We evaluated three different algorithms to identify the most accurate solution:
Linear Regression: Served as the baseline model to identify linear relationships within the data.
Random Forest Regressor: An ensemble model chosen for its robustness against outliers and non-linear patterns.
XGBoost Regressor: An advanced Gradient Boosting algorithm utilized to achieve maximum predictive performance and efficiency.
