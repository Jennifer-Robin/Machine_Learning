# Machine_Learning

# Project 1

Zomato User Preference Prediction 

 **Problem Statement**
 
The goal is to analyze and predict user preferences on Zomato based on aggregated restaurant ratings across different countries. By identifying patterns in customer satisfaction, this project helps restaurants tailor their offerings to regional preferences.

**Objective**

Build a predictive model that uses restaurant-level features (such as cuisine, pricing, and delivery options) to understand what influences ratings and votes.

**Dataset Description**

Restaurant ID & Name – Unique identifiers

Country Code, City, Locality, Address – Geographical data

Longitude & Latitude – Coordinates

Cuisines – Types of food offered

Currency – Local transaction currency

Has Table Booking, Has Online Delivery, Is Delivering Now – Availability flags

Price Range – Cost level (1 to 4)

Aggregate Rating –  Target variable

Rating Color, Rating Text – Visual/textual rating labels

Votes – Number of user votes

**Techniques Used**

Data Cleaning & Handling Null Values

Exploratory Data Analysis (EDA)

Feature Engineering

Regression Models: Linear, Random Forest

Evaluation Metrics: R² Score, RMSE, MAE

 **Business Value**
 
The model helps Zomato and its restaurant partners understand what drives customer satisfaction and how it differs across countries—improving user experience and strategic planning.

----



 # Project 2
 
 Employee Mental Health Treatment Prediction 
 
**Problem Statement**

Following a sudden employee loss at XYZ Technical Solutions, the company seeks to predict which employees may require mental health treatment using existing survey data.

**Objective**

Build a classification model to predict whether an employee needs treatment based on workplace policies, demographics, and mental health awareness.

**Dataset Description**

Demographics: Age, Gender, Country, State

Work Attributes: Remote work, Tech company, Self-employed, No. of employees

Mental Health Awareness: Family history, Work interference, Benefits, Resources, Anonymity

Perception Variables: Supervisor support, Interview comfort, Perceived consequences

Target Variable: treatment (Yes/No)

 **Submission Format**
 
csv

ID, treatment

1, Yes

2, No


**Techniques Used**

Categorical Encoding

Missing Value Imputation

Feature Selection

Classification Models: Logistic Regression, Random Forest, XGBoost

Evaluation: Accuracy, Precision, Recall, F1 Score

 **Business Value**
 
Helps organizations proactively identify employees who may be struggling with mental health issues and implement targeted wellness programs.

---

# Project 3

# 🚦 Smart Signals for a Smarter Bengaluru

A machine learning project to optimize traffic signal durations based on real-time vehicle flow, helping reduce congestion and improve urban mobility in Bengaluru.


## 📌 Project Objective

The goal of this project is to predict optimal green signal durations at traffic junctions using data science techniques. By analyzing vehicle flow across different times of the day, the system can dynamically adjust signal timing to enhance traffic efficiency.



## 📂 Dataset Overview

A simulated dataset was used, representing traffic at **7 major junctions** in Bengaluru. Each data point includes:
- `timestamp` – 15-minute interval records
- `junction_id` – unique identifier
- `north`, `south`, `east`, `west` – vehicle count per direction
- `signal_duration` – current green light duration

> Additional features: total vehicle count, hour of day, time of day classification


## 🔍 Exploratory Data Analysis (EDA)

Key insights uncovered:
 📈 Traffic peaks during morning and evening hours
 🕒 Signal durations did not always align with actual traffic volume
 📊 Distribution and KDE plots showed consistent error margins within ±6 seconds

Visuals include:
 Vehicle flow by hour
 Signal duration trends
 Time-of-day comparison
 Junction-level performance


## 🤖 Model Development

 **Algorithm:** Random Forest Regressor
 **Problem Type:** Regression
 **Features:** Hour of day, vehicle flow from all directions
 **Target:** Signal duration (seconds)
 **Evaluation:**  
   Mean Absolute Error ~ **5 seconds**
   Error distribution was centered and balanced


## ⚙️ Optimization Use-Case

A dynamic adjustment strategy was proposed:
 **+20% signal duration** during peak hours (morning & evening)
 **−10%** during off-peak times (midday & late evening)

This scenario reduces congestion while optimizing signal operation efficiency.


## 🧠 Skills Applied

 Feature engineering  
 EDA & data visualization  
 Regression modeling  
 Urban mobility optimization  
 Python, Pandas, Seaborn, Scikit-learn


## 📈 Results

This model proves that real-time traffic data can guide adaptive traffic signal management, leading to better traffic flow and resource utilization in urban cities like Bengaluru.

---
# Project 4

🚦 Urban Traffic Congestion Prediction & Optimization - Bengaluru
This project uses machine learning and rule-based logic to predict and optimize traffic congestion in the urban environment of Bengaluru, India. With growing vehicle density and static signal systems, the goal is to develop a data-driven approach to support urban mobility and reduce congestion.

## Problem Statement
Bengaluru suffers from rising traffic congestion due to:

Fixed signal timings

Inconsistent traffic volume

Limited real-time responsiveness

##Objectives:

Predict congestion levels based on real-world features.

Identify traffic hotspots.

Implement a rule-based signal timing strategy to reduce congestion during peak hours.

##📦 Dataset Overview
Source: Simulated dataset inspired by public data (Kaggle/manual collection)
Records: Thousands of hourly entries across multiple roads and intersections in Bengaluru

##Key Features:

Area Name, Road/Intersection

Traffic Volume, Average Speed, Travel Time Index

Weather, Incident Reports, Signal Compliance

Public Transport Usage, Parking Usage, Pedestrian Count

Target: Congestion Level (continuous range: 5–100)

##📊 Exploratory Data Analysis (EDA)
Heatmaps and Sunburst plots to locate congestion hotspots like Indiranagar, Koramangala

Scatter plots to show inverse relationship between speed and volume

Boxplots for Travel Time Index variability across areas

Pie charts summarizing incident reports per area

##🧪 Data Preprocessing & Feature Engineering
Handled nulls, outliers, and scaling

Label encoded categorical features

Extracted Hour from timestamp to capture peak hours

Scaled numerical fields using StandardScaler

##🤖 Model Building
Tested multiple regression models:

Linear Regression

Random Forest Regressor ✅ (Best performer)

XGBoost Regressor

Model Performance (Random Forest):

R² Score: 0.96

MAE: 2.85

RMSE: 4.31

##🧠 Signal Optimization Logic
Implemented a simple rule-based logic:

python
Copy
Edit
if congestion > 85 and hour in peak_hours:
    extend_signal_time()
✅ Resulted in a visible drop in average congestion during simulated peak hours.

##📈 Results
Successfully predicted congestion across locations and times

Identified traffic-heavy zones

Simulated signal adjustment led to congestion reduction

##🚀 Future Enhancements
Integrate real-time traffic data via IoT or GPS

Use LSTM or time-series deep learning models

Deploy Reinforcement Learning for real-time signal optimization

Create a dashboard for city traffic authorities

Extend model to multiple Indian cities

re (Add your PDF or Google Slides link)

🙌 Acknowledgements
Special thanks to open data contributors and the Data Science faculty at Imarticus Learning, Bangalore.




