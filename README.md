# Weather Temperature Impact on Daily Stress Levels

## Project Overview
In this project, I aim to observe if there is a relation between my daily stress levels and weather temperature or not. Over the next one month, I am planning on monitoring my stress levels 4 times a day through my smart watch and also noting the temperature and weather condition at the moment that I am recording my stress levels. I will also include the days of the week as a factor for this experiment. This project will involve data collection, explaratory data analysis, feature engineering and visualization techniques.

## Objectives
* Identify Stress Level Influencers: Observe the relationship between the day of the week, time of the day, temperature, weather condition and my stress levels.
* Detect Key Factors: Determine key factors that have the strongest impact on relatively lower stress levels.
* Applying Data Science Skills: Implement skills I have attained through DSA 210 course to improve my life quality. 
* Data-Driven Improving: Using the results from the analysis, I will work on improving my low stress levels according to the key factors that  influence my stress levels.

## Motivation
I have been struggling with anxiety for years and I really want to do something for it all by myself. I want to see if I can somehow manage it by knowing the factors that have an impact on it. Thus, I will be one step ahead on learning how to improve my life quality on my own.

## Dataset
The dataset consists of factors such as day of the week including the date, temperature, weather condition, time of the day and my stress levels.
The data will be collected from the following sources:
* Apple Weather App: I will collect temperature and weather condition data from the Weather App of my Apple device.
* Smartphone: The data of date and time of the day will be collected from my smartphone.
* Stress Levels: I will track my stress levels in the morning, afternoon, evening and at night each day through my smart watch.

## Plan
1. Data Collection: Data will be collected over the next one month maintaining consistent times of the day and ensuring data consistency.
2. Data Preperation and Analysis: Data will be reviewed for consistency and completeness at the end of the collection process. Exploratory Data Analysis will be conducted by identifying trends using statistical methods and visualization techniques. Regression Analysis will be made by applying Statistical Methods to study the the influence of different factors on stress levels. 

## Hypothesis
* Null Hypothesis (H₀): There is no significant relationship between temperature, weather condition and stress levels. Increase in temperature and improvement in weather condition do not significantly affect stress levels throughout the day.
* Alternative Hypothesis (Hₐ): There is a significant relationship between various factors and daily stress levels. As temperature increases and weather condition improves, daily stress levels decrease.


# Report
## Introduction
The main objective of this project is to analyze the relationship between weather conditions, temperature, time of day, and day of the week on daily stress levels. This study aims to determine how these external factors influence fluctuations in stress throughout the day. By identifying patterns and correlations in the data, the project seeks to provide data-driven insights that may help improve stress awareness, support personal well-being decisions, and  contribute to better lifestyle management.

## Restating Hypothesis
* Null Hypothesis (H₀): There is no significant relationship between temperature, weather condition and stress levels. Increase in temperature and improvement in weather condition do not significantly affect stress levels throughout the day.
* Alternative Hypothesis (Hₐ): There is a significant relationship between various factors and daily stress levels. As temperature increases and weather condition improves, daily stress levels decrease.

## Methods
### Data Collection
Stress level data was recorded four times a day using a smartwatch, alongside real-time weather conditions and temperature from the Apple Weather App. Each entry was reported with the corresponding time of day and day of the week.

### Data Preprocessing & Feature Engineering
* Created new features such as is_weekend to differentiate weekday and weekend stress patterns.
* Categorical variables (e.g., weather condition, day of week) were one-hot encoded.
* Numerical values (e.g., temperature) were scaled using standardization.

### Model Training
* Several machine learning models were applied to predict absolute stress levels, including:
 - Random Forest Regressor
 - Support Vector Regressor (SVR)
 - K-Nearest Neighbors Regressor (kNN)

### Evaluation & Visualization
Model performance was assessed using:
* Mean Squared Error (MSE)
* R² Score (explained variance)
* Actual vs. predicted stress levels were visualized with scatter plots to assess model fit.

## Machine Learning Test Result
<img width="658" alt="Model Performance Comparison" src="https://github.com/user-attachments/assets/ca0f3bb2-2e18-4e52-8f34-dc673e2e2d7a" />

## Findings
The analysis revealed that weather conditions, temperature, time of day, and day of the week have only a modest impact on daily stress levels. Specifically:
* Support Vector Regressor performed the best among the models tested, but still yielded a relatively low R² score (~0.25), indicating that only about 25% of the variation in stress levels could be explained by the selected features.

Both Random Forest Regressor and k-Nearest Neighbors models demonstrated even weaker predictive power, further confirming that these external environmental factors alone are not strong determinants of stress.

Despite the limited predictive strength, these findings show us that: While weather and timing may contribute minor fluctuations, they are not sufficient on their own to reliably predict stress levels.

## Limitations
* Small sample size: One month of data limits the model’s generalizability.
* Sensor inaccuracy: Smartwatch-based stress measurements may contain noise.
* Coarse weather data: Sudden environmental changes may have gone unrecorded.
* Model limitations: Assumptions of ML models may not fully capture complex human behavior.

## Future Work
* Include behavioral data: Include variables like sleep quality, academic workload, or physical activity for a more comprehensive view of stress.
* Expand data collection: Gather data over multiple months or seasons to capture long-term patterns and variability.
* Improve stress measurement: Combine smartwatch data with self-reported stress levels for greater accuracy.

## Conclusion
This project investigated whether weather conditions, temperature, time of day, and day of the week significantly affect stress levels. While the initial hypothesis assumed a meaningful relationship, the results showed only weak predictive power across all models (best R² ≈ 0.25).

Thus, we fail to reject the null hypothesis(H₀): There is no significant relationship between temperature, weather condition and stress levels. Increase in temperature and improvement in weather condition do not significantly affect stress levels throughout the day.

     
 
