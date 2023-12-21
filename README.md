## Gate-average-prediction-on-midus-data

## Classification approach

Gait_average is discretized as below average and above average.
* Class 1 indicates below-average
* Class 0 indicated above-average

XGboost was the best-performing model with 70% accuracy. You can see the model performance summary below. It's pretty good at predicting class 1 but almost dummy on class 0. I also report feature importances whenever it is possible. They are helpful in understanding which independent variables played an important role during the decision process. 

![classification_best_model](https://github.com/rizatemizel/Gate-average-prediction-on-midus-data/assets/127015640/ae4a2349-3edc-472e-8f56-d1376800ae7b)

You may also check the AUC score comparison for different models below:

![classification_summary](https://github.com/rizatemizel/Gate-average-prediction-on-midus-data/assets/127015640/1442e836-c257-4692-a1b9-d6b0b340596e)


## Regression approach

For regression, the best performing model was an ensemble model. Below, you can check the performance summary for this model. It has a 0.123 mean absolute error and 0.257 R2 score. 

I tried my best, but correlations between features and the target were quite weak. It's not great, but it still has some predictive power.

![regression_bestmodel_ensemble](https://github.com/rizatemizel/Gate-average-prediction-on-midus-data/assets/127015640/470fd7ec-c4a7-4800-85c0-de0608a597c5)

I also report feature importance for best performing base model (XGboost).

![best_model_feature_importance](https://github.com/rizatemizel/Gate-average-prediction-on-midus-data/assets/127015640/7a55b6ef-3d24-4d45-a666-8b367d9f5aa2)


GitHub has a known problem when rendering jupyter notebooks; this makes some output cells in notebooks quite ugly.

You can find  notebooks with better quality on the following links:

classification: https://nbviewer.org/github/rizatemizel/Gate-average-prediction-on-midus-data/blob/main/classification%20approach%28below%20average-%20above%20average%29.ipynb


regression: https://nbviewer.org/github/rizatemizel/Gate-average-prediction-on-midus-data/blob/main/regression%20approach%20-%20mae.ipynb

You can check notebooks for data cleaning, preprocessing, outlier handling, and modeling details. 

I added as much visualization as possible to make it easy to follow. 

