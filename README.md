Here’s a clean, professional **README.md** file for your GitHub project:

---

#  Sales Prediction System using Machine Learning

##  Project Overview

The **Sales Prediction System** is a machine learning project designed to predict total sales based on product, pricing, and time-based features.
It helps businesses understand key factors influencing sales and improve decision-making through data-driven insights.

---

##  Problem Statement

Organizations often face challenges such as:

* Fluctuating sales performance
* Inefficient pricing strategies
* Lack of insights into customer purchasing behavior

This project aims to build a predictive model to estimate **Total Sales** using historical transaction data.

---

##  Objectives

* Predict total sales accurately
* Identify key factors affecting sales (price, quantity, discount, etc.)
* Build and compare machine learning models
* Provide business insights for better decision-making

---

##  Dataset Information

###  Target Variable

* `Total_Sales`

###  Input Features

* Product_Price
* Quantity
* Discount
* Region
* City
* Product_Category
* Payment_Method
* Order_Date (split into Year, Month, Day)

---

##  Data Preprocessing

###  Data Cleaning

* Missing values handled:

  * Discount → filled with 0
  * Product_Price → median imputation
  * Quantity → median imputation
* Duplicate records checked and removed
* Outliers handled using **IQR / Z-score method**

###  Feature Engineering

* Extracted Year, Month, Day from Order_Date
* One-Hot Encoding for categorical variables
* Removed redundant columns:

  * Total_Before_Discount
  * Discount_Amount

---

##  Exploratory Data Analysis (EDA)

###  Univariate Analysis

* Distribution of Product_Price, Quantity, Discount, Total_Sales

###  Bivariate Analysis

* Price vs Sales
* Quantity vs Sales
* Category vs Sales
* Region vs Sales

###  Key Insights

* Quantity is the strongest driver of sales
* Product price has moderate impact
* Discounts have limited influence
* Sales are volume-driven rather than price-driven

---

##  Machine Learning Models

### Models Used:

1. Linear Regression (Baseline Model)
2. Decision Tree Regressor
3. Random Forest Regressor

---

##  Model Training

* Dataset split: **80% training / 20% testing**
* Training performed using sklearn models

---

##  Evaluation Metrics

* MAE (Mean Absolute Error)
* MSE (Mean Squared Error)
* RMSE (Root Mean Squared Error)
* R² Score

---

## Model Performance Summary

| Model             | MAE | RMSE | R² Score           |
| ----------------- | --- | ---- | ------------------ |
| Linear Regression | ✔   | ✔    | ✔ Good             |


---

##  Final Model Selection

**Best Model:** Random Forest Regressor

### Reason:

* Highest accuracy (R² score)
* Better handling of non-linear relationships
* Lower prediction error

---

##  Key Insights

* Quantity strongly impacts total sales
* Pricing strategy significantly influences revenue
* Regional differences affect sales performance
* Product categories show varying demand patterns

---

##  Business Recommendations

1. Optimize pricing strategy based on demand
2. Apply targeted discounts instead of random offers
3. Focus on high-performing regions and categories
4. Improve inventory planning using sales trends

---

##  Future Improvements

* Implement advanced models like XGBoost / LightGBM
* Hyperparameter tuning for better accuracy
* Deploy using Flask / FastAPI
* Build real-time sales dashboard
* Add customer behavior data for deeper insights

---

##  Technologies Used

* Python 
* Pandas & NumPy
* Matplotlib & Seaborn
* Scikit-learn
* Machine Learning Models

---

##  Conclusion

This project demonstrates how machine learning can be used to predict sales effectively and extract meaningful business insights. It helps organizations make data-driven decisions to improve revenue and efficiency.


