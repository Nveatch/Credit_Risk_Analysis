# Credit_Risk_Analysis

## Overview of Project

### Purpose
The purpose of this analysis was to use Jupyter Notebook to assess the accuracy of several different machine learning algorithms in determining credit card risk.

## Results
The following table is an aggregation of all the results from the Jupyter Notebook file:

![ML Table](https://github.com/Nveatch/Credit_Risk_Analysis/blob/main/Resources/ml_table.png))

- RandomOverSampler had a balanced accuracy score of 0.639(4th best), high risk precision and recall scores of 0.01(3rd best(worst)) and 0.59(6th best(worst)), and low risk precision and recall scores of 1.00(best) and 0.69(4th best)

- SMOTE had a balanced accuracy score of 0.648(3rd best), high risk precision and recall scores of 0.01(3rd best(worst)) and 0.60(5th best), and low risk precision and recall scores of 1.00(best) and 0.70(3rd best)

- ClusterCentroids had a balanced accuracy score of 0.531(6th best(worst)), high risk precision and recall scores of 0.01(3rd best(worst)) and 0.61(4th best), and low risk precision and recall scores of 1.00(best) and 0.45(6th best(worst))

- SMOTEENN had a balanced accuracy score of 0.633(5th best), high risk precision and recall scores of 0.01(3rd best(worst)) and 0.69(2nd best), and low risk precision and recall scores of 1.00(best) and 0.58(5th best)

- Balanced Random Forest had a balanced accuracy score of 0.765(2nd best), high risk precision and recall scores of 0.03(2nd best) and 0.65(3rd best), and low risk precision and recall scores of 1.00(best) and 0.88(2nd best)

- EasyEnsemble had a balanced accuracy score of 0.871(best), high risk precision and recall scores of 0.08(best) and 0.80(best), and low risk precision and recall scores of 1.00(best) and 0.94(best)

## Summary

### Result Summary
For this dataset, the ensemble models performed the best, with EasyEnsemble performing the best overall, having f1-scores of 0.14 and 0.97 for high and low risk respectively. ClusterCentroids performed the worst overall, scoring the worst in every category except high risk recall, where it was still bad with the 4th best of all the models. This is further proven by it's f1-scores, 0.01 and 0.62 for high and low risk respectively (the worst of all the models).
### ML Model Recommendation
From this analysis, the results would indicate that the best model is EasyEnsemble, and thus would receive my recommendation. However, just because that model performed the best on this dataset does not mean it would perform the best on other datasets. Usually different models excel at different things, so while EasyEnsemble was the best across the board in this instance, I would consider than an exception rather than the norm. That being said, while I don't feel comfortable that model in all instances, I can give a broader recommendation of ensemble models as a whole, as both the ones I tested here were significantly better than the other four non-ensemble models. This is especially of note as they use the same sampling type of ClusterCentroids (undersampling) which scored the worst overall, and yet were the top models. 