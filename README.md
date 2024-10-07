# SHAPing-Biases

This project, titled "SHAPing how AI Biases are Addressed in Healthcare", was done in preparation for CUCAI (Canadian Undergraduate Conference on Artificial Intelligence).

As a small team of three, we aimed to research and implement ways to expose biases in healthcare datasets. In this repository, you can find the following:

HA_Prediction_QMIND
-
This predictive model uses a Kaggle dataset comprising many patients and their personal information, such as age, sex, cholesterol, chest pain type, and many other factors that may or may not have contributed to a heart attack.

Using **SHAP values (SHapley Additive exPlanations)** and the help of **RandomForestClassifier()**, I created a predictive model that visually showcased the relevance of each factor to its target output — whether the patient would have a heart attack. The result of this model is a horizontal Pareto diagram that orders each factor from highest relevance to lowest relevance. 

This predictive model garnered an accuracy of up to **84%**.

Additionally, this notebook proves that bias was present in the samples; **207** patients were of one sex, while only **96** were of the other sex.

BC_Prediction_QMIND
-
Similarly to **HA_Prediction_QMIND**, this predictive model uses a Kaggle dataset comprising many patients and their personal information, such as age, race, tumour size, T stage, and many other factors that may or may not have contributed to breast cancer.

Again, I used **SHAP values** and **RandomForestClassifier()** to develop a predictive model that presented each factor and its relevance to its target output — whether the patient would have breast cancer. The result of this model is a horizontal Pareto diagram that orders each factor from highest relevance to lowest relevance.

This predictive model amassed an accuracy of up to **85%**.

As for sampling bias, I discovered that almost **85%** of patients were of the "White" race, **less than 7%** of patients were of the "Black" race, and about **8%** of patients identified as neither "White" nor "Black".
