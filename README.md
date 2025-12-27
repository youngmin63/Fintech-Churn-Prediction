This project was developed as part of a university coursework and explores customer churn prediction in a FinTech context using a custom dataset inspired by the Kaggle Telco Customer Churn dataset.

## I. Project Goals and Tasks

This project aims to predict customer churn in a FinTech application using user behaviour and transaction data. The objective is to identify key factors associated with churn and to provide actionable insights that can support data-driven retention strategies. To achieve this, the project applies and compares two machine learning classification models to analyse churn patterns and predictive performance.

## II. EDA Summary

- Monthly spending and total transaction amount showed overlapping distributions between churned and retained users, indicating that spending alone does not clearly separate churn behaviour.
- User activity duration (months_active) did not exhibit a strong linear relationship with churn, suggesting more complex behavioural patterns.
- Churn rates varied across categorical features such as membership type, payment method, and preferred channel, highlighting structural differences in user behaviour.
- Users on paid membership plans showed slightly higher churn rates than free users, indicating potential gaps between pricing and perceived value.
- Card-based payment users exhibited lower churn rates, suggesting a possible lock-in effect from certain payment methods.
- In-app support usage was associated with lower churn rates, implying that timely support interactions help reduce user churn.

## III. Description of Approach

### Data Preparation

The dataset was preprocessed by removing non-predictive identifier columns and separating the target variable (user_churn) from input features. Categorical variables were transformed using one-hot encoding, and numerical variables were scaled to ensure consistent feature ranges. The data was then split into training and test sets using stratified sampling to preserve the original churn distribution.

### Modelling Approach

Customer churn prediction was formulated as a binary classification problem. Two machine learning models were applied and evaluated:

- Logistic Regression 
- Random Forest Classifier

Both models were trained on the training set and evaluated on a held-out test set to compare predictive behaviour and performance.

## IV. Results Interpretation and Business Implications

Key Drivers of Churn

Across the models, cumulative transaction behaviour and spending intensity emerged as the most important predictors of customer churn. These variables act as strong behavioural signals that reflect long-term user engagement and usage patterns rather than direct causes of churn.

Business Implications

The results suggest that FinTech apps can reduce churn by prioritising high-value users through proactive engagement strategies and by strengthening trust and support mechanisms. Improving the visibility and accessibility of in-app support features and encouraging the adoption of security options may help lower churn risk and improve long-term user retention.

## V. Conclusion

This project demonstrates that customer churn in FinTech applications can be effectively analysed and predicted using transaction and engagement data. By applying two complementary machine learning models, the analysis highlights the importance of behavioural signals over static user attributes. The findings provide practical insights that can inform retention strategies and support data-driven decision-making in FinTech platforms.
