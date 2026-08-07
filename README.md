# Diabetes Readmission Prediction

This project develops and compares multiple machine learning models to predict hospital readmission using the Diabetes 130-US Hospitals dataset from the UCI Machine Learning Repository.

The project covers the complete machine learning workflow, including exploratory data analysis, data cleaning, preprocessing, feature engineering, model training, hyperparameter tuning, and model evaluation.

## Dataset

Source:
- UCI Machine Learning Repository
- Diabetes 130-US hospitals for years 1999–2008

The dataset contains over 100,000 hospital encounters from diabetic patients and aims to predict hospital readmission.

## Project Structure

├── data/
│   ├── raw/
│   └── processed/
├── models/
├── notebooks/
│   ├── 01_data_understanding.ipynb
│   ├── 02_exploratory_data_analysis.ipynb
│   ├── 03_data_cleaning.ipynb
│   ├── 04_preprocessing.ipynb
│   └── 05_modeling.ipynb
└── README.md

## Workflow

- Data Understanding
- Exploratory Data Analysis
- Data Cleaning
- Data Preprocessing
- Machine Learning Modeling
- Hyperparameter Tuning
- Model Comparison

## Models Evaluated

- Logistic Regression
- Decision Tree
- Random Forest
- Tuned Random Forest
- XGBoost
- Tuned XGBoost

## Main Findings

- Ensemble models outperformed the baseline models.
- Hyperparameter tuning improved the ability to detect minority classes.
- The tuned Random Forest achieved the best balance between overall performance and minority-class detection.
- Predicting readmission within 30 days remained challenging, suggesting that the available features only partially capture the factors associated with early readmission.

## Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn
- Jupyter Notebook

## Future Improvements

- Binary readmission prediction (readmitted vs not readmitted)
- Advanced feature engineering
- Cost-sensitive learning techniques


## Results

| Model                   | Accuracy | Macro F1 |
| ----------------------- | -------: | -------: |
| Logistic Regression     |     0.58 |     0.40 |
| Decision Tree           |     0.48 |     0.39 |
| Random Forest           |     0.57 |     0.44 |
| **Tuned Random Forest** | **0.55** | **0.46** |
| XGBoost                 |     0.58 |     0.40 |
| Tuned XGBoost           |     0.58 |     0.42 |
