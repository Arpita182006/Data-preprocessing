# Data-preprocessing

🔧 Data Preprocessing & Encoding in Machine Learning
📌 Overview
This project demonstrates various data preprocessing techniques commonly used in machine learning workflows. These include handling missing values, encoding categorical variables, feature scaling, and preparing data for model training.

 
📊 Dataset 1: data.csv
✅ Features:
Country (Categorical)

Age (May contain missing values)

Salary (May contain missing values)

Purchased (Target column - Yes/No)


🧪 Steps Performed
1. Handling Missing Values
Used SimpleImputer from sklearn.impute to replace missing values in Age and Salary with the mean of the column.

2. One-Hot Encoding (for Country)
Applied OneHotEncoder to convert the categorical Country column into multiple binary columns (Country_France, Country_Germany, Country_Spain).

Used get_feature_names_out to retrieve the encoded column names.

3. Label Encoding (for Purchased)
Used LabelEncoder to convert the Purchased column (Yes/No) into numerical values (0/1).

4. Feature Scaling
Standardized Age and Salary using StandardScaler to bring all values to the same scale (mean = 0, std = 1).

5. Data Splitting
Split the final dataset into training and testing sets using train_test_split.


📊 Dataset 2: Customer Satisfaction (Manual Sample Data)
✅ Features:
CustomerID

Education_Level

Product_Quality

Satisfaction_Level

Steps Performed:
Defined ordinal relationship between values (e.g., High_School < Bachelors < Masters < phD)

Used OrdinalEncoder from sklearn.preprocessing to convert ordered categories into numerical values, preserving the rank.


📦 Libraries Used
pandas

numpy

scikit-learn


📁 Project Structure
kotlin
Copy
Edit
data_preprocessing_project/
│
├── data.csv
├── customer_data.csv (optional sample data)
├── preprocessing_script.py
└── README.md  ← (this file)
📚 Learning Outcome
This project is useful for understanding real-world data cleaning and transformation techniques. These are foundational steps required before training any machine learning model.

