# Stroke-Prediction-
This dataset is used to predict whether a patient is likely to get stroke based on the input parameters like gender, age, various diseases, and smoking status. Each row in the data provides relevant information about the patient.

![stroke ](https://user-images.githubusercontent.com/125938742/236397413-7477643c-3a56-4ee1-b77a-4ae1cd7db921.jpeg)



**Source: https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset**

**Culumn** | **Description**  
--- | ---
id|unique identifier
age |age of the patient
gender| "Male", "Female" or "Other"
hypertension| 0 hypertension, 1  hypertension
heart_disease |0  doesn't have diseases, 1  has a heart disease
ever_married| "No" or "Yes"
work_type |"children", "Govt_jov", "Never_worked", "Private" or "Self-employed"
Residence_type|"Rural" or "Urban"
avg_glucose_level| average glucose level in blood
bmi| body mass index
smoking_status| "formerly smoked", "never smoked", "smokes" or "Unknown"
stroke| 1if the patient had a stroke or 0 if not

*Note: "Unknown" in smoking_status means that the information is unavailable for this patient
*Violin Plot 
![Violinplot ](https://user-images.githubusercontent.com/125938742/236390555-5f25f946-138a-43c9-8aa3-45e24d7def9e.png)

This violin plot depicts a clear pattern where there is a high concentration of women with hypertension who are at risk of getting strokes. The plot suggests that the female group has a higher incidence of hypertension


![Scatterplot bmi:G_level](https://user-images.githubusercontent.com/125938742/236391263-e4cf3337-6b2c-4c2e-8f3e-3065be43e8ac.png)

The scatter plot dipicts a correlation between BMI (body mass index) and glucose levels. This is because a higher BMI can increase the risk of insulin resistance and type 2 diabetes, which in turn can lead to higher glucose levels.

**Models Evaluated & Results**
1. Random Forest
2. Tuned Random Forest(Grid Search)
3. XGBoost (eXtreme Gradient Boosting) 
4. Tuned XGBoost
5. Logistic Regression
6. Tuned Logistic Regression
7. PCA Random Forest
8. PCA XGBoost



**Recommended Model (XGB):

The XGB model is 94% accurate in identifying stroke patients, which means it is effective in predicting stroke patients. The model also performs well across both stroke and non-stroke patients, and takes into account the class imbalance in our dataset with a 91%  weighted average score. This means that the model is a strong predictor of stroke patients and can be used to identify at-risk patients. 

Recommendations: 
1. Integrate the model into the clinical decision-making process to help identify high-risk patients earlier.
2. Use the XGB model to identify at-risk patients, for healthcare providers can develop personalized health plans for these patients to help prevent strokes. These plans could include lifestyle modifications such as exercise and diet changes, as well as medication management to control risk factors such as high blood pressure and high glucose levels

