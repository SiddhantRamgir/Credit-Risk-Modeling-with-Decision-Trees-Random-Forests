# Credit-Risk-Modeling-with-Decision-Trees-Random-Forests
Predictive Modeling and Anomaly Detection for Credit Risk Assessment Using Decision Trees and Random Forests

**Summary:**

The assignment focuses on assessing credit risk through predictive modeling using decision trees and random forests. The analysis was conducted on a dataset of past loan customer cases with the following key components:

1. **Exploratory Data Analysis (EDA) & Data Cleaning:**
   - **Missing Values:** Imputed using KNN (K Nearest Neighbor) to predict missing entries based on non-missing values.
   - **Duplicate Values:** Identified and removed 97 duplicates.
   - **Distribution Analysis:** Examined the distribution of numeric and categorical variables. Adjustments included standardizing categorical variables and addressing outliers in numeric data by replacing them with the mean.

2. **Entropy-Based Splits in Decision Trees:**
   - **Categorical Splits:** Entropy and information gain were used to determine the best feature for the root node split. **Credit_History_LE** was identified as the most informative feature.
   - **Binary Splits:** Compared to non-binary splits, binary splits on categorical features resulted in lower information gain, indicating less accuracy.

3. **Incorporation of Continuous Predictors:**
   - Even with continuous numeric predictors included, **Credit_History_LE** remained the best feature for the root node split in decision trees.

4. **Building Decision Tree Models Using Libraries:**
   - The decision tree classifier was initialized with entropy as the criterion. The model achieved an accuracy of 0.79, with **Credit_History_LE** being the most important predictor. The accuracy was higher compared to manually implemented decision trees.

5. **Random Forest Models:**
   - Implemented a random forest model, which also highlighted **Credit_History_LE** as the most important feature. The model's accuracy was 0.74, indicating that the decision tree performed better for this dataset.

6. **GDPR Compliance:**
   - The analysis demonstrated that even without sensitive data like Age and Personal Status, **Credit_History_LE** continued to be the most predictive feature. The model maintained high accuracy while adhering to GDPR restrictions.

7. **Anomaly Detection:**
   - Analyzed credit grading patterns over time and found no significant anomalies or trends, indicating a stable grading process.

**Conclusion:**
The decision tree and random forest models were effective in predicting credit risk. **Credit_History_LE** emerged as the most significant predictor variable. The decision tree model provided higher accuracy compared to the random forest, and both models performed well even with GDPR-compliant constraints.
