# Diamond Price Prediction

## Introduction
Welcome to my Diamond Price Prediction project, an ambitious endeavor leveraging the power of data science and machine learning to unravel and predict diamond prices. Diamonds, with their timeless allure and significant economic value, are priced based on a complex interplay of characteristics. This project seeks to demystify these variables and build a predictive model that accurately forecasts the price of diamonds based on their distinct features.

## Objective
The main objective of this project is to develop a predictive model capable of accurately estimating the price of diamonds. This model is intended not just as an academic exercise but as a practical tool that can be utilized by various stakeholders in the diamond industry, such as retailers, appraisers, and customers, to understand and predict diamond prices effectively.

## Data Set
The dataset can be obtained on Kaggle: https://www.kaggle.com/datasets/nancyalaswad90/diamonds-prices/data

- **Carat Weight:** The most significant factor in diamond pricing, representing the diamond's weight and indirectly its size.

- **Cut Quality:** This qualitative measure affects a diamond's symmetry and proportions, influencing its brilliance and overall appearance.

- **Color Grade:** A rating that reflects the absence of color in diamonds, with a scale that ranges from colorless to light yellow or brown.

- **Clarity Grade:** Indicates the presence or absence of inclusions and blemishes, impacting the diamond's purity and brilliance.

- **Additional Features:** Measurements like depth percentage, table percentage, and physical dimensions (length x width x depth) also play a role in valuation.

## Methodology

The project is structured into distinct phases:

1. **Data Preprocessing and Cleaning:** Ensuring data quality by handling missing values, outliers, and errors, making the dataset ready for analysis.

2. **Exploratory Data Analysis (EDA):** A deep dive into the dataset using statistical analysis and visualization techniques to identify patterns, correlations, and insights into how different features affect diamond prices.

3. **Feature Engineering:** Enhancing model performance by creating new features, transforming existing ones, and selecting the most relevant features for predicting diamond prices.

4. **Model Building and Selection:** Experimenting with various machine learning algorithms, such as linear regression, log linear regression, log log regression, and gradient boosting machines, to identify the model that best fits our data.

5. **Model Evaluation and Validation:** Rigorously testing the model using metrics like Mean Squared Error (MSE), Mean Absolute Percentage Error (MAPE), and cross-validation to assess its accuracy and robustness.

6. **Optimization and Fine-tuning:** Adjusting model parameters and employing techniques like grid search to enhance the model's performance.

## Results

Key highlights from our results include:

- **Model Performance:** The best-performing model achieved a Mean Absolute Percentage Error (MAPE) of 7.42%. This indicates a high level of precision in price prediction.
- **Feature Importance:** Analysis revealed that features such as the y dimension of the diamond, carat weight, and clarity grade had the most significant impact on the diamond price.
- **Comparative Analysis:** The XGboost model outperformed other models like linear regression, log linear regression, and log log regression in terms of performance metrics.

![Correlation Heatmap](https://github.com/nickyongth/images-/blob/main/correlationheatmapdiamonds.png)
