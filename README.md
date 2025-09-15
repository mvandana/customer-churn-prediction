📉 **Customer Churn Prediction**

**Summary**

Customer churn isn’t just a KPI, it’s a silent revenue killer. In this project, I built a fully functional churn prediction engine using telecom customer data. The model identifies high-risk users based on tenure, billing behavior, and contract preferences — arming teams with actionable insights to reduce churn.

The model is interpretable, fast to deploy, and delivers real-time churn probabilities for any new customer, making it ideal for integration into CRM systems or retention dashboards.

**My Approach**

1. Data Cleaning & Transformation
•	Converted TotalCharges to numeric and handled missing values.
•	Dropped irrelevant columns.

2. Exploratory Data Analysis (EDA)
•	Visualized churn distribution to understand class imbalance.
•	Used a heatmap to explore correlations between tenure, charges, and churn.

3. Feature Engineering
•	Label-encoded binary columns (e.g., gender, Partner, Churn).
•	One-hot encoded multi-class columns like Contract, InternetService, and PaymentMethod.
•	Scaled numerical features (tenure, MonthlyCharges, TotalCharges) for model stability.

4. Modeling
•	Trained a Decision Tree Classifier with max_depth=6 to balance performance and interpretability.

5. Evaluation & Diagnostics
•	Assessed performance using classification report (precision, recall, F1-score).
•	Visualized the confusion matrix to analyze prediction accuracy.
•	Plotted feature importances to identify top churn drivers.

6. Prediction Logic
•	Built a pipeline to input new customer data, align features, scale values, and predict churn probability.
•	Example: A customer with high monthly charges and a month-to-month contract had a 61% churn risk.

**Business Impact**

This model is more than just predictive, it’s prescriptive. Here’s what it enables:

•	Proactive Retention: Identify customers likely to churn before they actually do, and deploy tailored retention offers.
•	Prioritized Interventions: Focus outreach on customers with high churn probability, optimizing resource allocation.
•	Explainable Decisions: Tree-based model provides visibility into why a customer is flagged, useful for support teams.

Even a 5% reduction in churn can significantly boost recurring revenue, and this project gives teams the data muscle to make that happen.
