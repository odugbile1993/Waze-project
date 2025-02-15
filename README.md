Waze User Churn Analysis

Project Overview

Waze, a leading navigation app, aims to improve user retention by understanding and predicting user churn. Churn refers to users who have either uninstalled the app or stopped using it over a given period. This project focuses on analyzing monthly user churn to provide insights that will help optimize Waze's retention strategy.

Objectives

Build a dataframe for the churn dataset.

Identify and handle missing values.

Perform exploratory data analysis (EDA) to uncover patterns in user behavior.

Identify factors correlated with churn.

Compare churn characteristics between Android and iPhone users.

Provide actionable insights for improving user retention.

Data

The dataset consists of various features related to user engagement, including:

ID: Unique identifier for each user.

Device: User's device type (Android or iPhone).

Label: Churn status (0 = churned, 1 = retained).

Sessions, Drives, Total Sessions: Metrics related to app usage.

Navigations to Favorite Locations: Frequency of using favorite locations for navigation.

Driven KM & Duration Minutes: Measures of driving activity.

Activity & Driving Days: Frequency of app usage and driving behavior.

n_days_after_onboarding: Days since onboarding when the data was collected.

Key Analysis Steps

Data Cleaning & Preprocessing:

Identified and handled missing values.

Created new features such as km_per_drive, km_per_driving_day, and drives_per_driving_day for better insights.

Descriptive Statistics & Visualizations:

Compared median values between churned and retained users.

Assessed correlations between user activity and churn.

Device-Based Churn Analysis:

Calculated the churn rate for Android and iPhone users.

Compared user engagement metrics across device types.

Key Findings

Missing Data: The label column had missing values (253 for Android, 447 for iPhone). Other columns were unaffected.

Churn Rate:

Android users: ~4.75% churn rate.

iPhone users: ~4.62% churn rate.

User Behavior Differences:

Retained users had higher sessions, drives, and km_per_drive compared to churned users.

Users with lower engagement (fewer sessions and driving days) were more likely to churn.

Engagement Insights:

More frequent app usage (higher number of sessions, navigations, and driving days) correlated with retention.

Next Steps

Develop a predictive model to classify high-risk churn users.

Conduct A/B testing on targeted engagement strategies.

Explore additional features that may influence churn (e.g., app update frequency, notification interactions).

Repository Structure

📂 Waze-Churn-Analysis

├── data/                 # Raw and processed data files
├── notebooks/            # Jupyter notebooks for EDA and modeling
├── scripts/              # Python scripts for data processing
├── results/              # Visualization outputs and reports
├── README.md             # Project documentation

Technologies Used

Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn)

Jupyter Notebook

SQL (if applicable)

Contributors

Ayodele Odugbile
