📊 Student Performance – Exploratory Data Analysis (EDA)
📌 Project Overview

This project performs Exploratory Data Analysis (EDA) on a Student Performance dataset to understand the factors that influence students’ academic performance.
The analysis uses Python, Pandas, Matplotlib, and Seaborn to identify patterns, trends, relationships, and anomalies in the data.

🎯 Objectives

The main objectives of this EDA project are:

To understand the structure and quality of the dataset

To identify key factors affecting student performance

To detect missing values, duplicates, and outliers

To analyze relationships between academic, lifestyle, and performance variables

To validate basic statistical assumptions using visualizations

📂 Dataset Description

The dataset contains information related to students’ academic background and habits.

🔑 Columns Used:
Column Name	Description	Data Type
Previous Score	Student’s previous academic score	Numerical
Extracurricular Activities	Participation in extracurricular activities (Yes/No)	Categorical
Sleep Hours	Average sleep hours per day	Numerical
Sample Question Papers Practiced	Number of practice papers solved	Numerical
Performance Index	Overall performance score	Numerical (Target Variable)
🛠️ Tools & Libraries

Python

Pandas

NumPy

Matplotlib

Seaborn

🔍 Exploratory Data Analysis Steps
1️⃣ Data Understanding

Dataset shape (rows & columns)

Data types and column meanings

Summary statistics

2️⃣ Data Cleaning

Missing value detection

Duplicate row identification

Data consistency checks

3️⃣ Univariate Analysis

Distribution of numerical variables using histograms

Frequency analysis of categorical variables

4️⃣ Outlier Detection

Box plots used to detect extreme values

5️⃣ Bivariate Analysis

Correlation analysis between numerical variables

Group-wise comparison using categorical variables

6️⃣ Hypothesis Testing & Assumption Validation

Mean comparison across categories

Correlation coefficient analysis

Normality and linearity checks using visualizations

📈 Sample Analysis Code
Group-wise Mean Analysis
df.groupby('Extracurricular Activities')['Performance Index'].mean()

Correlation Analysis
df['Sleep Hours'].corr(df['Performance Index'])

Distribution Check
sns.histplot(df['Performance Index'], kde=True)
plt.show()

Linearity Check
sns.regplot(x='Sleep Hours', y='Performance Index', data=df)
plt.show()

📊 Key Insights

Students with extracurricular activities show variation in performance

Sleep hours and previous scores have a noticeable relationship with performance

Outliers are present and can affect modeling results

Data is suitable for further statistical analysis and predictive modeling

🚀 Conclusion

This EDA provides a strong foundation for:

Feature selection

Predictive modeling

Academic performance analysis

The insights gained help understand how study habits and lifestyle factors influence student outcomes.


👤 Author

Yogesh S
Aspiring Data Analyst
📌 Skills: Python, Data Analysis, EDA, Visualization
