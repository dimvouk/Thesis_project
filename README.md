# Thesis_project

This thesis project studies the dynamic dimensioning of operating reserves. When we talk about operating reserves, we refer to the Frequency Containment Reserves (FCR) and the Frequency Restoration Reserves (FRR), which consist of automatic Frequency Restoration Reserves (aFRR) and manual Frequency Restoration Reserves (mFRR).

The methodology that has been used broadly until recently is static, relying primarily on historical data to estimate the required reserve levels for a year ahead. This approach is based on a fixed calculation that doesn’t account for variations in the energy system over time.

However, this static method is becoming outdated. The increasing penetration of renewable energy sources like wind and solar power has introduced a higher level of uncertainty into the energy market. This uncertainty, driven by fluctuating generation from renewable sources, highlights the need for more flexible and adaptive methods in determining reserve requirements.

As a result, there is a growing emphasis on dynamic approaches, which aim to optimize the reserve levels on a more granular, daily basis. This project aims to explore the dynamic dimensioning of operating reserves and develop strategies that can respond to the challenges posed by the increased share of renewables in the energy mix.

# Linear regression model 
First attemt on identifying the requested level of reserves was to implement a simple linear regression model using OLS methodology to identify its parameters.

As it is obvious from the analysis plot, we notice that the regression line does not really model the dependence on time.
The regression line is almost flat relative to the high variation in the actual values, suggesting that the model is underfitting. 
We will need a more complex model that could capture the dynamics in our time series.

Towards this approach, we could use some other classical timeseries models such as arima or sarima that adds the seasonality support as well before moving further in ML models.

# Hidden Markov Model 

Second attempt is to use a long memory markov chain model to explore if we have a better forecast accuracy.

