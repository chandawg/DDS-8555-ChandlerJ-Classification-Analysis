# DDS-8555-ChandlerJ-Classification-Analysis

# Executive Summary
This assignment evaluated classification methods across two tasks. Logistic regression theory was demonstrated by showing the equivalence of the logistic and logit forms. Multiple classifiers were then compared on the ISLP Weekly dataset to predict market Direction using both the full feature set and a 1990–2008 training split with 2009–2010 holdout testing. Finally, four multi-class models were developed for the Kaggle obesity-risk dataset using consistent preprocessing and comparative evaluation. Across both datasets, results showed that predictive signal and appropriate assumptions matter more than model complexity, and that simpler models can perform competitively when signal strength is limited.
## Key Insights
* On the Weekly dataset, predictive signal was weak. Lag2 was the only statistically significant predictor in the full logistic regression, and logistic regression (Lag2) and LDA (Lag2) achieved the best holdout accuracy at 62.5%, with stronger identification of “Up” weeks than “Down” weeks.
* Increasing complexity on Weekly did not improve results. QDA and Naive Bayes performed slightly worse than linear classifiers, while KNN (k = 1) performed near chance, indicating limited benefit from nonlinear flexibility.
* For the Kaggle obesity-risk task, four complementary frameworks were implemented: regularized multinomial logistic regression, LDA, Naive Bayes, and an RBF SVM. Results emphasized disciplined preprocessing, model comparison, and the balance between interpretability and flexibility for multi-class classification.

```
DDS-8555-ChandlerJ-Classification-Analysis/
│
├── README.md
├── ChandlerJ_DDS-8555-Assignment5.Rmd
├── ChandlerJ_DDS-8555-Assignment5.docx
├── notebooks/
│   └── ChandlerJ_DDS-8555-Assignment5.ipynb
├── submissions/
│   ├── kaggle_submission_Chandler_logit_regularized.csv
│   ├── kaggle_submission_Chandler_lda.csv
│   ├── kaggle_submission_Chandler_naive_bayes.csv
    └── kaggle_submission_Chandler_svm.csv
```
