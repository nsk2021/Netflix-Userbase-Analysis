# 📺 Netflix Userbase Analysis

## 📌 Overview

This repository presents a detailed analysis of a Netflix userbase dataset. The primary objective is to explore user behavior, identify key revenue-driving segments, and develop data-backed strategies to improve customer retention and Lifetime Value (LTV). The project includes EDA, user profiling, LTV calculation, churn prediction, and future recommendations.

---

## 📊 Netflix Userbase Analysis Final Report

This report compiles the key findings and insights from the analysis of the Netflix userbase dataset, along with potential strategies and next steps based on these findings and the predictive modeling conducted.

---

## 📂 Data Overview and Initial Findings

- The dataset contains user-level data such as:
  - Subscription type and monthly revenue
  - Join and last payment dates
  - Country, age, gender, and device used
- The dataset had **no missing or duplicate rows**, ensuring clean input for analysis.
- Calculated fields include:
  - **Subscription duration** (in days and months)
  - **Lifetime Value (LTV)** = Monthly Revenue × Duration

---

## 🌍 User Distribution and Demographics

- **Geographic Concentration**: United States and Spain have the highest number of users, followed by Canada.
- **Gender Balance**: Consistent and balanced across countries and devices.
- **Age Concentration**: Most users are in the **26–35** and **46–51** age groups.
- **Device Usage**: Netflix is accessed through smartphones, tablets, laptops, and smart TVs.

---

## 💳 Subscription Type Analysis

- **Plan Preferences by Country**:
  - **Mexico** favors Standard plans.
  - **Brazil, Canada, Germany, Italy** lean toward Basic.
  - **US and Spain** dominate Premium subscriptions.
- **Plan Preferences by Device**:
  - Useful for tailoring device-specific marketing and bundle offerings.

---

## ⏱️ User Engagement & Lifetime Value (LTV)

- **Average Engagement Duration**: ~**10.14 months**
- **LTV Highlights**:
  - **Highest total LTV**: United States and Spain
  - **Highest average LTV**: France and the UK
  - **Devices**: Tablets and laptops yield slightly higher LTVs
  - **Age-based LTV**: Remains relatively consistent across age groups

---

## 🔮 Predictive Modeling Insights

### ⚠️ Churn Prediction – Random Forest Classifier

- **Churn Definition**: Based on shortened user duration
- **Performance**:
  - Accuracy: 0.5296
  - Precision: 0.5269
  - Recall: 0.5641
  - F1-score: 0.5449
  - AUC: 0.5168

**Model Insights**:
- Users with shorter durations, lower revenue, and certain device types (e.g., smartphones) had higher churn probabilities.
- Feature importance analysis showed **subscription type**, **device**, and **monthly revenue** were strong predictors of churn.
- This model enables proactive targeting of high-risk users with tailored retention campaigns or loyalty offers.

---

### 💰 LTV Prediction – Random Forest Regressor

- **Purpose**: Forecast user-level revenue potential
- **Performance**:
  - MAE: 0.4079
  - MSE: 2.3005
  - R²: 0.9973

**Model Insights**:
- LTV was most influenced by **subscription type**, **duration**, and **monthly revenue**.
- Users on Premium plans and using tablets/laptops had significantly higher predicted LTVs.
- This model helps identify valuable user segments for upselling, targeted promotions, or content personalization.

---

## 🛠 Tools & Technologies

- **Python** – Core scripting language
- **Pandas** – Data wrangling
- **Matplotlib & Seaborn** – Visualization
- **Scikit-learn** – Predictive modeling
- **Jupyter Notebook** – Exploratory analysis and documentation

---

## 🧭 Next Steps & Strategy Recommendations

### 🔍 Next Steps

- **Deep Dive into High LTV Countries**: Analyze user traits in France and UK to discover drivers of high value
- **Analyze Churn Factors**: Use model features and SHAP values to identify churn triggers
- **Segmentation Analysis**: Group users by age, country, device, plan, churn probability, and LTV
- **Time Series Analysis**: Explore churn, acquisition, and revenue trends over time
- **Feature Importance Analysis**: Identify what drives churn and LTV through model interpretation

### 💡 Strategies to Grow Customers & Revenue

- **Targeted Marketing Campaigns**: Segment by country, device, age group, LTV, and churn risk
- **Subscription Plan Optimization**: Tailor pricing based on country-specific preferences and value
- **Device-Specific Strategies**: Improve UX for high-revenue devices like tablets and laptops
- **Content Strategy**: Customize recommendations based on engagement and predicted LTV
- **Churn Reduction Initiatives**: Run proactive engagement for high-risk users with exclusive offers
- **Loyalty Programs**: Reward high-LTV users to boost retention and satisfaction
- **Promotions & Partnerships**: Collaborate with device manufacturers or telecoms in high-potential regions
