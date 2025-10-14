# Thyroid Cancer Risk Prediction

## Project Overview
This project focuses on predicting thyroid cancer risk (benign vs malignant) using machine learning. It leverages patient data such as age, gender, family history, and clinical measurements to make predictions. Several machine learning models, including Logistic Regression, Random Forest, Gradient Boosting, AdaBoost, and Decision Tree, were evaluated to determine the best model for prediction. The project aims to assist healthcare providers in making more accurate and timely decisions for thyroid cancer diagnosis and treatment.

## Dataset
The dataset used consists of 212,691 anonymized patient records. It includes demographic, clinical, and biochemical data, such as:

- **Age**
- **Gender**
- **Family History of Thyroid Disease**
- **Thyroid-Stimulating Hormone (TSH) Levels**
- **Triiodothyronine (T3) and Thyroxin (T4) Levels**
- **Diagnosis (Benign or Malignant)**

The dataset was preprocessed to handle missing values, encode categorical variables, and scale numerical features.

## Preprocessing
- **Handling Missing Values:** Used median for numerical data and mode for categorical variables.
- **Encoding Categorical Variables:** Applied label encoding and one-hot encoding.
- **Feature Scaling:** Normalized numerical features to ensure balanced model training.
- **Train-Test Split:** The dataset was split into an 80% training set and a 20% testing set, using stratified sampling.

## Models Implemented
The following machine learning algorithms were implemented and evaluated:

- **Logistic Regression**
- **Random Forest**
- **Gradient Boosting**
- **AdaBoost**
- **Decision Tree**
- **Naive Bayes**
- **XGBoost**
- **LightGBM**

Models were trained on the training set, and their performance was evaluated based on Accuracy, Precision, Recall, and F1-Score.

## Results
- **Top-performing models:** Logistic Regression, Gradient Boosting, and AdaBoost achieved an accuracy of approximately 82.5%.
- **Underperforming model:** Decision Tree had an accuracy of 70.2%, showing overfitting on the training data.

## Clinical Integration
Machine learning models like Logistic Regression and boosting algorithms (XGBoost, AdaBoost) show promise in supporting clinical decisions for thyroid cancer diagnosis. The integration of such models into clinical workflows could help doctors identify high-risk patients, enabling early diagnosis and personalized treatment.

## Future Work
- Optimize hyperparameters using advanced techniques.
- Explore deep learning methods for complex pattern recognition.
- Address class imbalance using techniques like SMOTE.
- Implement real-time integration with Electronic Health Records (EHRs).

## Installation
To run the project, clone the repository and install the required libraries.

```bash
git clone https://github.com/yourusername/thyroid-cancer-risk-prediction.git
cd thyroid-cancer-risk-prediction
pip install -r requirements.txt
