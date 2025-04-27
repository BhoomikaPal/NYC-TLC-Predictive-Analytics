# NYC TLC Predictive Analytics

## Project Title
**Predictive Modeling and Analysis of New York City Taxi and Limousine Commission Data**

---

## Project Overview
The goal of this project is to assist the New York City Taxi and Limousine Commission (NYC TLC) by analyzing taxi trip data, conducting statistical tests, building predictive models, and generating actionable insights.  
The project progressed through multiple phases, including exploratory data analysis (EDA), A/B testing, regression modeling, and machine learning modeling.  
The final machine learning model aimed to predict the likelihood of a customer leaving a tip, helping taxi drivers maximize their earnings.  
Additionally, multiple linear regression models were developed to predict fare amounts based on trip characteristics.

---

## Business Understanding
The NYC TLC faced challenges in better understanding customer behavior, trip costs, and tip predictions to improve both rider and driver experiences. Automatidata was tasked with:

- Cleaning and exploring the available trip data.
- Analyzing factors that influence payment behaviors.
- Building predictive models for fare estimation and tip likelihood.
- Delivering insights that could lead to better operational tools, such as fare estimation apps and tip prediction alerts for drivers.

Through this work, NYC TLC could enhance customer transparency, optimize driver performance, and support new technology development.

---

## Data Understanding
The dataset provided by NYC TLC included detailed information on taxi and limousine trips across New York City, collected over the course of a year.

**Key features:**
- Trip distance
- Pickup and dropoff times
- Payment type
- Fare amount
- Tip amount
- Passenger count
- Ride duration

**Data Preparation and Cleaning:**
- Missing values were identified and handled appropriately.
- Data was cleaned to remove erroneous records (e.g., trips with zero distance or zero fare).
- New features were engineered, including `mean_duration`, `mean_distance`, and `predicted_fare` based on observed patterns.
- Categorical columns like payment type were encoded numerically.
- Tableau dashboards were also created to visually represent trip activity across New York City for accessibility, including accommodations for users with visual impairments.

---

## Modelling and Evaluation

Multiple modeling approaches were applied throughout the project:

### Statistical Analysis
- An A/B test was conducted to analyze the relationship between fare amount and payment type.

### Regression Analysis
- A multiple linear regression model was built to predict taxi fare amounts.

**Key insights:**
- For every mile traveled, the fare increases by approximately **$2**.
- For every **3.57 miles**, the fare increases by about **$7.13**.

**Model performance metrics:**
- **R-squared:** 0.868 (86.8% of variance explained)
- **MAE:** 2.13
- **MSE:** 14.34
- **RMSE:** 3.8

### Machine Learning Model
- A Random Forest classifier was developed to predict whether a customer would leave a tip.

**Most important features for tip prediction:**
- `mean_duration`
- `predicted_fare`
- `mean_distance`

The Random Forest model showed modest predictive ability and could be useful as a supporting tool for drivers if tested and deployed carefully.

---

## Conclusion
The project successfully delivered actionable insights and predictive models to support the goals of NYC TLC.

**Major outcomes include:**
- A strong multiple linear regression model for fare prediction.
- Identification of key variables influencing customer tipping behavior.
- Creation of an accessible Tableau dashboard to visualize trip patterns across NYC.

**These findings can be leveraged to:**
- Create a fare estimator app for riders.
- Develop an early warning system for drivers regarding tipping likelihood.
- Enhance operational planning and customer experience improvements for NYC TLC.

While the Random Forest model was not perfect, it provides useful signals that could be further improved with additional data and feature engineering.

---
