**Problem Statement**

The main objective is to predict whether a patient has a 10-year risk of developing coronary heart disease (CHD). The dataset used in this study is from an ongoing cardiovascular study conducted on residents of Framingham, Massachusetts.  The dataset contains information on more than 3,390patients and includes 16 attributes, each representing a potential risk factor for CHD. These attributes cover various aspects, including demographic information, behaviors, and medical factors that could influence the risk of developing coronary heart disease.


# **The Dataset and Approach:-**
- Dataset has 17 columns and 3390 rows.
- Among the 17 columns the datatypes of the columns are float64-9, int64-6-, object-2.
- The dataset has missing values in the columns education, cigs per day, BP meds, totChol, BMI, heart rate and glucose.
- There are no duplicated columns but various columns may have duplcated vales.

The project began by handelling missing data. Various techniques, such as KNN Imputer and Simple Imputer, were used to handle null values. The impact of factors like smoking, blood pressure, BMI, and glucose levels on heart conditions was explored.Factors like age, blood pressure, and glucose level were found to play a significant role in heart disease. Correlations between different factors were analyzed. Class imbalance was tackled using the SMOTE technique and SMOTE combined with Tomek links for better balance.Classification models were built, starting from Logistic Regression to SVM with different algorithams, Random Forest, and XGBoost. Random Forest and XGBoost performed well, with Random Forest the best results.

As part of making the data easier to work with, i have **renamed all the columns** in the dataset. Additionally, identified and categorized the different types of variables to simplify the process of plotting graphs.**Droped id columns** which has all are unique values which will not help for anything.By renaming columns and categorizing variables, we can easily navigate and analyze the dataset, and plotting graphs becomes a more straightforward task, making the overall analysis process more efficient and intuitive.

# **Insights From EDA:-**

* In our dataset, **15.1% of individuals are at risk for cardiovascular disease, while 84.9% are considered safe from the ten-year risk.**

* Notably, there is a higher prevalence of cardiovascular disease risk in individuals **aged between 51 to 63.**

* The distribution of risk **between genders is balanced,** with approximately 200 cases in both males and females being at risk, even though females are more numerous in our dataset.

* Around 250 individuals **who smoke are at risk,** while approximately 210 non-smokers are also at risk for cardiovascular disease.

* It's challenging to definitively establish smoking as a direct cause of heart disease. The count plot reveals **no significant disparity between smokers and non-smokers.** Even the extreme case of an individual smoking 70 cigarettes per day doesn't show a clear link to ten-year risk.

* Around 200 individuals have taken blood pressure (BP) medication, compared to approximately 3200 individuals who haven't. However, **it's not conclusive that taking medication ensures safety from cardiovascular risk.**

* Around 500 individuals who have not experienced a stroke are at risk, contrasting with roughly 2800 individuals who are safe from cardiovascular disease.

* Around 250 individuals with hypertensive conditions are at risk, and a similar number of individuals without hypertensive conditions are also at risk.

* Interestingly, the majority of individuals **without diabetes (around 500) are at risk**, while very few individuals with diabetes show a similar risk.

* The cholesterol levels of individuals at risk and those not at risk don't exhibit a significant difference. For both groups, cholesterol levels are within a relatively similar range.

* Systolic blood pressure varies between 110 to 140 for most individuals who are not at risk, while for those at risk, it's between 125 to 160, **heigher systolic BP is indicative of a potential risk.**

* Diastolic blood pressure shows a slight increase for individuals at risk, with levels between 89 to 90, compared to the 75 to 85 range for those not at risk.

* BMI values between 22 to 28 are common for individuals not at risk, while those at risk have a BMI between 23 to 29, showing a relatively small difference.

* Heart rate ranges from 68 to 83 for individuals not at risk, and 68 to 84 for those at risk, showing minimal variation.

* Glucose levels show no substantial difference between individuals at risk and those not at risk, both ranging from 70 to 80.

* Smoking between 1 to 10 cigarettes is typical for most individuals, with corresponding heart rates between 60 to 100.

* Age distribution spans from 32 to 70, and the majority of individuals have systolic BP between 90 to 200.

# **Conclusion**

* I applied eight classification ML models in our analysis, including Logistic Regression,Decision Tree, Random Forest,AdaBoost,NaieBayes XGBoost, KNN, and SVM.

* After a comprehensive evaluation, **Random Forest (tuned)** emerged as my final optimal model. Despite encountering initial overfitting issues, I successfully mitigated them through hyperparameter tuning.

* **Random Forest consistently delivers the highest recall, precision, F1 score, accuracy, and AUC-ROC among all models.**

* Within a dataset of 678 patients, our optimal model accurately predicts 477 individuals of class 0 and 52 individuals of class 1. There are also 57 false negatives and 133 false positives.

* **Age, sex, and pulse pressure** are the most influential features driving the model's predictions.

* The best hyperparameters for the Random Forest model were determined **as criterion = gini,max depth = 9,min samples leaf = 2, nin samplessplit = 7.**


To sum up, this project showcases the effectiveness of machine learning methods in accurately predicting the 10-year risk of coronary heart disease (CHD) using data sourced from an ongoing cardiovascular study. The project's key takeaways are as follows:

1. Thorough data preprocessing and transformation greatly enhanced machine learning model performance, leading to more precise predictions.
2. The process of feature selection played a pivotal role in identifying the most influential predictors of CHD risk.
3. After evaluating various models, the Random Forest model (tuned) emerged as the final choice due to its strong recall score.
4. A combination of techniques, including SMOTE, Tomek links undersampling, and standard scalar scaling, was employed to address data imbalance and boost model effectiveness.
5. The project exemplifies the practical application of machine learning to solve real-world challenges and attain favorable business outcomes.

In summary, this endeavor underscores the significance of meticulous data preparation and analysis in machine learning ventures. By meticulously cleaning and transforming data, selecting pertinent features, and opting for suitable models, one can achieve accurate predictions and facilitate informed decision-making across diverse industries.
