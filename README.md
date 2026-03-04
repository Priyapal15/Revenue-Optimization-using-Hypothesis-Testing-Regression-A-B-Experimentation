# Revenue-Optimization-using-Hypothesis-Testing-Regression-A-B-Experimentation

**📌 Project Overview**

This project performs an end-to-end statistical and machine learning analysis to understand the relationship between trip revenue and payment method (Credit Card vs Cash).

The objective is to determine:

Is there a statistically significant relationship between payment type and total fare amount?

Do digital payments generate higher revenue?

Can we nudge customers toward higher-revenue payment methods?

What is the estimated revenue uplift from shifting payment behavior?

How does payment type impact driver earnings?

This project combines Exploratory Data Analysis (EDA), Hypothesis Testing, ANOVA, Regression Modeling, Logistic Regression, Revenue Simulation, and A/B Testing Framework to deliver business-ready insights.



**🗂 Dataset**

This is a hypothesis testing project that I've created to perform some analytics and statistical test to test hypothesis regarding the revenue increasing for cab provider named yellow trip as per their 2020 january data. The dataset can be found here. https://www.kaggle.com/datasets/microize/newyork-yellow-taxi-trip-data-2020-2019

NYC Taxi Trip Data (January 2020)

Features used:

payment_type

fare_amount

total_amount

tip_amount

Data preprocessing steps:

Removed negative/zero fares

Filtered only Credit Card & Cash

Trimmed extreme outliers (99th percentile)

Encoded categorical variables



**🔍 Exploratory Data Analysis (EDA)**

Descriptive statistics by payment type

Revenue distribution comparison

Outlier detection & trimming

Boxplots for revenue spread

Histogram for distribution analysis

Key Observation:
Credit card payments showed higher average total fare compared to cash payments.

📊 Hypothesis Testing
1️⃣ Independent T-Test

H₀ (Null Hypothesis):
There is no difference in average revenue between payment types.

H₁ (Alternative Hypothesis):
There is a significant difference in average revenue between payment types.

Result:

p-value < 0.05 → Reject H₀

Payment type significantly impacts revenue

2️⃣ ANOVA Test

Confirmed statistical difference in mean revenue across payment groups.

📈 Linear Regression Modeling

Model:
Total Fare = β₀ + β₁(Payment Type)

Findings:

Credit Card coefficient was positive

Indicates revenue lift associated with digital payments

Statistically significant relationship

Business Meaning:
Digital payments correlate with higher trip revenue.

🤖 Logistic Regression (High-Fare Prediction)

Defined high-fare trips as top 25% of revenue.

Model predicts probability of a trip being high-value using:

Payment type

Fare amount

Tip amount

Evaluation:

Classification Report

ROC-AUC score

Insight:
Payment behavior contributes to predicting high-value trips.

💰 Revenue Uplift Simulation

Simulated 10% customer shift from Cash → Credit Card.

Estimated:

New projected average revenue

Revenue uplift per trip

Business-scale revenue impact

Conclusion:
Small behavioral shifts can generate measurable revenue gains.

🧪 A/B Testing Framework

Designed experimental structure:

Control Group → No payment incentive

Treatment Group → Digital payment incentive

Used:

Two-sample T-test

Distribution comparison

Statistical significance validation

This demonstrates real-world experimentation capability.

🚕 Driver Revenue Impact Analysis

Compared:

Average revenue per trip

Total revenue contribution

Trip count by payment type

Finding:
Encouraging digital payments can improve average driver earnings.
