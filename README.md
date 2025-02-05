
# Bike Sharing Assessment

BoomBikes, a US bike-sharing provider, has experienced a drop in revenue due to the COVID-19 pandemic and aims to recover once the economy stabilizes. To prepare, they have contracted a consulting company to identify the key factors influencing bike demand in the American market. The goal is to understand which variables significantly impact demand for shared bikes and how well these factors can predict future demand. The company has collected a large dataset on daily bike usage based on various factors, including weather and people's preferences.

## Table of Contents

1. [General Information](#general-information)
2. [Business Objective](#business-objective)
3. [Dataset Description](#dataset-description)
4. [Methodolody](#methodology)
5. [Conclusions](#conclusions)
6. [Technologies Used](#technologies-used)
7. [Acknowledgement](#acknowledgements)
8. [Contact](#contacts)
## General Information

The goal is to build a model that predicts the demand for shared bikes based on various independent variables. This model will help management understand how different factors influence demand, allowing them to adjust their business strategies accordingly to meet customer expectations. Additionally, the model can serve as a useful tool for assessing demand dynamics in new markets.
## Business Objective

The primary objectives of this project are:

1.Predict Bike Demand: Build a model to predict total bike demand (cnt) based on factors like weather, season, and year.

2.Identify Key Factors: Determine which variables most influence bike demand to guide business decisions.

3.Optimize Strategy: Use the model to adjust marketing, pricing, and operations based on demand variations.

4.Support Expansion: Utilize the model to understand demand dynamics in new markets for informed expansion decisions.

5.Annual Growth Insights: Analyze yearly trends (e.g., 'yr' variable) to plan for seasonal growth and future capacity.
## Methodology

### Data Preparation:

1. Handle Missing Values: Ensure there are no missing values in the dataset. If present, either impute or drop the rows/columns.
2. Convert Categorical Features: Convert categorical variables like 'season', 'weathersit', and 'yr' into categorical string values or use one-hot encoding.
3. Feature Scaling: Normalize continuous variables (e.g., temp, humidity, windspeed) to bring them to a similar scale for better model performance.

### Feature Selection:

1. Identify and select the independent variables that might impact bike demand. These could include weather, season, weekday, temperature, windspeed, etc.
2. Drop irrelevant features or ones with high multicollinearity (e.g., atemp and temp if they are highly correlated).

### Train-Test Split:

Split the data into training and testing sets, typically 70-30 or 80-20, to validate the model's performance on unseen data.

### Model Building:

1. Use Linear Regression to model the relationship between independent variables and the target variable 'cnt' (total bike rentals).
2. Fit the model using the training data and evaluate performance on the test set.

### Model Evaluation:

1. Evaluate the model using R-squared (R²) to assess how well the independent variables explain the variance in bike demand.
2. Perform residual analysis (e.g., Q-Q plot, residual plots) to check for assumptions like linearity, homoscedasticity, and normality.

### Model Interpretation:

Review the coefficients of the linear model to understand the impact of each feature on bike demand.
Identify significant predictors (those with a high absolute value of coefficients or low p-values).
## Conclusions

1. BoomBikes rentals is majorly affected by temperature, season, weather and month.
2. The demand for bikes was more in 2019 than 2018.
B3. oomBikes rentals must focus more on Summer & Winter season and September month as they have good influence on bike rentals. They must increase their bike availibilty and promotions to further increase their rental count.
4. Cloudy and Light Rain weather has negative coefficients. To increase the demand, offers must be introduced
5. Holidays has negative coefficient. It would be great to provide offers on holidays.
## Technologies Used

1. Pandas 
2. NumPy 
3. MatplotLib 
4. Seaborn
5. Statsmodel
6. Scikit Learn
## Acknowledgements

This project was created as a case study for IITB Machine Learning and AI program.

## Contact

Created by [@rutujajadhav2890](#@rutujajadhav2890) - feel free to contact me!
