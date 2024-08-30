# Heart_Disease_Prediction

### Objective
- The objective of this project is to develop a predictive model to accurately identify the presence of heart disease in patients using various machine learning algorithms. By analyzing patient data, we aim to assist healthcare professionals in making informed decisions and improve patient outcomes through early detection and intervention.![image](https://github.com/user-attachments/assets/a6d8ef2c-d52a-4cb3-a26e-edb3635bc9bf)

### Dataset

The dataset contains 14 features and a binary target variable indicating the presence or absence of heart disease. The features include:

‣ age: Age of the patient

‣ sex: Gender of the patient

‣ cp: Chest pain type

‣ trestbps: Resting blood pressure

‣ chol: Serum cholesterol in mg/dl

‣ fbs: Fasting blood sugar > 120 mg/dl

‣ restecg: Resting electrocardiographic results

‣ thalach: Maximum heart rate achieved

‣ exang: Exercise induced angina

‣ oldpeak: ST depression induced by exercise

‣ slope: Slope of the peak exercise ST segment

‣ ca: Number of major vessels colored by fluoroscopy

‣ thal: Thalassemia

‣ target: Presence of heart disease (1) or absence (0)

### Data wrangling

1. Missing Values: There are no missing values in the dataset. 

2. Summary Statistics:

‣ The dataset has a mix of categorical (e.g., sex, cp, fbs, etc.) and continuous  variables
(e.g., age, trestbps, chol, etc.).

‣ The values in the columns seem to be within reasonable ranges, but some columns like
ca (number of major vessels colored by fluoroscopy) have values up to 4.

3. Target Variable Distribution:
   
‣ 0 (absence of heart disease): 499 samples

‣ 1 (presence of heart disease): 526 samples 

‣ The dataset is relatively balanced between the two classes.

### Exploratory Data Analysis
![image](https://github.com/user-attachments/assets/1c3abbc8-72cd-4b9b-bc8a-249e1ce43413)

‣ The graph indicates the distribution of sex in the dataset: there are 713 males (69.6%) and 312 females (30.4%).

![age (2)](https://github.com/user-attachments/assets/825d9a7e-0c81-48ba-9601-913197691958)

‣  The graph indicates the distribution of age groups in the dataset: there are individuals 6.6% in the 'Younger' group, individuals 66.8% in the 'Middle' group, and individuals 26.5% in the 'Older' group.

![target](https://github.com/user-attachments/assets/9d41ba67-c596-4fa0-b4b0-3c673eb03e83)

![image](https://github.com/user-attachments/assets/8695e8d2-06cc-4efa-8413-422238a09cc2)

The distributions of the continuous variables show that:

‣ Age has a normal distribution, with most patients between 50 and 60 years old.

‣Resting blood pressure (trestbps) peaks around 120-140 mmHg.

‣ Cholesterol (chol) shows a right-skewed distribution, with most values between 200 and 300 mg/dL.

‣ Maximum heart rate (thalach) is normally distributed, peaking around 150 bpm.

‣ Oldpeak (ST depression induced by exercise) shows a right-skewed distribution, with most values
between 0 and 1.

![image](https://github.com/user-attachments/assets/704f11c0-67ce-4d5d-8c6f-6749e4efd455)

![image](https://github.com/user-attachments/assets/1c234afb-0954-467a-b566-1bca7adb4f30)

### Younger (Age < 40):

‣ Among the younger individuals, those without heart disease (target = 0) are more prevalent compared to those with heart disease (target = 1).

### Middle-aged (Age ≤ 60):

‣ There is a significant presence of heart disease (target = 1) in the middle-aged group, especially in the 50-60 age range. 

### Older (Age > 60):

‣ There is a noticeable number of older individuals with heart disease (target = 1), indicating that heart disease prevalence increases with age.

![correlation](https://github.com/user-attachments/assets/d131e95f-2cef-4ae4-beaf-62f5bb25a639)
![image](https://github.com/user-attachments/assets/58a0b1bc-a0ca-4c3c-a7c4-cd4adbeddf90)

‣ The correlation heatmap shows the relationships between different variables. In simple terms, it highlights that the strongest positive correlation with the target variable (heart disease) is with cp (chest pain type), while the strongest negative correlations are with exang (exercise-induced angina) and oldpeak (ST depression).

### Applied Machine Learning Algorithms:

![image](https://github.com/user-attachments/assets/5aea6044-c939-4941-8b1f-8e13c3d8f451)
![image](https://github.com/user-attachments/assets/f50d938e-7df6-446b-9c2f-8aee404c08c3)
![image](https://github.com/user-attachments/assets/14b3459e-5c01-4206-967b-3c731edf885f)
![image](https://github.com/user-attachments/assets/a4295d5c-3ad7-4c41-8d93-d528287e0263)
![image](https://github.com/user-attachments/assets/60f72dc4-b900-420f-beb2-dc7568176854)

* Accuracy: All models performed reasonably well, with Random Forest achieving the highest accuracy.
* Precision: Decision Tree & Random Forest have the highest precision, indicating they are better at predicting heart disease without many false positives.
* Recall: Random Forest has the highest recall, meaning it is better at identifying actual heart disease cases.
* F1-Score: Random Forest has the highest F1-score, indicating a good balance between precision and recall.
### ROC Curves
![download](https://github.com/user-attachments/assets/07c8b498-050a-4158-a0a7-a539d6542b88)

## **Conclusion:**

  * The heart disease prediction model developed through this project is a powerful tool for early diagnosis. By leveraging machine learning techniques, we can significantly aid medical professionals in making informed decisions, ultimately improving patient outcomes. The insights gained from this project highlight the importance of certain features in predicting heart disease, and the balanced dataset ensures reliable performance. Future work can enhance the model further, making it even more valuable in a clinical setting.

## **Healthcare Implications:**

  *  Regular screening for heart disease is crucial, especially for those between Middle-aged 50 and 60 years old.

  *  Monitoring and managing cholesterol, blood pressure, and exercise-induced ST depression can be effective preventative measures.

  *  Utilizing predictive models like Random Forest and Decision Tree can help in early detection and timely intervention for heart disease, potentially improving patient outcomes.

## Power BI Dashboard Overview

![image](https://github.com/user-attachments/assets/d9dde698-4605-4f71-b197-386c6d3f20e4)

