# customer-churn-analysis
Customer Churn Analysis and Prediction using Machine Learning

This project focuses on predicting customer churn using machine learning and visualizing insights through an interactive Tableau dashboard.
The objective is to identify customers who are likely to leave the service and understand the key factors influencing churn. Churn probability represents the likelihood of a customer discontinuing the service based on their attributes.

DATASET
The dataset used is the Telco Customer Churn dataset from Kaggle. It represents a telecom service provider, but it is anonymized and not tied to a specific company
It contains customer information such as:
- Demographics (gender, senior citizen)
- Services (internet, phone, streaming)
- Billing details (monthly charges, total charges)
- Contract type
- Target variable: Churn (Yes/No)

DATA PREPROCESSING

- Converted TotalCharges to numeric and handled missing values
- Converted Churn column to binary (1 = churn, 0 = no churn)
- Removed irrelevant features like customerID
- Applied one-hot encoding to categorical variables

MODEL USED

Logistic Regression was used for churn prediction due to its simplicity and effectiveness for binary classification problems.

MODEL EVALUATION

The model achieved approximately:
- Accuracy: ~73%
- Balanced recall for churn prediction using class_weight='balanced'

Key Features Engineered

- Churn Probability: Probability of customer leaving
- Risk Level: Categorized into Low, Medium, High based on probability

Tableau Dashboard

Dashboard includes:
- KPI Cards (Total Customers, Churn Rate, High Risk Customers)
- Churn by Contract Type
- Churn by Payment Method
- Monthly Charges vs Churn Probability
- Customer Risk Segmentation

Key Insights

- Customers with month-to-month contracts have the highest churn rate
- Electronic check users are more likely to churn
- Higher monthly charges are associated with higher churn probability
- The model effectively identifies high-risk customers for targeted retention

Business Impact

This project helps businesses:
- Identify customers at risk of churn
- Understand key drivers of churn
- Take proactive retention measures such as targeted offers or contract upgrades

Technologies Used

- Python (Pandas, NumPy, Scikit-learn)
- Machine Learning (Logistic Regression)
- Tableau (Data Visualization)
- Jupyter Notebook

Dashboard insights

-Contract type reflects customer commitment level, and customers with shorter contracts showed higher churn rates.

<img width="719" height="720" alt="image" src="https://github.com/user-attachments/assets/c3a2ffa4-fde0-4858-bf35-a91782b28f3c" />

-Electronic check users showed higher churn because they are typically less committed customers, often on flexible plans, and not enrolled in automatic payments, making it easier for them to discontinue the service.

<img width="719" height="720" alt="image" src="https://github.com/user-attachments/assets/0ad2526b-a366-4cfa-9a91-63b26d78ffb5" />

-The scatter plot visualizes the relationship between monthly charges and churn probability, showing that customers with higher charges tend to have a higher likelihood of churning.

<img width="775" height="720" alt="image" src="https://github.com/user-attachments/assets/a4479b05-1a02-45cf-b56f-3b6cf4e74850" />

-Risk segmentation groups customers based on how likely they are to churn. Customers are segmented into low, medium, and high risk based on churn probability, enabling businesses to prioritize retention strategies effectively.

<img width="775" height="720" alt="image" src="https://github.com/user-attachments/assets/817c7d82-ae03-4e7b-81df-811adb346d66" />

DASHBOARD:

<img width="969" height="786" alt="image" src="https://github.com/user-attachments/assets/1c2ffafb-bd2b-4c80-9481-af9b968b2ac1" />



