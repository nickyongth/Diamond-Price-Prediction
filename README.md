# Diamond Price Prediction

[Diamond](https://github.com/nickyongth/images-/blob/main/Blue%20Diamonds.png)

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

## Visualizations

### Correlation Heatmap
![Correlation Heatmap](https://github.com/nickyongth/images-/blob/main/correlationheatmapdiamonds.png)

This heatmap provides a visual representation of the Pearson correlation coefficients between various features related to diamonds and their prices. This is essential for understanding the relationships between the features of diamonds and can guide feature selection and engineering for predictive modeling.

Observations:
- The `carat` size shows a strong positive correlation with price, which is in line with the understanding that larger diamonds are generally more valuable.
- The dimensions of the diamond (`x`, `y`, `z`) are highly correlated with each other, suggesting that diamonds with larger dimensions are typically heavier.
- There's a notable positive correlation between `carat` and the dimensions, indicating that as diamonds get heavier, they generally increase in size.
- Depth and table show less significant correlations with price, suggesting they may have a subtler effect on a diamond's value.

### Log of Carat Weight vs. Log of Price by Color Grade
![Log of Carat Weight vs. Log of Price by Color Grade](https://github.com/nickyongth/images-/blob/main/logcaratweightvslogpricebycolorgrade.png)

The scatter plot transforms the carat weight and price data using a logarithmic scale, reducing skewness and allowing for better visualization of the relationship between these variables across different color grades. Points are colored according to the diamond's color grade, providing insight into how color impacts the price relative to the carat weight.

Observations:
- There is a clear positive trend, indicating that as the carat weight increases, the price tends to increase as well, even on a logarithmic scale.
- The data spread suggests variability in price increases with higher carat weights, across all color grades.
- Diamonds of different color grades largely overlap in price ranges, implying that while color is a factor, carat weight is a dominant predictor of price on a logarithmic scale.

### Feature Importance with SHAP Values
![Feature Importance with SHAP Values](https://github.com/nickyongth/images-/blob/main/shapdiamonds.png)

This bar chart depicts the average impact of each feature on the model's output as measured by SHAP values. The mean absolute value of the SHAP values for each feature is shown, indicating the strength and significance of the feature's effect on the predictive model's price estimation. Understanding the influence of each feature helps in refining the model for better accuracy and offers insights into the aspects of diamonds that most strongly affect their market price.

Observations:
- The `y` dimension is shown to have the highest average SHAP value, suggesting a strong influence on the model's output.
- Carat weight follows closely, reaffirming its known importance in determining diamond prices.
- Other attributes like clarity, color, and additional dimensions (`z`, `x`) are also influential, though to a lesser extent than the `y` dimension and carat weight.
