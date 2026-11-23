# Customer Intelligence & Purchase Prediction

An end-to-end Data Science and Machine Learning project that analyzes e-commerce customer behavior, segments customers based on purchasing patterns, and predicts future purchase behavior.

## Project Overview

The project uses the Online Retail II dataset to transform transaction data into actionable business insights.

It focuses on two main tasks:

- **Customer Segmentation:** Grouping customers based on their purchasing behavior using RFM Analysis and K-Means Clustering.
- **Purchase Prediction:** Predicting whether a customer will make a purchase within the next 90 days using Machine Learning classification models.

## Dataset

- **Source:** [UCI Online Retail II Dataset](https://archive.ics.uci.edu/dataset/502/online+retail+ii)
- Transactional e-commerce data.
- Includes invoice details, products, quantities, prices, dates, and customer IDs.

## Project Workflow

### 1. Data Preprocessing
- Data cleaning and handling missing values.
- Removing cancelled transactions and invalid records.
- Calculating transaction revenue.

### 2. Customer Segmentation
- RFM Analysis: Recency, Frequency, and Monetary.
- Log Transformation and StandardScaler.
- K-Means Clustering.
- Identifying four customer segments:
  - Champions
  - At-Risk Customers
  - Hibernating Customers
  - Recent / Developing Customers

### 3. Purchase Prediction
- Defining a 90-day prediction window.
- Feature Engineering using historical customer behavior.
- Training and comparing:
  - Logistic Regression
  - Random Forest
  - XGBoost
- Classification threshold optimization.

### 4. Model Evaluation

The final Logistic Regression model achieved:

| Metric | Score |
|---|---:|
| Accuracy | 71.52% |
| Precision | 64.42% |
| Recall | 76.91% |
| F1-Score | 70.11% |
| ROC-AUC | 79.45% |
| PR-AUC | 76.02% |

The final classification threshold was set to 0.4 to improve Recall.

### 5. Interactive Dashboard

An interactive Plotly dashboard presents:
- Customer distribution by segment.
- Revenue contribution by segment.
- Average revenue per customer.
- Actual vs. predicted purchase rates.
- Average purchase probability.
- Actual vs. predicted buyers.

## Technologies & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Scikit-learn
- XGBoost
- Google Colab

## Business Value

The project helps businesses:
- Understand customer purchasing behavior.
- Identify high-value and at-risk customers.
- Predict potential repeat purchases.
- Design targeted marketing campaigns.
- Improve customer retention strategies.

## Project Structure

```text
Customer-Intelligence-Purchase-Prediction/
│
├── Customer_Intelligence_Project.ipynb
├── Customer_Intelligence_Dashboard.html
├── Customer_Segmentation_Results.csv
├── Cluster_Profile.csv
├── Revenue_Analysis.csv
├── README.md
└── requirements.txt
```

## Author

**Menna Mohamed Shaheen**

AI Student | Machine Learning & Data Science

---

*This project was developed for educational and portfolio purposes.*
