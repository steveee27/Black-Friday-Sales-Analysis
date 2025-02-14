# Black Friday Sales Analysis

## Table of Contents
- [Introduction](#introduction)
- [Dataset Overview](#dataset-overview)
- [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Predictive Modeling](#predictive-modeling)
  - [Linear Regression](#linear-regression)
  - [Random Forest Regression](#random-forest-regression)
- [Results and Discussion](#results-and-discussion)
- [Conclusion](#conclusion)
- [License](#license)

## Introduction

The Black Friday Sales Analysis project is designed to help "ABC Private Limited" understand customer behavior through detailed analysis of customer demographics, purchasing patterns, and product categories based on the Black Friday dataset. Using exploratory data analysis (EDA) and predictive modeling, we aim to guide ABC Private Limited in creating offers that can boost their sales in upcoming months.

## Dataset Overview

The dataset contains information on **550,000** customers, including:
- **Customer demographics**: Age, gender, marital status, city type, and years of stay in the current city.
- **Product details**: Product ID and category.
- **Total purchase amount**.

This data was used to analyze customer purchasing behavior across various product categories and demographics to generate useful business insights.

## Data Cleaning and Preprocessing

Before analysis, the dataset underwent the following preprocessing steps:
- **Removing irrelevant columns**: Unnecessary columns were discarded.
- **Handling missing data**: Missing values were handled using appropriate strategies such as imputation.
- **Feature encoding**: Categorical variables were converted into numerical values using one-hot encoding.
- **Normalization**: Numerical features were normalized to ensure consistency across models.

## Exploratory Data Analysis

Through EDA, we uncovered several key patterns in customer purchase behavior:
- **Gender vs Purchase**: Male customers visited the store more frequently and made more purchases than female customers.
- **Age vs Purchase**: Customers aged 26-35 years contributed the most to sales.
- **Occupation vs Purchase**: Occupation category "4" had the highest number of purchases.
- **City Category vs Purchase**: Most customers were from city category B.
- **Product Category Analysis**:
  - In product category 1, Product 5 had the highest sales, followed by Products 8 and 19.
  - Product 8 was the most purchased in category 2.
  - Product 16 dominated sales in category 3.

These insights are valuable for targeting specific customer groups with personalized offers.

## Predictive Modeling

### Linear Regression

A linear regression model was applied to predict total purchase amount based on various customer and product features. However, this model showed limited predictive power due to the complexity of the relationships in the dataset.

### Random Forest Regression

A random forest regression model provided a significantly better fit, explaining **63.38%** of the variance in the response variable. The model achieved a **mean squared residual** of **8,729,361**, indicating a reasonably good fit. Random Forest outperformed linear regression in predicting customer purchase behavior.

## Results and Discussion

The predictive models demonstrate that **Random Forest Regression** is the most accurate model for predicting customer purchases. The **R-squared value** of **0.6275** indicates a reasonable fit, suggesting that the model captures significant patterns in the data. However, there are other influencing factors not considered in this analysis that could improve model performance.

- **Business Recommendations**:
  Based on the analysis, we recommend creating offers like **discounts** for top-selling products in categories 1, 2, and 3, specifically targeting male customers aged **26-35**. This approach is expected to drive more foot traffic and boost sales in the next months.

## Conclusion

This project provides valuable insights into customer behavior and highlights the potential for ABC Private Limited to increase sales by offering targeted promotions. The combination of EDA and predictive modeling can help the company understand its customer base better and tailor future marketing strategies accordingly.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
