# Predictive Modeling Using Machine Learning
**Internship Task 2 - Data Science Domain**

## Objective
Build and evaluate machine learning models that predict an outcome from data, and visualize performance with confusion matrices and ROC curves.

## Problem
Classify breast tumors as **malignant or benign** from 30 cell-nucleus measurements (Breast Cancer Wisconsin dataset, 569 samples, bundled with scikit-learn).

## Models compared
Logistic Regression, Decision Tree, Random Forest (tuned with GridSearchCV).

## Results (test set, 114 samples)
| Model | Accuracy | Precision | Recall | F1 | ROC-AUC |
|---|---|---|---|---|---|
| Logistic Regression | 0.9825 | 0.9861 | 0.9861 | 0.9861 | 0.9954 |
| Decision Tree | 0.9211 | 0.9565 | 0.9167 | 0.9362 | 0.9163 |
| Random Forest | 0.9561 | 0.9589 | 0.9722 | 0.9655 | 0.9931 |

5-fold cross-validation gives the same ranking. Top Random Forest features: worst perimeter, worst radius, worst concave points, worst area, mean concave points.

## Files
| File | Description |
|---|---|
| `Predictive_Modeling_ML.ipynb` | Full executed notebook (EDA, training, evaluation, tuning) |
| `Predictive_Modeling_Report.html` | Static export of the notebook, viewable in any browser |
| `Final_Report_Task2.docx` | Written report |
| `model_results.csv` | Metrics table |
| `charts/` | Confusion matrices, ROC curves, feature importance and other figures |

## How to run
```
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook Predictive_Modeling_ML.ipynb
```
The dataset loads directly from scikit-learn, so no download is needed.

## Tools
Python, Pandas, NumPy, scikit-learn, Matplotlib, Seaborn
