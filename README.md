This project aims to classify drugs based on patient physiological features using supervised machine learning models. The dataset contains medical attributes such as age, sex, blood pressure (BP), cholesterol level, and sodium-to-potassium ratio. The model predicts the most appropriate drug (out of 5 possible classes) for a patient.

Problem Type: Multi-class classification
ML models used : Logistic Regression, KNN, Decision Tree, Random forest
Number of Classes: 5 (DrugA, DrugB, DrugC, DrugX, DrugY)
Input Features: Age, Sex, Blood Pressure (BP), Cholesterol, Na-to-K ratio

Approach
- Data Preprocessing: Used one-hot encoding on categorical features and StandardScaler for numerical features
- Models Used: Custom ML classifiers implemented using sklearn. No use of deep learning.
- Finding best model using Evaluation Metrics: 5-fold cross validation and Confusion Matrix on all models to get best model, Accuracy, Classification Report with y_pred and y_test.
- Performed Feature imporatance and SHAP to know which feature contributes and how much in the classification of the drugs.

Dataset: The dataset is a commonly used UCI Drug Classification dataset. It includes patient-level features and labels corresponding to the drug class prescribed.

Result : 
- Best model was found out to b Logistic Regression with 0.918 accuracy in 5 fold cross validation, 0.975 in test accuracy, AUC 1.
- Visualization of Class distribution of features in dataset, Accuracy of different models, Confusion matrices, ROC curve for Logistic Regression and SHAP summary plots for different classes
