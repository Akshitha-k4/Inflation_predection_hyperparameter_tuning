# Inflation_predection_hyperparameter_tuning
K Akshitha (2024) published research explores Inflation predection using machine learning.(plese do not copy)As the paper is copyrighted under IEEE. This code is provided as a learning resource. Feel free to suggest improvements! You can run it in any Python IDE.

**Introduction**

This project investigates the effectiveness of various machine learning algorithms for regression tasks, specifically in predicting inflation rates. The study employs a comprehensive dataset encompassing inflation data for multiple countries from 1970 to 2022.

**Methodology**

Several regression models are evaluated, including:

- Linear Regression
- Ridge Regression
- Lasso Regression
- Elastic Net
- KNN Regression
- Support Vector Regressor
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting

Mean Squared Error (MSE) serves as the primary metric for model comparison.

**Results**

The analysis reveals Gradient Boosting as the most proficient model, exhibiting resilience to outliers and delivering predictions closely aligned with real-world values. To further enhance its performance, hyperparameter tuning is applied using techniques like RandomSearchCV and GridSearchCV.

**Hyperparameter Tuning**

Gradient Boosting's hyperparameters explored include:

- `subsample`
- `n_estimators`
- `min_samples_split`
- `min_samples_leaf`
- `max_features`
- `max_depth`
- `learning_rate`

RandomSearchCV identifies the following optimal parameters:

```
{'subsample': 1.0, 'n_estimators': 100, 'min_samples_split': 10, 'min_samples_leaf': 2, 'max_features': 1.0, 'max_depth': 20, 'learning_rate': 0.01}
```

This configuration yields a superior score of 0.3381441665956274.

GridSearchCV, on the other hand, suggests the following optimal parameters:

```
{'learning_rate': 0.1, 'max_depth': 20, 'max_features': 1.0, 'min_samples_leaf': 1, 'min_samples_split': 2, 'n_estimators': 200, 'subsample': 0.5}
```

However, this configuration results in a higher MSE of 326.4495832586182.

**Conclusion**

The study demonstrates that Gradient Boosting is a powerful tool for inflation rate prediction. Hyperparameter tuning can significantly improve its accuracy.

**Future Work**

Potential areas for further exploration include:

- Incorporation of additional features that might influence inflation rates.
- Investigation of more advanced machine learning algorithms.
- Evaluation of the model's performance on more recent data.

I hope this refined README file effectively summarizes the project's key points!
