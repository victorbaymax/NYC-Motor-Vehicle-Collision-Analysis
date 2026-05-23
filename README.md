# NYC Motor Vehicle Collision Analysis

## Project Overview

This project analyzes motor vehicle collision data from New York City in order to identify trends, contributing factors, and patterns associated with traffic accidents and injuries. The project combines exploratory data analysis, statistical analysis, data visualization, and machine learning techniques to better understand traffic safety conditions across NYC boroughs.

The analysis was completed as part of the Flatiron School AI and Machine Learning program using Python, Jupyter Notebook, Pandas, Matplotlib, Seaborn, and Scikit-learn.

The project also includes a machine learning pipeline designed to predict whether a collision resulted in injuries based on crash-related features.

---

# BLUF (Bottom Line Up Front)

The analysis found that:

- Brooklyn and Queens experienced the highest number of collisions.
- Collision frequency peaks during morning and evening commuting hours.
- Driver Inattention/Distraction was the most common contributing factor associated with accidents.
- Most collisions did not result in fatalities, but injuries remain common across all boroughs.
- Traffic patterns, driver behavior, and congestion appear to be strongly associated with collision frequency.

The machine learning models demonstrated that crash-related features such as contributing factors, location, and time-based variables can be used to reasonably predict whether a collision is likely to result in injuries.

---

# Business Problem

Traffic accidents remain a major public safety concern in urban environments such as New York City. Understanding when, where, and why collisions occur can help transportation agencies and policymakers improve road safety and reduce injuries.

This project seeks to answer the following questions:

- Which boroughs experience the most collisions?
- What times of day are most associated with crashes?
- What are the most common contributing factors?
- Which variables are associated with injury-related collisions?
- Can machine learning models predict whether a crash will result in injuries?

---

# Dataset Information

Dataset Source:

- NYC Open Data Motor Vehicle Collisions Dataset:
https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95

The dataset contains information on:
- Crash dates and times
- Boroughs and geographic coordinates
- Injuries and fatalities
- Contributing factors
- Vehicle types
- Pedestrian and cyclist involvement

---

# Technologies Used

## Programming Language
- Python

## Libraries
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Tools
- Jupyter Notebook
- Tableau
- GitHub

---

# Repository Structure

```text
NYC-Traffic-Collision-Analysis/
│
├── data/
│   ├── Motor_Vehicle_Collisions.csv
│   └── MVCollisionsDataDictionary.xlsx
│
├── notebooks/
│   └── nyc_motor_vehicle_collision_analysis_final.ipynb
│
├── images/
│   ├── crashes_by_borough.png
│   ├── crashes_by_hour.png
│   ├── contributing_factors.png
│   ├── confusion_matrix.png
│   └── feature_importance.png
│
├── README.md
├── requirements.txt
├── .gitignore
│
└── LICENSE
```

---

# Data Cleaning and Preparation

The dataset required several preprocessing steps before analysis:

- Converted crash date columns into datetime format
- Extracted hour, weekday, and month features
- Handled missing values
- Filtered invalid coordinates
- Simplified contributing factor categories
- Created injury classification labels for machine learning

Feature engineering was also performed to create:
- Hour of crash
- Day of week
- Injury indicator variables
- Severity-related fields

---

# Exploratory Data Analysis (EDA)

The notebook includes comprehensive exploratory analysis including:

## Temporal Analysis
- Collisions by hour of day
- Collisions by weekday
- Monthly collision trends

## Geographic Analysis
- Collisions by borough
- Injury distributions by borough

## Contributing Factors
- Top contributing causes of collisions
- Driver distraction analysis
- Failure-to-yield analysis

## Injury Analysis
- Injury and fatality distributions
- Correlation heatmaps
- Severity comparisons

---

# Machine Learning Modeling

This project includes a supervised machine learning section to predict whether a collision resulted in injuries.

## Target Variable
- Injury Accident Classification

## Baseline Model
- Logistic Regression

## Final Model
- Random Forest Classifier

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

---

# Scikit-learn Pipeline Implementation

The project uses a Scikit-learn Pipeline and ColumnTransformer to streamline preprocessing and model training.

The pipeline includes:
- Missing value imputation
- Feature scaling
- One-hot encoding for categorical variables
- Model integration

This approach improves reproducibility and follows machine learning best practices.

---

# Key Findings

## Major Insights
- Driver Inattention/Distraction was the leading contributing factor in collisions.
- Collision frequency was highest during commuting hours.
- Brooklyn and Queens experienced the largest number of crashes.
- Weekdays showed higher collision volume compared to weekends.
- Injury-related collisions can be partially predicted using crash-related features.

---

# Recommendations

Based on the analysis, several recommendations were identified:

1. Increase enforcement related to distracted driving during peak commuting hours.

2. Improve traffic infrastructure at high-collision intersections, including:
   - street lighting,
   - pedestrian crossings,
   - and traffic signal optimization.

3. Expand public safety campaigns focused on distracted driving and failure-to-yield behaviors.

4. Prioritize collision hotspot analysis for future transportation planning initiatives.

---

# How to Run the Project

## 1. Clone the Repository

```bash
git clone <your-github-repo-link>
```

## 2. Install Dependencies

```bash
pip install -r requirements.txt
```

## 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
nyc_motor_vehicle_collision_analysis_final.ipynb
```

---

# Future Improvements

Potential future enhancements include:
- Weather data integration
- Geospatial hotspot clustering
- Real-time accident forecasting
- Additional machine learning optimization
- Interactive web dashboard deployment

---

# Author

Victor Bhowmik

Flatiron School — AI & Machine Learning Program

2026
