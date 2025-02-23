# Machine-Learning-Module-Project
Module End Project of MAchine learning in association with Entri Elevate


Analyzing the Results

One needs to examine the df_results DataFrame and look for the model with the highest R-squared value, the lowest MSE, and the lowest MAE.

Example:

My analysis resulted in the following df_results DataFrame:

				MSE	R-squared	MAE
Linear Regression		0.258532	0.792011	0.346027
Decision Tree			0.244733	0.803112	0.334895
Random Forest			0.244733	0.803112	0.334895
Gradient Boosting		0.244733	0.803112	0.334895
Support Vector Regression	0.244733	0.803112	0.334895


Identifying the Best Model

In this example, Gradient Boosting would be the best-performing model because:

Highest R-squared: It has the highest R-squared value (0.80), indicating that it explains the most variance in the target variable.
Lowest MSE and MAE: It has the lowest MSE (0.24) and MAE (0.33), suggesting that its predictions are, on average, closer to the actual values compared to other models.
Although the other models have similar MSE,R-squared and MAE values, Gradient Boosting has the upper hand in that, it often performs better because it combines multiple weak learners (decision trees) to create a strong predictive model. It iteratively learns from the mistakes of previous trees, leading to improved accuracy.
So based on the analysis, Gradient Boosting would be the best-performing model due to its high R-squared value and low error metrics.

Based on my analysis, the top three most important features are: Engine location(Americans prefer rear-engine vehicles), Engine type(rotor type is preferred) and Engine type (dohcv type engines are preferred).

Hyperparamter tuning was performed. Theoretically, if the tuned model has a lower MSE and a higher R-squared than the original model, then hyperparameter tuning has successfully improved its performance. This is absolutely true in case of the Dataset under consideration. Hence it maybe concluded that performance of the model has been increased.

Understanding the features:

Engine location: This is a binary feature (0 or 1) indicating whether the engine is located in the rear of the car. Most cars have engines in the front, so this feature likely highlights a specific and less common configuration. Hence pricing of rear engine cars have a lot of importance when trying to break into the American Market.

Engine type: This binary feature indicates whether the car has a rotary engine (Wankel engine). Rotary engines are relatively rare and known for their unique characteristics and it is an important feature for the American buyers and hence pricing of these Vehicles will have to on thelower end to capture the interest of the new Market.

Engine type: This binary feature indicates whether the car has a DOHCV (Dual Overhead Camshaft per cylinder head, with Variable Valve Timing) engine. DOHCV engines are often associated with performance-oriented vehicles. When it comes to pricing it helps to keep this on the lower end of the spectrum.

Since these features are of high positive importance, it would mean that, they increase the price of the Cars. Providing competitive prices (in effect lower prices) in these categories will determine what percentage of the market share the Chinese Automotive Manufacturer will be able to capture in the American market.
