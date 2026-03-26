# Student Performance Prediction 🎓

![Python](https://img.shields.io/badge/Python-3.9+-blue?style=flat-square&logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange?style=flat-square&logo=scikit-learn)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat-square)

> Predicting student academic performance using supervised machine learning.
> Vikram Kumar — BS Data Science, Sindh University

---

## Overview

This project uses Linear Regression and Decision Tree Regression to predict
a student's overall score based on study habits, attendance, subject scores,
and demographic features.

---

## Dataset

| Detail  | Info                                  |
|---------|---------------------------------------|
| File    | Student_Performance.csv               |
| Records | 395+ students                         |
| Target  | overall_score (0–100)                 |

### Features Used

| Feature                | Type        | Description                    |
|------------------------|-------------|--------------------------------|
| study_hours            | Numeric     | Weekly study hours             |
| attendance_percentage  | Numeric     | % of classes attended          |
| math_score             | Numeric     | Math exam score                |
| science_score          | Numeric     | Science exam score             |
| english_score          | Numeric     | English exam score             |
| internet_access        | Categorical | Home internet (yes/no)         |
| extra_activities       | Categorical | Extracurricular participation  |
| parent_education       | Categorical | Parental education level       |

---

## Project Structure

student-performance-prediction/
├── Student_Performance.csv
├── Student_Performance_Prediction.ipynb
├── requirements.txt
└── README.md

---

## Notebook Sections

| # | Section              | Description                              |
|---|----------------------|------------------------------------------|
| 1 | Import Libraries     | pandas, numpy, sklearn, seaborn          |
| 2 | Load & Explore       | shape, info, describe, missing values    |
| 3 | EDA                  | 4 visualizations — distributions         |
| 4 | Feature Engineering  | Label encoding + correlation heatmap    |
| 5 | Train/Test Split     | 80/20 split, random_state=42            |
| 6 | Train Models         | Linear Regression + Decision Tree        |
| 7 | Evaluate             | MAE, MSE, RMSE, R²                       |
| 8 | Visualize            | Actual vs Predicted + Residual plots     |
| 9 | Predict              | Live prediction clipped to 0–100         |
| 10| Conclusion           | Key findings and next steps              |

---

## Results

| Model              | MAE  | RMSE | R²   |
|--------------------|------|------|------|
| Linear Regression  | ~6.5 | ~8.0 | ~0.82|
| Decision Tree      | ~5.8 | ~7.4 | ~0.86|

---

## Key Findings

- Study hours and subject scores are the strongest predictors
- Attendance has a moderate positive effect on performance
- Students with internet access slightly outperform those without
- Parental education level correlates with higher scores
- Output is clipped to 0–100 to prevent impossible predictions

---

## How to Run

git clone https://github.com/vikramkumar/student-performance-prediction.git
cd student-performance-prediction
pip install -r requirements.txt
jupyter notebook Student_Performance_Prediction.ipynb

---

## Requirements

pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter

---

## Future Improvements

- [ ] Try Random Forest and XGBoost
- [ ] Add k-fold cross-validation
- [ ] Build a Streamlit web app
- [ ] Deploy as a REST API using Flask

---

## Author

Vikram Kumar
BS Data Science — Sindh University
GitHub: https://github.com/vikramkumar

---

## License

MIT License
