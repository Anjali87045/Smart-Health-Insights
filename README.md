# Bellabeat Analytics: Smart Health Insights

## Table of Contents
1. [Project Overview](#project-overview)
2. [Business Objective](#business-objective)
3. [Stakeholders](#stakeholders)
4. [Data Source ](#data-source)
5. [Data Preparation](#data-preparation)
6. [Exploratory Data Analysis](#exploratory-data-analysis)
7. [Advanced Analysis and Modeling](#advanced-analysis-and-modeling)
8. [Key Insights and Findings](#key-insights-and-findings)
9. [Strategic Recommendations](#strategic-recommendations)
10. [Implementation Roadmap](#implementation-roadmap)
11. [Success Metrics](#success-metrics)
12. [Technical Summary](#technical-summary)


## Project Overview
This project involves a comprehensive analysis of FitBit Fitness Tracker data to uncover actionable insights for Bellabeat, a wellness technology company. By understanding user behavior and trends in smart device usage, this analysis aims to provide strategic recommendations to enhance Bellabeat's product line and marketing strategies.

## Business Objective
The primary objective is to analyze user data from FitBit devices and apply the insights to improve Bellabeat's products—such as the Leaf tracker, Time watch, and Spring water bottle—and to optimize marketing efforts.

## Stakeholders
- **Urška Sršen (Cofounder & CCO):** Focuses on driving product innovation and creative direction.
- **Sando Mur (Cofounder):** Concentrates on business strategy and financial growth.
- **Marketing Analytics Team:** Requires actionable insights for optimizing marketing campaigns.
- **Product Development Team:** Needs data-driven insights to inform product improvements.

## Data Source 
### Data Source:
The analysis is based on publicly available FitBit Fitness Tracker data, which includes:
- `dailyActivity_merged.csv`
- `sleepDay_merged.csv`
- `heartrate_seconds_merged.csv`


## Data Preparation
### Data Cleaning:
- **Missing Data:** Imputed missing values with mean/mode where appropriate.
- **Duplicates:** Identified and removed duplicate records.
- **Outliers:** Applied the Interquartile Range (IQR) method to detect and remove outliers in key variables like `TotalSteps`.

### Data Transformation:
- **Date Conversion:** Converted date columns to `datetime` format.
- **Feature Engineering:** Created new features such as `ActivityIntensityRatio`, `DayOfWeek`, and `IsWeekend` to enrich the dataset.
- **Merging Datasets:** Combined activity, sleep, and heart rate data to form a comprehensive dataset for analysis.

## Exploratory Data Analysis
### Key Analyses:
- **Distribution Analysis:** Analyzed the distribution of daily steps to understand user activity patterns.
- **Correlation Analysis:** Generated a heatmap to explore correlations between metrics like `TotalSteps`, `Calories`, `TotalMinutesAsleep`, and `AvgHeartRate`.
- **Activity Trends:** Investigated how activity levels vary by day of the week and explored the relationship between sleep duration and daily steps.

### Visualizations:
- Distribution of daily steps
- Correlation heatmap of key health metrics
- Average daily steps by day of the week
- Scatterplot of sleep duration vs. daily steps

## Advanced Analysis and Modeling
### Statistical Analysis:
- **Random Forest Regressor:** Developed a model to predict calorie burn with an R-squared score of 0.86, identifying `TotalSteps` as the most significant predictor.
  
### Machine Learning:
- **K-Means Clustering:** Segmented users into three distinct groups based on activity levels and calorie burn, providing a foundation for personalized recommendations.

### Model Evaluation:
- **Model Performance:** Evaluated using Mean Squared Error (MSE) and R-squared metrics.
- **Feature Importance:** Ranked features by their contribution to the model's predictions.

## Key Insights and Findings
- **Activity Patterns:** Users are most active on Tuesdays and least active on Sundays, with an average daily step count of 7638.
- **Sleep Insights:** The average sleep duration is approximately 7 hours, with a weak negative correlation between sleep duration and physical activity.
- **User Segments:** Identified three user segments: High Activity, Moderate Activity, and Low Activity groups.
- **Device Engagement:** A significant proportion of users track sleep (74%) and heart rate (88%), indicating high engagement with these features.

## Strategic Recommendations
### Product Development:
- **Enhance Sleep Tracking:** Improve sleep-related features in the Leaf tracker to address the weak correlation between sleep and activity.
- **Personalized Goals:** Introduce customizable activity goals in the Time watch, tailored to user segments identified through clustering.
- **Integrated Hydration Tracking:** Fully integrate hydration tracking in the Spring water bottle with the Bellabeat app, creating a seamless user experience.

### Marketing Strategy:
- **Segmented Campaigns:** Develop targeted marketing campaigns for distinct user segments (e.g., "Weekend Warriors" for less active users).
- **Holistic Health Messaging:** Position Bellabeat products as holistic wellness tools that integrate activity, sleep, and hydration data.
- **Content Marketing:** Create educational content around the predictors of calorie burn and the benefits of balanced activity.

### User Engagement:
- **Gamification:** Implement a gamified experience in the Bellabeat app to increase user engagement, particularly on less active days.
- **Personalized Insights:** Leverage data insights to offer personalized recommendations, enhancing the user experience.

## Implementation Roadmap
### Short-term (0-3 months):
- Update the Bellabeat app with personalized insights and basic gamification features.
- Launch marketing campaigns targeted at identified user segments.

### Medium-term (3-6 months):
- Enhance sleep tracking features in the Leaf tracker.
- Develop and test hydration tracking integration in the Spring bottle.

### Long-term (6-12 months):
- Fully integrate hydration tracking into the Bellabeat ecosystem.
- Introduce advanced gamification and social features to increase user engagement.

## Success Metrics
- **User Growth:** Achieve a 25% increase in daily active users within 6 months.
- **User Retention:** Improve retention rates from 60% to 75% over the next year.
- **Market Share:** Expand Bellabeat's market share in the women's wellness technology sector by 10% within 12 months.
- **User Engagement:** Increase average daily engagement time with Bellabeat products from 30 to 45 minutes.

## Technical Summary
### Skills and Tools:
- **Python:** Used for data cleaning, feature engineering, and analysis.
- **Pandas & NumPy:** For data manipulation and transformation.
- **Matplotlib & Seaborn:** For visualizing data trends and patterns.
- **Scikit-learn:** For building machine learning models, including Random Forest and K-Means clustering.



