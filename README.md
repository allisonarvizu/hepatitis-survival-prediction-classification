# Hepatitis Survival Prediction Using Classification Models

This project explores a supervised classification problem focused on predicting patient
survival outcomes following a hepatitis infection. Multiple machine learning classifiers
were built and evaluated to compare predictive performance across different modeling
approaches.

The analysis emphasizes model evaluation beyond accuracy, examines the impact of
hyperparameter tuning, and assesses whether ensemble methods improve performance.

---

## Project Overview

The dataset contains patient-level medical information, including a combination of
numerical and categorical clinical features. Separate training and testing datasets
were used to evaluate how well models generalize to unseen data.

The primary objective of this project is to compare individual classification models,
a hyperparameter-tuned model, and a stacking ensemble using standard classification
metrics.

---

## Models Implemented

The following classification models were evaluated using default settings:

- Linear Support Vector Classifier (LinearSVC)
- Decision Tree Classifier
- Random Forest Classifier
- K-Nearest Neighbors Classifier

To improve performance, hyperparameter tuning was performed on the Random Forest
classifier using randomized search with cross-validation.

In addition, a one-layer stacking ensemble was constructed by combining predictions
from the four base classifiers, using a Multilayer Perceptron (MLP) as the meta-learner.

---

## Evaluation Metrics

Model performance was evaluated using multiple metrics to provide a comprehensive
comparison:

- Accuracy
- Precision
- Recall
- F1 Score

These metrics help capture different aspects of model behavior, particularly in cases
where class imbalance may influence results.

---

## Feature Importance

Feature importance scores from the tuned Random Forest model were analyzed to identify
which clinical variables contributed most strongly to model predictions. This analysis
provides insight into factors associated with hepatitis survival outcomes.

---

## Key Takeaways

This project highlights the trade-offs between model complexity and predictive
performance. Hyperparameter tuning improved the Random Forest model across select
metrics, while ensemble learning was used to assess whether combining diverse classifiers
could further enhance results.

Future work could explore additional feature engineering, alternative ensemble
strategies, or methods for addressing potential class imbalance.

---

## Technologies Used

- Python
- pandas
- NumPy
- scikit-learn
