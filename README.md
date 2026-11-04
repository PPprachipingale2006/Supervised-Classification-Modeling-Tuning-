# Supervised Classification Modeling & Tuning

## Project Overview

This project focuses on implementing supervised machine learning classification algorithms using the Titanic dataset.

The main objective is to predict passenger survival based on passenger information using multiple machine learning models, hyperparameter optimization, and performance evaluation.

## Project Objectives

- Train at least four different classification algorithms.
- Perform hyperparameter tuning using GridSearchCV.
- Apply Stratified 5-Fold Cross-Validation.
- Evaluate model performance using multiple metrics.
- Compare different classification algorithms.
- Select and save the best-performing model.

## Dataset Information

**Dataset:** Titanic Dataset (`titanic.csv`)

**Target Variable:** `Survived`

- 0 = Did not survive
- 1 = Survived

The dataset contains passenger information used to build the classification models.

## Machine Learning Algorithms

Four classification algorithms were implemented:

1. Logistic Regression
2. Random Forest Classifier
3. Support Vector Machine (SVM)
4. Histogram-Based Gradient Boosting Classifier

## Technologies and Libraries

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Joblib
- Jupyter Notebook

## Implementation Steps

1. Dataset loading and exploration.
2. Data cleaning and missing value handling.
3. Feature and target separation.
4. Training and testing data splitting.
5. Feature preprocessing using ColumnTransformer.
6. Numerical feature scaling.
7. Categorical feature encoding.
8. Model training using four algorithms.
9. Hyperparameter optimization using GridSearchCV.
10. Stratified 5-Fold Cross-Validation.
11. Model evaluation and comparison.
12. Champion model selection.
13. Model serialization using Joblib.

## Evaluation Metrics

The classification models were evaluated using:

| Metric | Description |
|---|---|
| Accuracy | Overall prediction correctness |
| Precision | Correct positive predictions |
| Recall | Actual positive cases identified |
| F1-Score | Balance between precision and recall |
| ROC-AUC | Ability to distinguish between classes |

A confusion matrix and ROC-AUC curves were also generated to visualize model performance.

## Hyperparameter Optimization

GridSearchCV was used to find the best hyperparameters for each classification algorithm.

Stratified 5-Fold Cross-Validation was applied to maintain class proportions across validation folds.

ROC-AUC was selected as the primary optimization metric.

## Project Structure

```text
Supervised-Classification-Modeling-Tuning/
│
├── titanic.csv
├── supervised_classification_modeling.ipynb
├── requirements.txt
├── README.md
│
└── outputs/
    ├── model_comparison.csv
    ├── roc_auc_comparison.png
    ├── confusion_matrix.png
    └── champion_model.joblib
```

## Installation and Execution

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/Supervised-Classification-Modeling-Tuning.git
```

### Step 2: Navigate to the Project Folder

```bash
cd Supervised-Classification-Modeling-Tuning
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Open Jupyter Notebook

```bash
jupyter notebook
```

Open `supervised_classification_modeling.ipynb` and run all cells in sequence.

## Project Outputs

The project generates:

- `model_comparison.csv` – Performance comparison of all four models.
- `roc_auc_comparison.png` – ROC-AUC curves for model evaluation.
- `confusion_matrix.png` – Visualization of classification predictions.
- `champion_model.joblib` – Saved best-performing classification pipeline.

## Model Selection

The champion model is selected based on the highest cross-validation ROC-AUC score.

The final test-set metrics are also calculated to evaluate the selected models on unseen data.

## Conclusion

This project demonstrates a complete supervised machine learning classification workflow, including data preprocessing, model training, hyperparameter optimization, model evaluation, comparison, and serialization.

It provides practical experience in applying machine learning algorithms to a real-world classification problem.

## Author

**Prachi Pingale**

Computer Science Student | Machine Learning Enthusiast