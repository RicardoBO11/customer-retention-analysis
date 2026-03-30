# Customer Churn Analysis Project

## Business Context

In highly competitive markets, customer retention is a critical factor for sustainable growth. Companies must understand **why customers churn** and identify the key drivers behind customer disengagement.

This project analyzes customer behavior, spending patterns, and membership tiers to uncover insights that can help reduce churn and increase customer lifetime value.

---

## Objective

The main goal of this analysis is to:

* Identify the key factors driving customer churn
* Understand the relationship between customer value and retention
* Provide actionable recommendations to improve customer retention

---

## Dataset Description

The dataset includes customer-level information such as:

* `customer_id`: Unique identifier
* `gender`: Customer gender
* `age`: Customer age
* `city`: Customer location
* `membership_type`: Bronze, Silver, Gold
* `total_spend`: Total amount spent
* `items_purchased`: Number of items purchased
* `average_rating`: Customer rating
* `discount_applied`: Whether a discount was applied
* `days_since_last_purchase`: Recency indicator
* `satisfaction_level`: Customer satisfaction score
* `churn`: Target variable (1 = churn, 0 = retained)

---

## Key Insights

### 1. High Overall Churn

* The churn rate is **35.4%**, indicating a significant retention problem.

### 2. Membership Drives Retention

* Bronze: 51.7% churn
* Silver: 49.6% churn
* Gold: 5.1% churn

Gold members are highly loyal, while lower tiers are at high risk.

---

### 3. Customer Value Matters

* Churned customers spend significantly less (~619 vs ~969).

Lower engagement is strongly linked to churn.

---

### 4. Satisfaction is Not Predictive

Satisfaction shows limited impact in isolation but becomes a strong predictor when combined with other variables.

---

### 5. Discount Strategy Needs Review

* Customers without discounts show extremely low churn.

This may indicate selection bias or ineffective targeting.

---

### 6. Short-Term Purchase Behavior

* High purchase activity does not guarantee retention.

Some users engage temporarily and then churn.

---

## Business Impact

This analysis highlights that churn is concentrated among **low-value and low-tier customers**, while high-value customers (Gold members) remain loyal and profitable.

Improving retention strategies could:

* Increase revenue
* Reduce customer acquisition costs
* Improve long-term business sustainability

---

## Recommendations

### 1. Promote Membership Upgrades

Encourage users to move to higher tiers through incentives and exclusive benefits.

---

### 2. Engage Low-Value Customers

Target low-spending users with personalized campaigns to increase engagement early.

---

### 3. Improve Post-Purchase Retention

Implement loyalty programs, follow-ups, and cross-selling strategies.

---

### 4. Reassess Satisfaction Metrics

Improve how satisfaction is measured to better predict churn.

---

### 5. Optimize Discount Usage

Analyze discount allocation to ensure it effectively reduces churn.

---

## Tools & Technologies

* Python (Pandas, NumPy)
* Data Visualization (Matplotlib / Seaborn)
* Jupyter Notebook

---

## Machine Learning Model

To complement the analysis, a predictive model was developed to identify customers at risk of churn.

### Model Used

* Logistic Regression

### Data Preparation

* Categorical variables encoded using one-hot encoding
* Satisfaction level transformed into an ordinal feature (`satisfaction_score`)
* Missing values handled with mean imputation
* Irrelevant columns removed (e.g., `city`, `customer_id`)

---

## Model Performance

| Metric    | Score |
| --------- | ----- |
| Accuracy  | 0.98  |
| Precision | 0.96  |
| Recall    | 1.00  |
| F1 Score  | 0.98  |

### Confusion Matrix

```
[[42  1]
 [ 0 27]]
```

---

## Model Insights

* The model successfully identifies all churned customers (Recall = 1.0)
* Customer satisfaction and recency are key predictors
* The model slightly overestimates churn, which is acceptable in retention strategies

---

## Business Value of the Model

This model can be used to:

* Identify at-risk customers in advance
* Trigger retention campaigns
* Reduce churn-related revenue loss

---

## Limitations

* Small dataset may lead to slight overfitting
* Results should be validated with more data before deployment

---

## Project Highlights

- End-to-end data analysis (EDA + Machine Learning)
- Strong business-oriented insights
- High-performing churn prediction model (Recall = 1.0)
- Focus on customer retention strategies

---

## Author

This project is part of my journey to become a **Data Analyst**, focusing on solving real business problems through data-driven insights.


