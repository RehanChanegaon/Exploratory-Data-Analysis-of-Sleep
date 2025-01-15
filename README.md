# Exploratory Data Analysis of Sleep

## Introduction

This project is focused on analyzing the sleep patterns of individuals based on various factors such as age, gender, lifestyle habits (caffeine, alcohol, smoking), and sleep stages. The goal is to identify key insights that can help understand the impact of different variables on sleep quality, duration, and efficiency.

## Dataset Overview

The dataset contains the following columns:

| **Column Name**             | **Description**                                                                                               |
|-----------------------------|---------------------------------------------------------------------------------------------------------------|
| `ID`                        | Unique identifier for each individual in the dataset.                                                         |
| `Age`                       | Age of the individual.                                                                                        |
| `Gender`                    | Gender of the individual (Male/Female).                                                                       |
| `Bedtime`                   | The time the individual went to bed, used to calculate the sleep window and bedtime patterns.                  |
| `Wakeup time`               | The time the individual woke up, used to calculate the sleep window and wake-up patterns.                      |
| `Sleep duration`            | Total hours of sleep for the individual, calculated from bedtime and wake-up time.                             |
| `Sleep efficiency`          | The ratio of actual sleep duration to the time spent in bed, expressed as a percentage.                        |
| `REM sleep percentage`      | The percentage of sleep spent in the REM (Rapid Eye Movement) stage.                                           |
| `Deep sleep percentage`     | The percentage of sleep spent in deep sleep, a crucial stage for physical recovery.                           |
| `Light sleep percentage`    | The percentage of sleep spent in light sleep, the less restorative phase of sleep.                            |
| `Awakenings`                | Number of times the individual woke up during their sleep.                                                     |
| `Caffeine consumption`      | Amount of caffeine consumed by the individual (in terms of cups or milligrams).                                |
| `Alcohol consumption`       | Amount of alcohol consumed by the individual.                                                                 |
| `Smoking status`            | Indicates whether the individual smokes (Yes/No).                                                             |
| `Exercise frequency`        | The number of times the individual exercises per week.                                                         |

## Objectives

The primary objectives of this analysis are:

1. To investigate the relationship between **age**, **gender**, and **sleep duration**.
2. To explore how lifestyle habits like **caffeine consumption**, **alcohol consumption**, **smoking**, and **exercise frequency** affect **sleep efficiency** and **sleep quality**.
3. To examine the distribution of different sleep stages (REM, Deep, Light) and how they vary by **age**, **gender**, and **lifestyle**.
4. To analyze patterns of **awakenings** and their impact on overall sleep efficiency.

## Steps in the Analysis

1. **Data Cleaning and Preparation**
   - Convert date and time columns (`Bedtime`, `Wakeup time`) to appropriate datetime format.
   - Categorize age into groups to facilitate age-based analysis.
   - Generate new columns such as **Sleep Window** (the total time from bedtime to wakeup) and **Sleep Deviation** (difference between sleep window and actual sleep duration).

2. **Exploratory Data Analysis (EDA)**
   - **Distribution Analysis**: Understand the distribution of variables such as sleep duration, REM sleep, deep sleep, and light sleep percentages.
   - **Correlation Analysis**: Investigate correlations between different variables (e.g., sleep efficiency vs. lifestyle factors).
   - **Visualizations**: Create visualizations such as histograms, bar charts, and scatter plots to better understand the patterns.

3. **Lifestyle Impact on Sleep**
   - Calculate a **Lifestyle Impact Score** based on caffeine, alcohol, smoking, and exercise to quantify how these factors affect sleep duration and efficiency.
   - Investigate the relationship between this score and sleep quality (based on sleep efficiency).

4. **Sleep Quality Classification**
   - Classify individuals' sleep quality as **High**, **Moderate**, or **Low** based on their sleep efficiency.
   - Analyze how age, gender, and lifestyle factors influence the likelihood of achieving good sleep quality.

## Conclusion

This analysis aims to provide deeper insights into the factors that influence sleep quality and duration. By analyzing patterns in the dataset, we aim to identify key trends that can help individuals optimize their sleep habits for better health and well-being.

## Future Work

Potential future improvements include:

- Expanding the dataset to include more individuals for a more comprehensive analysis.
- Investigating the impact of external factors such as work schedules and stress levels on sleep patterns.
- Developing a predictive model to estimate sleep efficiency based on lifestyle habits and demographic data.

