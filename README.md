# 📺 Netflix Userbase Analysis Report

## 📌 Overview

This repository contains an in-depth analysis of a Netflix userbase dataset. The primary goal is to understand customer behavior and identify strategies to increase the customer base and revenue. The analysis includes data visualizations, LTV and engagement metrics, and predictive models for churn and LTV forecasting.

---

## 📂 Dataset

The dataset includes detailed user information such as:

- Subscription type
- Monthly revenue
- Join date and last payment date
- Country, age, and gender
- Primary streaming device

---

## 📊 Analysis and Key Findings

### 🌍 User Distribution and Demographics

- **Geographic Concentration**: Highest user counts in the **United States** and **Spain**, followed by **Canada**.
- **Gender Balance**: Users are almost evenly split between male and female.
- **Age Groups**: Dominant age brackets are **26–35** and **46–51**.
- **Device Usage**: Netflix is accessed via smartphones, tablets, laptops, and smart TVs.

### 💳 Subscription and Engagement

- **Plan Preferences**:
  - **Mexico** prefers Standard plans.
  - **Brazil, Canada, Germany, Italy** lean toward Basic plans.
  - **US and Spain** dominate Premium subscriptions.
- **Average User Duration**: ~**10.14 months**.
- **Lifetime Value (LTV)**:
  - **Total LTV** highest in **US** and **Spain**.
  - **Average LTV** per user peaks in **France** and **UK**.
  - **Tablets and Laptops** show slightly better revenue performance.

---

## 🔮 Predictive Modeling

### ⚠️ Churn Prediction – Random Forest Classifier

- **Definition**: Churn is based on user duration.
- **Metrics**:
  - Accuracy: 0.5296
  - Precision: 0.5269
  - Recall: 0.5641
  - F1-Score: 0.5449
  - AUC: 0.5168

### 💰 LTV Prediction – Random Forest Regressor

- **Goal**: Estimate long-term user value for targeted strategies.
- **Metrics**:
  - MAE: 0.4079
  - MSE: 2.3005
  - R²: 0.9973

---

## 🛠 Tools & Technologies

- **Python**: Data analysis and modeling
- **Pandas**: Data manipulation
- **Matplotlib & Seaborn**: Visualizations
- **Scikit-learn**: Machine learning models
- **Jupyter Notebook**: Interactive analysis

---

## 🧭 Next Steps & Strategy Recommendations

- **Deeper Regional Insights**: Conduct granular analysis in high-LTV regions (France, UK) to determine what drives customer value.
- **Churn Driver Analysis**: Identify key features contributing to churn risk using model interpretability tools (e.g., SHAP).
- **Behavioral Segmentation**: Segment users by behavior, demographics, and LTV to personalize content and offers.
- **Retention Tactics**: Design campaigns for users predicted to churn—e.g., exclusive offers, early access to content.
- **Upsell Opportunities**: Encourage Basic and Standard users in high-value regions to shift to Premium via tailored recommendations.
- **Device-Specific Experience**: Enhance UX on tablets and laptops where LTV is higher to boost retention.
