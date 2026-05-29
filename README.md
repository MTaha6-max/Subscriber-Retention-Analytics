# Telecom Customer Churn: From Exploratory Data Analysis (EDA) to Diagnostic Insights

## Executive Summary
This project delivers an end-to-end data analytics solution investigating customer attrition (churn) for a Telecom provider. By combining statistical data discovery in **Python** with advanced executive storytelling in **Power BI**.

---

## Business Problem
* **Critical Revenue Exposure:** The overall churn rate stands at a high **26.5%**, which is significantly above telecom industry benchmarks. More alarmingly, the calculated **Revenue at Risk ($139.13K)** represents a staggering **44%** of our total active **Monthly Recurring Revenue (MRR: $316.99K)**. This means nearly half of the company's predictable monthly cash flow is actively exposed to immediate erosion, shifting this analysis from a routine review to a critical operational priority.

---
## Methodology
* **Data Wrangling & Analysis:** Python (Pandas, NumPy)
* **Business Intelligence & Visualization:** Power BI Desktop (DAX, Star-Schema Layout)

---
### Skills

1. Power BI: Advanced DAX, Custom Measures, ETL (Power Query), Calculated Columns, Data Modeling (Star Schema), Executive Data Visualization 
2. Python: Exploratory Data Analysis (EDA), Pandas, NumPy, Matplotlib, Custom Reusable Functions, Statistics, Product Funnel Building 
3. Business Analytics: Diagnostic Analytics, Financial Metric Modeling (MRR, Revenue at Risk), Retention & Churn Strategy 

---
## 🔍 Deep-Dive Diagnostic Scenarios & Insights

### Scenario 1: The Fiber Optic Crisis
* **The Discovery:** A deep segment analysis reveals that **Fiber Optic** subscribers exhibit an alarming churn rate of over **40%**, drastically outperforming DSL and non-internet users in attrition.
* **The Business Impact:** Fiber Optic is our premium, high-ticket product. High churn here indicates a severe gap between customer expectations and product delivery (e.g., speed drops, pricing traps, or unreliable infrastructure).
* **Strategic Recommendation:** Issue an immediate service quality audit for fiber infrastructure and offer targeted loyalty discounts to high-risk fiber cohorts before their next billing cycle.
churn rate by internet service.png
<img width="343" height="290" alt="churn rate by internet service" src="https://github.com/user-attachments/assets/f6886fd0-1363-492a-b969-8bb3419294c1" />

### Scenario 2: Support Person Attitude & Customer Service Friction
* **The Discovery:** "Support Person Attitude" ranks as the #1 primary qualitative reason stated for customer exit, directly driving a massive chunk of overall attrition.
* **The Business Impact:** Technical stability means nothing if the human touchpoint creates friction. Poor customer service actively destroys brand equity and undoes millions spent on marketing.
* **Strategic Recommendation:** Implement mandatory customer empathy and technical resolution training for support staff, tied directly to quarterly performance bonuses and CSAT scores.
<img width="460" height="273" alt="churn reason" src="https://github.com/user-attachments/assets/98cce7a6-ee83-4b03-887e-aa7e8aeab965" />


### Scenario 3: The Month-to-Month Contract & Value Gap
* **The Discovery:** Customers on **Month-to-Month** contracts represent the vast majority of churned users, carrying an individual churn probability of **42.7%**, whereas 1-year and 2-year contracts remain highly stable.
* **The Business Impact:** Short-term contracts lack "friction" to exit. Without contractual lock-in, any minor inconvenience prompts the customer to drop the service.
* **Strategic Recommendation:** Launch a proactive migration campaign offering a free month of service or a hardware upgrade (e.g., premium router) in exchange for switching to a 1 or 2-year contract.
<img width="454" height="288" alt="churn rate by contract" src="https://github.com/user-attachments/assets/08da0c85-dc62-4986-9175-479614a02805" />
<img width="478" height="290" alt="customer churn risk by tenure" src="https://github.com/user-attachments/assets/2e1c3055-763d-45ce-9fb3-b6710b013584" />


### Scenario 4: The Tech Support 
* **The Discovery:** Substantial data correlation shows that subscribers who do **not** have **Tech Support** or **Online Security** add-ons enabled exhibit churn rates soaring past **41.6%**. Conversely, those with these features enabled are highly sticky.
* **The Business Impact:** Value-added services create ecosystem "stickiness." When a customer relies on the provider for digital safety and immediate technical relief, the switching costs become psychologically higher.
* **Strategic Recommendation:** Bundle Online Security and Tech Support features into standard internet packages for the first 6 months for all new sign-ups to build early product dependence.
<img width="346" height="269" alt="churn rate by tech support" src="https://github.com/user-attachments/assets/374969ca-7610-4f07-b21a-654353bc30f6" />


### Scenario 5: The Electronic Check Payment Trap
* **The Discovery:** The payment method breakdown isolates **Electronic Check** as a severe operational bottleneck, yielding an aggressive **45.3%** churn rate. Customers utilizing Automated methods (Credit Card Auto-pay / Bank Transfer) show minimal attrition.
* **The Business Impact:** Manual monthly payment via electronic check forces the customer to actively review their expenses every single month, triggering a conscious re-evaluation of the service's value. Automatic payments create frictionless retention.
* **Strategic Recommendation:** Incentivize the transition to Auto-pay by offering a one-time $5 bill credit or bonus data for any customer migrating away from manual electronic checks.
<img width="487" height="277" alt="churn rate by payment method" src="https://github.com/user-attachments/assets/87d82518-1d77-46d0-a0c9-f747af118f78" />

---

## Data Limitations & Future Recommendations

* **Missing Time-Series Data:** The current dataset lacks actual calendar timestamps (Dates) for when subscribers churned. This limits the analysis to static historical snapshots based on customer tenure.
* **Recommendation:** Recommend implementing monthly snapshot tracking (Snapshot Date) to allow the calculation of active Monthly Churn Rates (Cohorts) over calendar months, moving the dashboard into true time-series forecasting.
