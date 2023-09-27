## Logistic Regression Interview Questions

1. **What is Logistic Regression?**
   - Logistic regression is a statistical model used for binary classification, where the goal is to predict the probability that an input belongs to one of two possible classes.

2. **How does Logistic Regression differ from Linear Regression?**
   - In linear regression, the output is a continuous numeric value, while in logistic regression, the output is a probability score between 0 and 1, which can be interpreted as the likelihood of belonging to a particular class.

3. **What is the Sigmoid (Logistic) Function in Logistic Regression?**
   - The sigmoid function is an "S"-shaped curve that maps any real-valued number to a value between 0 and 1. In logistic regression, this function is used to transform the linear combination of inputs into a probability score.

4. **What are the Assumptions of Logistic Regression?**
   - Logistic regression assumes that the relationship between the independent variables and the log-odds of the dependent variable is linear. It also assumes that the errors are independent and follow a logistic distribution.

5. **What is the Log-Odds Ratio in Logistic Regression?**
   - The log-odds, also known as the logit, is the natural logarithm of the odds of the event occurring. In logistic regression, it's used to linearize the relationship between the predictors and the response variable.

6. **How is a Logistic Regression Model Trained?**
   - Logistic regression models are typically trained using an optimization algorithm like gradient descent. The algorithm adjusts the model parameters (coefficients) to minimize the logistic loss function.

7. **What is the Cost Function in Logistic Regression?**
   - The cost function (also called the logistic loss or cross-entropy loss) measures the difference between the predicted probabilities and the actual class labels. The goal is to minimize this cost function during training.

8. **How do you Interpret the Coefficients in Logistic Regression?**
   - The coefficients in logistic regression represent the change in the log-odds of the dependent variable for a one-unit change in the corresponding independent variable. They can be exponentiated to interpret their effect on the odds ratio.

9. **What is Overfitting in Logistic Regression, and How Can it be Prevented?**
   - Overfitting occurs when a model fits the training data too closely and performs poorly on unseen data. Regularization techniques, like L1 or L2 regularization, can be applied to prevent overfitting.

10. **What is ROC Curve, and Why is it Used in Logistic Regression?**
    - The ROC curve is a graphical representation of the model's performance across different probability thresholds. It helps assess the trade-off between true positive rate and false positive rate.

11. **What is AUC-ROC, and How is it Interpreted?**
    - The Area Under the ROC Curve (AUC-ROC) quantifies the model's ability to distinguish between the two classes. An AUC-ROC of 0.5 indicates random guessing, while an AUC-ROC of 1 indicates perfect classification.

12. **What are Confusion Matrix, Precision, Recall, and F1-Score in Binary Classification?**
    - The confusion matrix is a table that shows the true positive, true negative, false positive, and false negative classifications. Precision, recall, and the F1-score are metrics derived from the confusion matrix that assess the model's performance.

13. **How do you Handle Imbalanced Data in Logistic Regression?**
    - Imbalanced datasets occur when one class has significantly fewer samples than the other. Techniques like oversampling the minority class, undersampling the majority class, or using appropriate evaluation metrics can address this issue.

14. **What are the Advantages and Disadvantages of Logistic Regression?**
    - Advantages include simplicity, interpretability, and the ability to model probabilities. Disadvantages include sensitivity to outliers and the assumption of linearity.

15. **Provide an Example of a Real-World Application of Logistic Regression.**
    - A real-world example could be predicting whether an email is spam or not spam based on its content and features, which is a classic binary classification problem.
