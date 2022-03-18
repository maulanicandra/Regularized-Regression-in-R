# Regularized-Regression-in-R
Regularized Regression Ridge and Lasso in R
Files contain of:
1. Split Training and Test Dara
2. Correlation Study. The results are:
- The Feature tax and rad are positively correlated with each other (0.91)
- The feature age and dis are negatively correlated with each other (-0.75)
- Price (medv) depends upon feature RM (positively correlated 0.75) and lstat (negatively correlated -0.76)
-Since Threshold abs(corr) >=0.8, the feature tax and rad are selected to be compared with medv. Since rad -> medv < tax -> medv, rad (Index of accessibility to radial highways) will be drop
3. Model Training (Ridge Regression and Lasso Regression). The Result are:
- The best lambda of ridge regression based on validation data is 0.01. The RSME value or The standard deviation of prediction errors is 4.3464 (lowest).
- The best lambda of lasso regression based on validation data is 0.01. The RSME value or The standard deviation of prediction errors is 4.340783 (lowest).
5. Model Evaluation.
![image](https://user-images.githubusercontent.com/97785087/158914697-d968ed14-3086-4b2f-9782-7642c075c89b.png)
The intrepetation of RSME, MAE, and MAPE
RSME
- Ridge: RSME values is 6.820639 which means The standard deviation of prediction errors is 6.820639 i.e. from the regression line, the residuals mostly deviate between +- 6.820639.
- Lasso: RSME values is 6.823445 which means The standard deviation of prediction errors is 6.823445 i.e. from the regression line, the residuals mostly deviate between +- 6.823445.

MAE
- Ridge: On average, our prediction deviates the true medv by 3.898674.
- Lasso: On average, our prediction deviates the true medv by 3.888415.

MAPE
- Ridge: The 3.898674 deviation is equivalent to 17.11394% deviation relative to the true medv
- Lasso: The 3.888415 deviation is equivalent to 17.07025% deviation relative to the true medv
