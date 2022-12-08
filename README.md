# Stat 435 Project
Zach Fechko (011711215) & Anthony Ghimpu

## Dataset and Description
Use the dataset `Boston` which is located in the `MASS` library. This dataset contains 506 observations on 14 vairiables. The response is `medv` and the rest are potential predictors. Namely we are interested in predicting `medv` using a linear model. Please make sure you understand the meaning and type of each variable in the dataset.

## Tasks
1. Use `set.seed(1)` for all operation that involve user-induced randomness (such as `sample` or `cv.glmnet`). Otherwise your resultes will not be reproducable when they are checked and graded

2. randomly split using the `sample` command the observations into a training/testing set so that the training set can be used to fit a linear model, and the validation set can be used to evaluate the prediction accurarcy of the fitted model. Here you have the freedom on splitting. But please be careful with the number of observations for each set, since a training set with a few observations cannot produce a relatively good-fit model.

<div class="alert alert-block alert-warning">
<b>Caution:</b> these 2 sets should be non-intersecting; sample from the row indeces but do not sample with replacement when creating the two sets
</div>

3. Implement LASSO (with cross-validation to select the optimal tuning parameter) on all potential predictors without interactions between them, report the best model (that is based on the optimal tuning parameter) and its fitted model, conduct hypothesis tests on some coefficients of the model and report your findings, and assess the prediction accuracy of the fitted model.


5. Among the best/optimal models you would find in (2), and (3) respectively, which one has
the best prediction accuracy? If you consider a trade-off between the number of predictors in
a model and its prediction accuracy, which among the best models you found in (2), and (3)  would you prefer?

<div class="alert alert-block alert-info">
<b>Note:</b> For conducting hypothesis tests on some model coefficients for the models you found in and (3)
 you can use the R <code>library(hdi)</code>
</div>
