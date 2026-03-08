# DDS-8555-ChandlerJ-Assignment 5 and 6

# Executive Summary for Classification Methods
This assignment evaluated classification methods across two tasks. Logistic regression theory was demonstrated by showing the equivalence of the logistic and logit forms. Multiple classifiers were then compared on the ISLP Weekly dataset to predict market Direction using both the full feature set and a 1990–2008 training split with 2009–2010 holdout testing. Finally, four multi-class models were developed for the Kaggle obesity-risk dataset using consistent preprocessing and comparative evaluation. Across both datasets, results showed that predictive signal and appropriate assumptions matter more than model complexity, and that simpler models can perform competitively when signal strength is limited.
## Key Insights
* On the Weekly dataset, predictive signal was weak. Lag2 was the only statistically significant predictor in the full logistic regression, and logistic regression (Lag2) and LDA (Lag2) achieved the best holdout accuracy at 62.5%, with stronger identification of “Up” weeks than “Down” weeks.
* Increasing complexity on Weekly did not improve results. QDA and Naive Bayes performed slightly worse than linear classifiers, while KNN (k = 1) performed near chance, indicating limited benefit from nonlinear flexibility.
* For the Kaggle obesity-risk task, four complementary frameworks were implemented: regularized multinomial logistic regression, LDA, Naive Bayes, and an RBF SVM. Results emphasized disciplined preprocessing, model comparison, and the balance between interpretability and flexibility for multi-class classification.

# Executive Summary for Tree-Based Modeling and Ensemble Methods for Multi-Class Prediction
This assignment addressed two conceptual and applied problems in tree-based statistical learning. The first task involved constructing an original recursive binary partition of two-dimensional feature space with six regions and its corresponding decision tree. The second applied boosting, bagging, random forests, and a single decision tree to the Boston housing dataset, comparing their predictive performance against a linear regression baseline. Additionally, four tree-based models—a decision tree, a bagged ensemble, a random forest, and a gradient boosted classifier—were developed and submitted to the Kaggle Multi-Class Prediction of Obesity Risk competition. Across all contexts, ensemble methods consistently outperformed single-tree models, and gradient boosting achieved the strongest predictive performance. Random forests offered a strong balance of accuracy and interpretability through variable importance.

## Key Insights
* Ensemble methods (bagging, random forest, boosting) substantially outperform single decision trees in both applied tasks, consistent with the bias-variance tradeoff framework in statistical learning.
* Gradient boosting achieved the highest accuracy in the Kaggle obesity risk competition, while random forests provided competitive performance with interpretable variable importance rankings.
* Tree-based methods require minimal preprocessing assumptions and handle mixed predictor types naturally, making them well-suited for complex multi-class classification tasks with behavioral and demographic predictors.

```
DDS-8555-ChandlerJ-Assignment-5-and-6/
│
├── README.md
├── ChandlerJ_DDS-8555-Assignment5.Rmd
├── ChandlerJ_DDS-8555-Assignment5.docx
├── ChandlerJ_DDS-8555-Assignment6.Rmd
├── ChandlerJ_DDS-8555-Assignment6.docx
├── notebooks/
│   ├── ChandlerJ_DDS-8555-Assignment5.ipynb
│   └── ChandlerJ_DDS-8555-Assignment6.ipynb
├── submissions/
│   ├── kaggle_submission_Chandler_logit_regularized.csv
│   ├── kaggle_submission_Chandler_lda.csv
│   ├── kaggle_submission_Chandler_naive_bayes.csv
│   ├── kaggle_submission_Chandler_svm.csv
│   ├── kaggle_submission_Chandler_random_forest.csv
│   ├── kaggle_submission_Chandler_gradient_boosting.csv
│   ├── kaggle_submission_Chandler_decision_tree.csv
    └── kaggle_submission_Chandler_bagging.csv
```
