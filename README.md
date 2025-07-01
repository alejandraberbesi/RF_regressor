**Regression Modeling Pipeline (2021)**

This project showcases a data preprocessing pipeline for a regression task. 

🧱 1. Data Source

* Loaded from Google Drive: dataset_test.txt

* 1000 rows, 11 columns (mixed types: categorical, numerical, dates)

🧹 2. Data Cleaning

* Replaced 'na' strings with NaN

* Dropped rows with missing label or disc_6 values (critical for model)

* Removed outliers from cont_3, cont_4, and label using IQR method

* Resulting dataset: 789 rows

🔍 3. Preprocessing

* Converted disc_6, disc_5, and label to numeric types

* Transformed date_2 to datetime

* Encoded categorical variables cat_7 and cat_8 using LabelEncoder

* Dropped cont_10 due to high correlation with cont_9 (r ≈ 0.99)

📈 4. EDA Insights

* Detected outliers via boxplots

* Categorical variable distributions visualized

* Verified no duplicate rows after cleaning

* Final selected features: cont_3, cont_4, disc_5, disc_6, cat_7, cat_8, cont_9
