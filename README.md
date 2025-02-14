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
  - [Model Performance](#model-performance)
  - [Confusion Matrix Analysis](#confusion-matrix-analysis)
  - [Conclusion](#conclusion)
- [License](#license)
- [Contributors](#contributors)

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
![1](https://github.com/user-attachments/assets/1ec28a4c-aa56-41ce-8bc2-6b129e3e40ed)
![image](https://github.com/user-attachments/assets/60462f2b-f0ec-4763-b5d1-6a24e725eeb6)
- **Age vs Purchase**: Customers aged 26-35 years contributed the most to sales.
  - ![image](https://github.com/user-attachments/assets/e5ddd732-7e03-43b8-914c-7b8a1e3ac70c)
- **Occupation vs Purchase**: Occupation category "4" had the highest number of purchases.
  - ![image](https://github.com/user-attachments/assets/2ca3e1c0-face-4eb4-b3a6-b51907ceac37)
- **City Category vs Purchase**: Most customers were from city category B.
  - ![image](https://github.com/user-attachments/assets/a97ba5a5-89ca-4963-804a-f6f5ea9f1dde)
- **Product Category Analysis**:
  - In product category 1, Product 5 had the highest sales, followed by Products 8 and 19.
    - ![image](https://github.com/user-attachments/assets/5b73266c-f392-438f-a6a4-a0d9cba23f3d)
  - Product 8 was the most purchased in category 2.
    - ![image](https://github.com/user-attachments/assets/79c12e16-aec5-4921-9b17-bdd5d970dae0)
  - Product 16 dominated sales in category 3.
    - ![image](https://github.com/user-attachments/assets/4451b5f9-8fc6-46f4-848a-9f001ab3399b)
These insights are valuable for targeting specific customer groups with personalized offers.

## Predictive Modeling

### Linear Regression
A linear regression model was applied to predict total purchase amount based on various customer and product features. However, this model showed limited predictive power due to the complexity of the relationships in the dataset.

### Random Forest Regression
A random forest regression model provided a significantly better fit, explaining **63.38%** of the variance in the response variable. The model achieved a **mean squared residual** of **8,729,361**, indicating a reasonably good fit. Random Forest outperformed linear regression in predicting customer purchase behavior.

## Results and Discussion

### Model Performance
Our results indicate that **Random Forest Regression** performed better than **Linear Regression** for predicting customer purchase behavior. The Random Forest model explained approximately **63.38%** of the variance in the data, which is a good fit, considering the complexity of the dataset. The R-squared value of **0.6275** suggests that the model captures important trends in the data.

### Conclusion
The combination of **Random Forest Regression** and **EDA** provides useful insights into customer behavior and purchasing patterns. Our analysis demonstrates that creating targeted offers for male customers aged **26-35**, particularly for products from categories 1, 2, and 3, can significantly increase sales in future months. Although the Random Forest model explains a good portion of the variance, there are still factors that could be explored in future studies to further enhance prediction accuracy.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributors
- **Steve Marcello Liem**
- **Davin Edbert Santoso Halim**
- **Felicia Andrea Tandoko**
