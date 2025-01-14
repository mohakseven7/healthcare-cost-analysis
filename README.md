# Healthcare Cost Analysis and Forecasting

## Project Overview
This project aims to analyze and forecast healthcare costs using machine learning techniques, with a focus on predicting billing amounts based on various features such as patient age, length of stay, and room number.


## Project Description
This project explores a healthcare dataset to predict the billing amount for patients based on their age, length of stay, and room number. It involves data cleaning, exploratory data analysis (EDA), feature selection, and building a linear regression model for prediction.

## Technologies Used
- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebooks (for interactive development)
- Google Colab (for cloud execution)

## Dataset
The dataset `healthcare_dataset.csv` contains the following features:
- `age`: Age of the patient
- `date_of_admission`: Date the patient was admitted
- `discharge_date`: Date the patient was discharged
- `admission_type`: Type of admission (Emergency, Scheduled, etc.)
- `room_number`: Room number assigned to the patient
- `billing_amount`: Total billing amount for the patient
- `length_of_stay`: Number of days spent in the hospital (calculated from `date_of_admission` and `discharge_date`)

## Data Preprocessing
- Standardized column names.
- Converted date columns (`date_of_admission`, `discharge_date`) to datetime format.
- Calculated the length of stay in the hospital.
- Handled incorrect or missing values by replacing negative stays with the median value.

## Exploratory Data Analysis (EDA)
- **Age Distribution**: A histogram to understand the distribution of patient ages.
- **Correlation Heatmap**: A heatmap showing the correlation between numerical features in the dataset.
- **Billing Amount by Admission Type**: A boxplot showing the distribution of billing amounts by admission type.

## Predictive Model
- **Features**: The model uses `age`, `length_of_stay`, and `room_number` as predictors.
- **Target**: The target variable for prediction is `billing_amount`.
- **Model**: A Linear Regression model was trained to predict the billing amount.

## Model Evaluation
The model's performance was evaluated using:
- **Mean Squared Error (MSE)**: A measure of the average squared differences between predicted and actual values.
- **R-squared (R2) Score**: A measure of how well the model explains the variance in the target variable.

The final model is saved as `billing_prediction_model.pkl` and can be used for future predictions.

## Installation
To install the required dependencies, clone this repository and run the following command:


