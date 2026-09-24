# 📊 Customer Churn Analysis

An end-to-end **Customer Churn Analysis** project using Python to analyze customer behavior, churn patterns, retention, revenue impact, and customer risk.

---

## 📌 Project Overview

Customer churn is an important business problem for subscription-based companies. Understanding **who is leaving, why they are leaving, and which customer segments are most affected** can help businesses improve customer retention and reduce revenue loss.

In this project, customer, subscription, and support data were analyzed using **Python, Pandas, NumPy, Matplotlib, and Seaborn**.

The project covers the complete analytics workflow:

> **Data Loading → Data Cleaning → Feature Engineering → Exploratory Data Analysis → KPI Analysis → Visualization → Business Insights**

---

## 🎯 Business Objective

The main objective of this project is to understand customer churn and identify the factors and customer segments associated with higher churn.

The analysis focuses on:

- Measuring overall customer churn
- Measuring customer retention
- Understanding churn across different plans
- Analyzing churn across different contract types
- Comparing churn across states
- Analyzing churn by subscription type
- Understanding customer age and tenure
- Analyzing revenue and customer lifetime value
- Identifying customers with higher churn risk
- Understanding the relationship between support activity and churn
- Developing actionable business insights

---

## ❓ Business Questions

The project answers the following questions:

1. What is the overall customer churn rate?
2. What is the overall customer retention rate?
3. Which plan type has the highest churn rate?
4. How does churn vary across different contract types?
5. How does churn vary across different states?
6. How does churn vary by subscription type?
7. What is the average customer age?
8. What is the average customer tenure?
9. What is the average revenue per user (ARPU)?
10. How much revenue is associated with high-risk customers?
11. What are the major cancellation reasons?
12. What is the relationship between customer support escalations and churn?
13. Which customer segments require further investigation?

---

## 🗂️ Dataset

The dataset contains information related to **customers, subscriptions, and customer support**.

### Customer Data

The customer dataset contains fields such as:

- Customer ID
- Customer Name
- Country
- State
- Gender
- Date of Birth
- Interests
- Pincode

### Subscription Data

The subscription dataset contains:

- Customer ID
- Subscription Start Date
- Subscription Type
- Renewal Date
- Plan Type
- Contract Type
- Cancellation Date
- Cancellation Reason
- Monthly Charges
- CLTV
- Churn Score
- Churn Flag

### Support Data

The support dataset contains:

- Customer ID
- Complaint Date
- Escalations
- CSAT Score
- Comments

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Python** | Data analysis and processing |
| **Pandas** | Data cleaning, transformation and analysis |
| **NumPy** | Numerical operations |
| **Matplotlib** | Data visualization |
| **Seaborn** | Statistical visualization |
| **Jupyter Notebook** | Development and analysis environment |
| **Excel** | Source data |

---

## 🔄 Project Workflow

```text
Raw Data
   │
   ▼
Data Loading
   │
   ▼
Data Cleaning
   │
   ├── Data Type Conversion
   ├── Missing Value Handling
   ├── Column Selection
   └── Data Quality Checks
   │
   ▼
Feature Engineering
   │
   ├── Customer Age
   ├── Customer Tenure
   ├── Churn Flag
   └── Churn Risk
   │
   ▼
Exploratory Data Analysis
   │
   ├── Churn Analysis
   ├── Retention Analysis
   ├── Revenue Analysis
   ├── Customer Segmentation
   └── Support Analysis
   │
   ▼
Data Visualization
   │
   ▼
Business Insights
   │
   ▼
Business Recommendations
```

---

## 🧹 Data Cleaning

The following data-cleaning activities were performed:

- Checked the structure of the dataset
- Inspected data types
- Converted date columns into appropriate datetime format
- Selected relevant columns
- Checked for missing values
- Handled null values
- Performed data quality checks
- Removed unnecessary columns
- Checked categorical variables
- Prepared the data for further analysis

---

## ⚙️ Feature Engineering

Several features were created to support the analysis.

### Customer Age

Customer age was calculated using the customer's date of birth.

### Customer Tenure

Customer tenure was calculated based on the subscription start date and the relevant end/current date.

### Churn Flag

The `churn_flag` variable was used to identify whether a customer had churned.

```text
0 → Retained Customer
1 → Churned Customer
```

