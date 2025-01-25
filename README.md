# Insights from Supermarket Sales Data: Regression and Classification Approaches

## Project Overview
This project focuses on analyzing supermarket sales data to uncover key insights and develop predictive models. It incorporates data preprocessing, visualization, regression, and classification techniques to explore the relationships between various features and target variables such as gross income, unit price, gender, customer type, and day-of-purchase.

## Purpose
The primary goals of this project are:
1. To preprocess and analyze supermarket sales data.
2. To build predictive models for gross income, unit price, gender classification, customer type classification, and purchase day prediction.
3. To uncover significant relationships and patterns in the data for actionable insights.

## Methods Used
1. **Data Preprocessing**:
   - Converted the `Date` attribute into the day of the week and segmented `Time` into morning, afternoon, evening, and night.
   - Removed redundant features like `Invoice ID` and constant-value attributes.
   - Applied standard scaling for numerical features and one-hot encoding for categorical attributes.
   - Used ordinal encoding for target variables in classification tasks.

2. **Regression Techniques**:
   - Multiple linear regression with and without Lasso regularization for predicting gross income and unit price.
   - Hyperparameter tuning using grid search for optimal regularization parameters.

3. **Classification Techniques**:
   - Logistic regression for gender and customer type classification.
   - Multi-class logistic regression and random forest classifier for predicting the day of purchase.

## Insights from the Data
1. **Gross Income**:
   - Positive impact of features like quantity, unit price, and certain days (Tuesday, Thursday, Saturday).
   - Afternoon and evening time slots showed higher gross income contributions.

2. **Unit Price**:
   - Higher gross income positively correlates with higher unit prices.
   - Increased quantity resulted in reduced unit price (bulk discounts).

3. **Gender Classification**:
   - Certain product combinations (e.g., fashion accessories purchased on Saturday or evenings) influenced gender prediction.

4. **Customer Type Classification**:
   - Specific product and time combinations, such as health and beauty products purchased on Fridays, were significant.

5. **Day-of-Purchase Prediction**:
   - Both logistic regression and random forest classifiers were tested. While logistic regression underperformed, random forest classifiers overfitted on training data, indicating the need for better generalization.

## Machine Learning Techniques
- **Linear Regression**:
  - Applied for gross income and unit price predictions with Lasso regularization.
- **Logistic Regression**:
  - Used for binary classification tasks (gender and customer type).
  - Polynomial feature interactions (degree 2) were added for improved performance.
- **Random Forest Classifier**:
  - Employed for multi-class classification of purchase days.
- **Grid Search**:
  - Conducted for hyperparameter tuning across models.

## Key Results
1. **Regression Models**:
   - Achieved high R² scores for gross income and unit price prediction, indicating strong predictive performance.

2. **Classification Models**:
   - Gender and customer type classification showed moderate accuracy with key feature combinations highlighted.
   - Day-of-purchase prediction models revealed overfitting and underfitting issues, requiring further optimization.

## Conclusion
This project demonstrates the application of regression and classification techniques to derive actionable insights from supermarket sales data. While regression models performed well in predicting numerical outcomes, classification models highlighted the importance of feature engineering and model optimization. The findings can inform marketing strategies and operational decisions for supermarkets.



