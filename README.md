# MORINGA-PHASE-3-PROJECT-2024
Customer Churn Prediction for SyriaTel
Project Overview
In the competitive telecommunications sector, customer churn is a significant challenge for companies like SyriaTel. This project focuses on building a predictive model to identify customers at risk of churning. By understanding customer behavior and demographics, SyriaTel can deploy proactive retention strategies to minimize revenue losses and maintain its market reputation.

Business Understanding
Problem Statement
SyriaTel faces the challenge of customer retention in a highly competitive market. Churn results in financial losses and impacts the company’s reputation. The goal is to develop a machine learning model to identify at-risk customers, enabling SyriaTel to implement targeted retention strategies and reduce churn.

Objectives
The project aims to:

Develop a reliable predictive model for churn detection.
Provide actionable insights to stakeholders like the Customer Retention, Marketing, Sales, Customer Support, and Business Analytics teams.
Help mitigate financial losses through targeted customer retention strategies.
Data Understanding
Source: The dataset, sourced from Kaggle, contains 3,333 customer records with 20 attributes, including demographics, usage patterns, and subscription details.

Key Features:

Customer demographics (e.g., state, area code).
Subscription details (e.g., international and voice mail plans).
Service usage metrics (e.g., total call minutes, charges).
Account length as a measure of customer lifetime value.
Churn Distribution:
14.5% of customers (483) have churned, indicating an imbalanced dataset that requires mitigation.

Data Preparation
Steps Taken
Checked for duplicates and missing values (none found).
Analyzed and visualized feature distributions to identify patterns and outliers.
Addressed dataset imbalance for accurate modeling.
Feature Insights
Categorical Features: Area code 415 had the most customers, and churn likelihood varied across codes.
Numerical Features: Usage metrics showed skewed distributions; outliers identified high-usage customers.
Key Predictors: High monthly charges, short tenure, and frequent customer service calls were strong churn indicators.
Modeling and Evaluation
Techniques Used
Logistic Regression and Decision Trees were employed for churn prediction.
Addressed imbalanced data using appropriate resampling techniques.
Performance metrics focused on precision, recall, and AUC for balanced evaluation.
Results
Logistic Regression:

AUC: 0.80
Balanced performance in classifying churn and non-churn cases.
Decision Tree:

AUC: 0.85
Higher AUC but less consistent performance in distinguishing between classes.
Limitations:

Recall for churn prediction was low in initial models, highlighting a need for further refinement.
Key Insights
Churn Correlation: Customers with high service charges or frequent customer service calls were more likely to churn.
Service Preferences: Evening and night call usage dominated, suggesting tailored tariff plans could improve retention.
Plan Effectiveness: International and voice mail plans showed varying impacts on churn behavior.
Recommendations
Target High-Risk Customers:

Offer personalized incentives (e.g., discounts, loyalty rewards).
Address concerns of high-risk customers proactively.
Enhance Customer Experience:

Improve infrastructure and expand support teams based on feedback.
Segment and Personalize:

Use behavior data to segment customers and tailor communication strategies.
Monitor Key Predictors:

Set up alerts for high-risk behaviors (e.g., high charges, short tenure).
Optimize Pricing Plans:

Offer competitive bundles to retain cost-sensitive customers.
Next Steps
Refine the Model:

Experiment with advanced algorithms like XGBoost or CatBoost.
Focus on improving recall to identify more churners.
Deploy the Model:

Build a real-time dashboard for churn predictions.
Collaborate with business teams to validate and act on predictions.
Continuous Improvement:

Update the model with fresh data to adapt to evolving customer behavior.
Tools and Technologies
Languages: Python (pandas, numpy, matplotlib, seaborn, scikit-learn).
Environment: Jupyter Notebook.