### Churn Risk

Customers were analyzed based on their churn risk to identify potentially high-risk customer segments.

### Categorical Encoding

Categorical variables were encoded where required for analysis and modeling.

---

## 📈 Key Performance Indicators

### 1. Churn Rate

```text
Churn Rate =
Churned Customers / Total Customers × 100
```

### 2. Retention Rate

```text
Retention Rate =
100 - Churn Rate
```

### 3. ARPU

```text
ARPU =
Total Revenue / Active Customers
```

### 4. Average Customer Tenure

Average duration for which customers remained subscribed.

### 5. Revenue at Risk

Revenue associated with customers having a high churn risk.

### 6. Escalation Rate

```text
Escalation Rate =
Total Escalations / Total Complaints × 100
```

---

## 🔍 Analysis Performed

### 1. Overall Churn Analysis

Calculated the overall churn rate to understand the proportion of customers who left the service.

### 2. Retention Analysis

Calculated the overall retention rate to understand the proportion of customers who remained active.

### 3. Churn by Plan Type

Analyzed churn across different subscription plans:

- Basic
- Standard
- Premium

### 4. Churn by Contract Type

Compared churn across different contract durations, particularly:

- Monthly
- Annual

### 5. Churn by State

Analyzed churn across different geographical regions to identify states with relatively higher churn.

### 6. Churn by Subscription Type

Compared churn across different subscription/acquisition types.

### 7. Customer Tenure Analysis

Analyzed how long customers remained subscribed and examined tenure in relation to churn.

### 8. Revenue Analysis

Analyzed:

- Total revenue
- Monthly charges
- Revenue associated with churn
- Revenue at risk
- Customer lifetime value (CLTV)

### 9. Customer Risk Analysis

Used churn scores and risk categories to identify customers who may require additional attention.

### 10. Support Analysis

Analyzed complaints and escalations to understand their relationship with customer churn.

---

## 📊 Key Findings

The analysis produced the following key findings:

- **Overall Churn Rate:** 28.6%
- **Overall Retention Rate:** 71.4%
- Monthly-contract customers showed substantially higher churn than annual-contract customers.
- Basic-plan customers represented a large share of churn.
- Karnataka had the highest churn among the states in the analyzed dataset.
- Average customer tenure was approximately **1,451 days**.
- ARPU was approximately **₹18.8** based on the analyzed dataset.
- Revenue loss and CLTV loss were analyzed to quantify the financial impact of churn.

---

## 💡 Business Insights

The analysis suggests several areas that could be investigated further:

### Contract Type

The difference in churn between monthly and annual contracts indicates that contract structure may be an important area for further investigation.

### Plan Type

A significant portion of churn was associated with customers on the Basic plan. Further analysis of pricing, usage, and customer expectations could help understand the reason.

### Geographic Analysis

Karnataka showed the highest churn among the analyzed states. Possible factors such as pricing changes, customer complaints, service issues, or competitive pressure could be investigated further.

### Customer Risk

Customers with higher churn-risk scores can be monitored more closely to identify potential retention opportunities.

### Support

Support complaints and escalations can be analyzed alongside churn to understand whether service-related issues are associated with customer attrition.

---

## 💼 Business Recommendations

Based on the analysis, the following areas can be considered:

- Investigate the reasons behind higher churn among monthly-contract customers.
- Analyze pricing and service-related issues among high-churn customer segments.
- Investigate customer complaints and support escalations.
- Monitor customers with high churn-risk scores.
- Analyze cancellation reasons such as competitor switching and pricing concerns.
- Examine high-churn geographical regions in greater detail.
- Explore retention strategies for customers who are at higher risk of churn.

 
## 📸 Project Visualizations

Key visualizations from the analysis include:

- Churn by Plan Type
- Churn by Contract Type
- Churn by State
- Churn by Subscription Type
- Revenue Analysis
- Customer Risk Analysis
- Support and Churn Analysis

---

## 🚀 Future Improvements

The project can be extended further by:

- Building an interactive Power BI dashboard
- Developing a machine learning model to predict customer churn
- Performing deeper customer segmentation
- Conducting cohort-based retention analysis
- Performing time-series analysis of churn
- Building an automated churn monitoring dashboard

---

## 👨‍💻 Author

**Anish Kumar**

 
