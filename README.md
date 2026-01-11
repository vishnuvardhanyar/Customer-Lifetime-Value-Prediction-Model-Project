# Customer-Lifetime-Value-Prediction-Model-project
📊 Customer Lifetime Value (LTV) Prediction Model



📌 Project Overview

Customer Lifetime Value (LTV) represents the total revenue a business can expect from a customer over the entire duration of their relationship.
This project aims to predict Customer LTV using purchase behavior data and segment customers to support targeted marketing strategies.

🎯 Objective

Predict Customer Lifetime Value (LTV) based on historical purchase behavior

Identify high-value, medium-value, and low-value customers

Help businesses focus marketing efforts on profitable customers

🛠 Tools & Technologies Used

Python

Pandas & NumPy – Data preprocessing and feature engineering

Scikit-learn – Machine learning (Random Forest Regression)

Matplotlib – Data visualization

Excel – Data understanding and optional analysis

📂 Dataset Description

File: customer_transactions.csv

Columns:

customerid – Unique customer identifier

orderdate – Date of purchase

amount – Purchase amount

The dataset contains multiple transactions per customer, which helps in calculating behavioral metrics.

🔧 Project Workflow



1️⃣ Data Preprocessing

Loaded transaction data

Converted date columns to datetime format

Grouped transactions by customer ID

2️⃣ Feature Engineering

Created the following features:

Recency – Days since the last purchase

Frequency – Number of purchases made

AOV (Average Order Value) – Average amount spent per order

3️⃣ LTV Calculation

A simple LTV formula was used:

LTV = Frequency × AOV


This value is used as the target variable for model training.

4️⃣ Model Building

Trained a Random Forest Regressor

Input features: Recency, Frequency, AOV

Output: Predicted Customer LTV

5️⃣ Model Evaluation

The model was evaluated using:

MAE (Mean Absolute Error)

RMSE (Root Mean Squared Error)

Lower values indicate better prediction accuracy.

6️⃣ Customer Segmentation

Customers were segmented into:

Low Value

Medium Value

High Value

Segmentation was based on predicted LTV using quantiles.

7️⃣ Visualization

Bar chart showing customer distribution across LTV segments

📁 Deliverables

📓 Python Notebook: Model implementation and analysis

📊 Visualizations: Customer segmentation chart

📄 Final Output File: Final_LTV_Predictions.csv containing predicted LTV and customer segments

📈 Business Impact

Helps identify high-value customers

Enables targeted marketing and retention strategies

Improves customer relationship management and revenue planning

✅ Conclusion

This project successfully demonstrates how customer transaction data can be used to predict Customer Lifetime Value using machine learning. The insights gained from LTV prediction and segmentation can significantly enhance marketing efficiency and business decision-making.
