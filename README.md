

# Customer Satisfaction Prediction

This project involves building a machine learning model to predict customer satisfaction scores based on various demographic, behavioral, and product/service quality factors. The goal is to help businesses better understand and forecast customer satisfaction, allowing for data-driven decisions to improve products, services, and overall customer experience.


## **Project Overview**
The Customer Satisfaction Prediction model uses features like Age, Income, Product Quality, Service Quality, and Purchase Frequency to predict customer satisfaction scores. This predictive model can help businesses enhance their customer service by identifying areas for improvement and proactively addressing customer dissatisfaction.

---

## **Dataset Description**
The dataset contains the following columns:
- **CustomerID**: Unique identifier for each customer.
- **Age**: Age of the customer.
- **Income**: Annual income of the customer.
- **ProductQuality**: Rating of the product quality (1 to 10).
- **ServiceQuality**: Rating of the service quality (1 to 10).
- **PurchaseFrequency**: Number of purchases per year.
- **SatisfactionScore**: Target variable, satisfaction score (1 to 100).

---

## **Data Preprocessing**
1. **Handling Missing Values**: Missing values are filled using the mean of the respective columns.
2. **Feature Selection**: The `CustomerID` column is dropped as it does not contribute to the model's prediction.
3. **Scaling**: The features are normalized using `StandardScaler` to ensure uniformity across different feature ranges.
4. **Train-Test Split**: Data is split into training and test sets using an 80-20 ratio.

---

## **Model Development**
Two machine learning models were trained to predict the **SatisfactionScore**:
1. **Linear Regression**: A baseline model to predict satisfaction based on linear relationships between features and target.
2. **Random Forest Regressor**: A more advanced model that captures non-linear relationships between the features.

---

## **Model Evaluation**
The models were evaluated using the following metrics:
- **Mean Absolute Error (MAE)**: Measures the average magnitude of errors in predictions.
- **Mean Squared Error (MSE)**: Measures the average of the squared differences between predicted and actual values.
- **R² Score**: Represents the proportion of the variance in the target variable explained by the model.

**Results:**
- **Linear Regression**:
  - MAE: 7.38
  - MSE: 84.88
  - R²: 0.697
- **Random Forest Regressor**:
  - MAE: 5.70
  - MSE: 65.73
  - R²: 0.765

The **Random Forest Regressor** outperformed the **Linear Regression** model with better accuracy and a higher R² score.

---
