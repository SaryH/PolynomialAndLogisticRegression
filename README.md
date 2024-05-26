Polynomial and Logistic Regression Model Selection and Hyperparameter Tuning

This project focuses on model selection and hyperparameter tuning for both regression and classification tasks. It utilizes a provided dataset to perform polynomial and ridge regression as well as logistic regression, exploring various degrees of polynomial functions and regularization parameters to optimize model performance.

Dataset

The project involves two primary datasets:

data_reg.csv: Contains 200 examples with two attributes (x1, x2) and a continuous target label (y).

train_cls.csv and test_cls.csv: Used for binary classification tasks, with training and testing examples provided separately.

Tasks and Methodology

Polynomial Regression

Data Splitting and Visualization:

The data is split into training (120 examples), validation (40 examples), and testing sets (40 examples).

A 3D scatter plot is created to visualize the examples from each set, with different colors representing each set.

Model Training and Validation:

Polynomial regression models are trained with degrees ranging from 1 to 10.

Validation error is plotted against polynomial degree to determine the optimal degree.

For each polynomial model, the surface of the learned function is plotted alongside the training examples.

Ridge Regression:

Ridge regression is applied to a polynomial of degree 8.

Various regularization parameters ({0.001, 0.005, 0.01, 0.1, 10}) are tested to find the best value.

Mean Squared Error (MSE) on the validation set is plotted against the regularization parameter.

Logistic Regression

Linear Decision Boundary:

A logistic regression model with a linear decision boundary is trained using the training set.

The decision boundary is visualized on a scatter plot of the training examples.

Training and testing accuracy of the model are computed.

Quadratic Decision Boundary:

The logistic regression model is retrained with a quadratic decision boundary.

The new decision boundary is visualized, and training and testing accuracies are compared with the linear model.

Model Evaluation:

Comparison of the linear and quadratic models in terms of overfitting and underfitting.

Analysis of the impact of model complexity on performance.

Results and Analysis

Optimal Polynomial Degree: Determined based on the validation error curve.

Best Regularization Parameter: Selected by evaluating the MSE on the validation set.
Logistic Regression Performance: Comparison of linear and quadratic decision boundaries to assess model fit and accuracy.
Conclusion
The project provides a comprehensive exploration of model selection and hyperparameter tuning techniques. It highlights the importance of balancing model complexity and regularization to achieve optimal performance in both regression and classification tasks.

Future Work
Further investigation could include testing additional models, expanding the dataset, and applying cross-validation techniques to enhance the robustness of the results.
