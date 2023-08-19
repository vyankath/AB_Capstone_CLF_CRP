# AB_Capstone_CLF_CRP
ClasificationCapstone Project.

**Problem Statement**

The goal of this project is to predict whether patients have a 10-year risk of developing coronary heart disease (CHD) based on data from an ongoing cardiovascular study in Framingham, Massachusetts. The dataset includes information on 15 attributes for over 4,000 patients.

**Approach**

The project began by handelling missing data. Various techniques, such as KNN Imputer and Simple Imputer, were used to handle null values. The impact of factors like smoking, blood pressure, BMI, and glucose levels on heart conditions was explored.

Factors like age, blood pressure, and glucose level were found to play a significant role in heart disease. Correlations between different factors were analyzed. Class imbalance was tackled using the SMOTE technique and SMOTE combined with Tomek links for better balance.

Classification models were built, starting from Logistic Regression to SVM with different algorithams, Random Forest, and XGBoost. Random Forest and XGBoost performed well, with Random Forest the best results.

**Conclusion**

Among the different models tested, Random Forest out as the optimal choice for predicting CHD risk. Its performance surpassed other models. This indicates that Random Forest can be a reliable tool for predicting cardiovascular risk.

**Project Summary**

The project focuses on predicting 10-year CHD risk using machine learning. Data from Framingham, Massachusetts, including 15 attributes for 4,000+ patients, is used. Missing data is handled, and factors affecting CHD risk like blood pressure, BMI, and glucose levels are examined.

Class imbalance is addressed using SMOTE and SMOTE with Tomek links. Different models are tested, with XGBoost emerging as the best performer. This suggests that XGBoost is effective for predicting cardiovascular risk in patients.
