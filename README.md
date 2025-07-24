# Stroke Prediction with Machine Learning

## Overview
This project aims to predict the likelihood of stroke occurrence based on patient health data using a variety of machine learning models. The dataset used contains patient information such as age, BMI, glucose level, and lifestyle habits. The project includes data preprocessing, feature engineering, and model performance comparison.

## Key Features
- **Data Preprocessing**:
  - Removal of irrelevant columns (e.g., patient ID).
  - Imputation of missing BMI values using the median within stroke groups.
  - Encoding categorical variables with one-hot encoding.

- **Feature Engineering**:
  - Creation of age groups (Child, Young Adult, Middle-aged, Senior, Elderly).
  - Categorization of BMI into Underweight, Normal, Overweight, and Obese.

- **Class Imbalance Handling**:
  - Use of **SMOTE (Synthetic Minority Over-sampling Technique)** to balance the stroke and non-stroke classes.

- **Models Implemented**:
  - Random Forest
  - Logistic Regression
  - Decision Tree
  - Deep Learning Neural Network (Keras)

- **Evaluation Metrics**:
  - AUC (Area Under Curve)
  - Accuracy, Precision, Recall
  - F1-score
  - Confusion Matrices

## Results
A summary table of metrics is generated for all models, allowing easy comparison of their predictive performance.  
Sample results include:  
- **Random Forest:** AUC ≈ 0.755, Accuracy ≈ 0.93  
- **Logistic Regression:** AUC ≈ 0.779, Recall ≈ 0.48  
- **Deep Learning:** AUC ≈ 0.765

## Dependencies
- Python 3.x
- Pandas, NumPy, Matplotlib, Seaborn
- scikit-learn
- imbalanced-learn (for SMOTE)
- TensorFlow/Keras (for Deep Learning)

## How to Run
1. Clone this repository.
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the notebook `Prediction model of Stroke.ipynb`.
4. Run all cells to preprocess the data, train models, and view results.

## Future Improvements
- Hyperparameter tuning for each model.
- Integration of cross-validation for robust performance evaluation.
- Deployment of the best-performing model as an API.
