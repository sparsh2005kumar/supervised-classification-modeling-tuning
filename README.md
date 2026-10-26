# Supervised Classification / Regression Modeling & Tuning

## Contents
- `supervised-classification-modeling-tuning.ipynb`: complete runnable classification workflow.
- `README.md`: project instructions.

## Features
- Four model families: Logistic Regression, Random Forest, Extra Trees, Gradient Boosting.
- `GridSearchCV` with stratified 5-fold cross-validation.
- Leak-free imputation/scaling inside a Scikit-Learn `Pipeline` and `ColumnTransformer`.
- Model comparison table with precision, recall, F1, ROC-AUC, accuracy, and balanced accuracy.
- ROC curves and confusion matrices.
- Champion selection by mean CV ROC-AUC.
- Serialization to `champion_model.joblib`.

## Run
Install dependencies:
```bash
python -m pip install pandas numpy matplotlib scikit-learn joblib jupyter
```
Open the notebook in Jupyter or VS Code and run cells in order. The notebook creates `champion_model.joblib` in the working directory when its serialization cell runs.

## Dataset limitation
The task screenshot did not provide a dataset, so this notebook generates a reproducible synthetic dataset. All scores are for demonstration only. Replace the synthetic data cell with a documented and permitted real dataset if required by the task.
