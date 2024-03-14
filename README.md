
# Heart Disease Prediction Model

This repository contains code for a machine learning model designed to predict the likelihood of heart disease in patients based on various medical attributes.

## Dataset

The dataset used for training and evaluation is stored in `dataset.csv`. It contains the following attributes:

- `age`: Age of the patient.
- `sex`: Gender of the patient (0 for female, 1 for male).
- `cp`: Chest pain type.
- `trestbps`: Resting blood pressure (in mm Hg).
- `chol`: Serum cholesterol level (in mg/dl).
- `fbs`: Fasting blood sugar > 120 mg/dl (1 for true, 0 for false).
- `restecg`: Resting electrocardiographic results.
- `thalach`: Maximum heart rate achieved.
- `exang`: Exercise induced angina (1 for true, 0 for false).
- `oldpeak`: ST depression induced by exercise relative to rest.
- `slope`: The slope of the peak exercise ST segment.
- `ca`: Number of major vessels colored by fluoroscopy.
- `thal`: Thalassemia.

The target variable is `target`, which indicates whether the patient has heart disease (1 for true, 0 for false).

## Model Training

The model was trained using three different classifiers:

1. **K-Nearest Neighbors (KNN) Classifier**: The optimal value of K was determined using cross-validation.
2. **Random Forest Classifier**: Ensemble learning method using decision trees.
3. **Decision Tree Classifier**: A single decision tree for classification.

The dataset was preprocessed by encoding categorical variables and scaling numerical features using standard scaling.

## Evaluation

The models were evaluated using cross-validation to assess their performance. Mean accuracy scores were computed for each classifier to compare their effectiveness in predicting heart disease.

## Usage

To use the trained KNN classifier for predicting heart disease on new data:

1. Ensure Python and required libraries are installed.
2. Clone this repository.
3. Place your new dataset in CSV format and update the file path in the code accordingly.
4. Run the provided code in a Python environment.
5. The predictions will be displayed, indicating whether each patient is predicted to have heart disease (1) or not (0).

