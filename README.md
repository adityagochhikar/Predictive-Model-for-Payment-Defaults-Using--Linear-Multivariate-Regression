#  📊 Bank Loan Default & Credit Risk Analysis
# 🎯 Objective

Banks need to ensure financial stability while managing loan defaults and credit risks. This study aims to:

✔ Predict whether a customer can repay their loan.

✔ Estimate the due amount at the end of the payment period.

✔ Develop Linear Regression Models (Simple & Multiple) to assess credit risk and improve financial decision-making.

✔ Perform statistical validation to ensure model reliability.

# 📂 Dataset Overview

# 📌 Independent Variables:

Credit Score – Measures a customer’s creditworthiness.

Age – Older individuals may be more financially stable.

Credit Accounts – Number of active credit accounts.

Credit Limit – The maximum credit a customer can use.

Employment Status – Whether the customer is employed or not.

Gender – Examining gender-based financial behaviors.

Salary – Income level affecting repayment ability.

# 📌 Dependent Variable:

Due Amount – The outstanding loan balance.

# 🔄 Step-by-Step Model Building Process

Step 1: Define the Problem Statement
✔ Predicting the due amount of a customer based on financial indicators.

Step 2: Selecting Relevant Variables

✔ Initially, credit score was chosen as the key predictor.

✔ Later, age, salary, employment status, credit accounts, and gender were included for better accuracy.

Step 3: Data Collection & Cleaning

✔ The dataset had no missing values.

✔ Data was formatted correctly for regression analysis.

Step 4: Model Specification

✔ Started with Simple Linear Regression (SLR).

✔ Applied Ordinary Least Squares (OLS) Regression to minimize errors.

✔ Transitioned to Multiple Linear Regression (MLR) for better predictive accuracy.

Step 5: Model Fitting

✔ 70% of data used for training.

✔ 30% of data used for testing.

Step 6: Model Validation & Criticism

✔ Evaluated the model using R², p-values, and Variance Inflation Factor (VIF) for multicollinearity.

Step 7: Model Refinement (Handling Multicollinearity)

✔ Dropped Credit Limit & Credit Accounts due to high VIF (>10).

Step 8: Final Model Deployment

✔ The best-performing model was selected based on statistical significance and interpretability.

# 🔄 Regression Models & Analysis

# 📍 Simple Linear Regression (SLR) Model

due_amount = −192 + 1.30 × credit_score

due_amount=−192+1.30×credit_score

Correlation: +0.86 (Strong positive relationship).

Error Issue: The best-fit line did not minimize errors, requiring an OLS Regression approach.

# 📍 Ordinary Least Squares (OLS) Regression Model

due_amount = − 194.74 + 1.31 × credit_score

due_amount=−194.74+1.31×credit_score

Goodness of Fit (R² Value): 75%

# Key Insight:

Credit score explains 75% of the variation in due amount.

Some low credit score customers still have high due amounts, requiring deeper analysis.

# 📍 Multiple Linear Regression (MLR) Model

✔ To improve predictive power, additional financial variables were included:

due_amount = 1.3254 × credit_score − 200.7348

due_amount=1.3254×credit_score−200.7348

Initial R² Value: 74.7%

Final Adjusted R² Value: 95.2% (After adding key predictors).

# Handling Multicollinearity

✔ High VIF Variables Dropped:

Credit Limit (VIF > 10, highly correlated).

Credit Accounts (high p-value > 0.05, insignificant predictor).

# ✔ Final Predictors:

Age (-) – Older individuals have lower due amounts.

Credit Score (+) – Higher scores indicate higher due amounts.

Employment Status (-) – Employed individuals tend to owe less.

Salary (-) – Higher salaries correlate with lower due amounts.

# 📊 Assumptions Validation for Linear Regression

✅ 1. Linear Relationship

✔ Scatterplot confirms a linear relationship between credit score & due amount.

✅ 2. Independence of Residuals

✔ The error terms are randomly distributed, confirming independence.

✅ 3. Homoscedasticity (Constant Variance)

✔ Residuals show no increasing or decreasing spread.

✅ 4. Normality of Residuals

✔ The histogram of error terms follows a normal distribution.

✅ 5. Model Performance (R² = 95%)

✔ The model explains 95% of the variation in due amount.

# 🏆 Key Business Insights

📊 1. Age vs Due Amount

✔ Older individuals tend to owe less, indicating better financial discipline.

📊 2. Credit Score vs Due Amount

✔ Higher credit scores correlate with higher due amounts (Borrowers with good credit histories qualify for larger loans).

📊 3. Salary vs Due Amount

✔ Higher salaries lead to lower due amounts, indicating better repayment ability.

📊 4. Employment vs Due Amount

✔ Employed individuals are less likely to have high due amounts.

# 🔮 Conclusion & Recommendations

✔ Final Model Accuracy: 95% (R² Value)

95% of due amount variation can be explained using age, salary, employment, and credit score.

# ✔ How Banks Can Use This Model:

🔹 Identify high-risk borrowers (low-income, unemployed, low credit score).

🔹 Set customized credit limits based on financial indicators.

🔹 Improve loan approval policies & reserve management strategies.

# 🚀 Future Scope

🔹 Enhancing model accuracy using Machine Learning techniques (Random Forest, XGBoost, etc.).

🔹 Exploring additional features like customer spending habits & debt-to-income ratio.

# Final Thoughts

✅ The best-performing model (Multiple Linear Regression) successfully explains 95% of the variance in due amount.

✅ The model satisfies all regression assumptions.

✅ The insights help banks make better loan approval and risk management decisions.

# 🚀 This Version Covers Everything!

I have fully integrated everything, including:

✔ SLR, OLS, and MLR models.

✔ Statistical validation (R², p-values, VIF, residual checks, etc.).

✔ Handling multicollinearity & model refinements.

✔ Key insights & business impact.

✔ Future recommendations & next steps.

#                                                Business Case – Credit Cards

