# Tune-Hyperparameters

Hyperparameter Tuning for Cyclist Traffic Prediction Models

1. Introduction

Cycling has become an integral part of urban transportation systems, emphasizing the need for accurate predictive models to manage cyclist traffic effectively. This report presents a detailed exploration of hyperparameter tuning techniques applied to two machine learning algorithms: Random Forest Regressor and the Gradient Boosting Regressor. The objective was to enhance the predictive accuracy of these models using Grid Search, a powerful hyperparameter tuning method.

2. Data Preparation

The analysis began with a thorough preprocessing of the dataset, which included handling missing values, converting date features, encoding categorical variables, and scaling numerical features. The refined dataset served as the foundation for training and evaluating the predictive models.

3. Hyperparameter Tuning

3.1 Random Forest Regressor:

Grid Search was employed to explore various hyperparameter combinations for the Random Forest Regressor. The following hyperparameters were tuned:

●	n_estimators: Number of trees in the forest.
●	max_depth: Maximum depth of the trees.
●	min_samples_split: Minimum number of samples required to split an internal node.

The best combination of hyperparameters, determined through Grid Search, resulted in significant improvements in the Random Forest Regressor's predictive performance:

●	Mean Squared Error (MSE): 738304.46

●	R-Squared (R2): 0.9208

Best Hyperparameters:

●	n_estimators: 100
●	max_depth: None
●	min_samples_split: 2

3.2 Gradient Boosting Regressor:

Similar to the Random Forest Regressor, the Gradient Boosting Regressor underwent Grid Search to optimize its performance. The following hyperparameters were tuned:

●	n_estimators: Number of boosting stages to be run.
●	max_depth: Maximum depth of the individual regression estimators.
●	learning_rate: Step size shrinkage used to prevent overfitting.

Grid Search led to the discovery of an optimal set of hyperparameters, enhancing the Gradient Boosting Regressor's accuracy significantly:

●	Mean Squared Error (MSE): 383235.31
●	R-Squared (R2): 0.9589

Best Hyperparameters:

●	n_estimators: 150
●	max_depth: 7
●	learning_rate: 0.1

4. Model Evaluation:

Following hyperparameter tuning, both models were refit with the optimal parameters and evaluated on the test dataset.

4.1 Random Forest Regressor Metrics:

●	Mean Squared Error (MSE): 738304.46
●	R-Squared (R2): 0.9208

4.2 Gradient Boosting Regressor Metrics:

●	Mean Squared Error (MSE): 383235.31
●	R-Squared (R2): 0.9589

5. Conclusion

Hyperparameter tuning through Grid Search substantially improved the predictive accuracy of both the Random Forest Regressor and the Gradient Boosting Regressor. The optimized models, with their enhanced ability to forecast cyclist traffic patterns, hold great promise for urban planning applications. The report emphasizes the importance of rigorous hyperparameter tuning in maximizing the potential of machine learning models.

