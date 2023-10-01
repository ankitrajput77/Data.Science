# Ensemble techniques 
- In machine learning involve combining multiple individual models (often called "base models" or "weak learners") to create a more robust and accurate predictive model. The idea behind ensemble methods is that by aggregating the predictions or decisions of multiple models, the overall performance can be improved compared to using a single model. Ensemble techniques are commonly used for both classification and regression problems. Here are some popular ensemble techniques:

## Bagging (Bootstrap Aggregating): 
Bagging is an ensemble technique that creates multiple base models by training them on different subsets of the training data. Each base model is trained independently, and their predictions are combined through averaging (for regression) or voting (for classification). Random Forest is a well-known ensemble method that uses bagging with decision trees as its base models.

![image](https://github.com/ankitrajput77/Data.Science/assets/113281225/f9d93ebd-ede9-4ee3-860d-679c2fd5351f)

## Boosting: 
Boosting is an ensemble technique that combines multiple base models sequentially. It focuses on training each new base model to correct the mistakes made by the previous models. Common boosting algorithms include AdaBoost, Gradient Boosting (e.g., XGBoost, LightGBM), and CatBoost.

## Stacking (Stacked Generalization): 
Stacking involves training multiple diverse base models and then training a "meta-model" (often a simple model like logistic regression) on top of the base models' predictions. The meta-model learns to combine the base models' outputs to make the final prediction. Stacking can capture different aspects of the data and often leads to improved performance.

## Voting: 
Voting ensembles combine the predictions of multiple base models by taking a majority vote (for classification) or averaging (for regression). There are three main types of voting ensembles:

### Hard Voting: 
Each base model's prediction is treated as a vote, and the class with the most votes is the final prediction (for classification).
### Soft Voting: 
Base models' predicted probabilities are averaged, and the class with the highest average probability is selected as the final prediction (for classification).
### Regression Averaging: 
For regression problems, base models' predictions are averaged to obtain the final prediction.
## Weighted Averaging: Similar to voting, this ensemble technique combines base models' predictions by assigning different weights to each model's output. The weights are often determined based on the performance of the individual models on a validation set.

## Adaptive Boosting (AdaBoost): AdaBoost is a boosting algorithm that assigns weights to data points and focuses on the samples that were misclassified by previous base models. It iteratively trains new base models, adjusting the weights to give more emphasis to difficult-to-classify examples.

- Ensemble techniques are effective because they harness the diversity and complementary strengths of multiple models. By combining their predictions, ensemble methods can often achieve higher accuracy, better generalization, and improved robustness to noisy or outlier data compared to individual models. However, they may also require more computational resources and tuning to optimize their performance. The choice of ensemble technique and the selection of base models should be guided by the characteristics of the specific problem and dataset.
