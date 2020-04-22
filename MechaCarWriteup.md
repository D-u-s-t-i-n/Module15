# MPG Regression

## Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

Based off the summary table of our model, the predictors vehicle.length and ground.clearance provide a non-random amount of varaince to the mpg values in the data set. The other predictors - vehicle.weight, spoiler.angle, and AWD have a p-value > .05 so they are not significant and unlikely to provide a non-random amount of variance to mpg in the data set.

## Is the slope of the linear model considered to be zero? Why or why not?

The slope is not zero because we have predictors that are significant (p-value < .05) and have a non-zero value for the estimates of their coefficient.

## Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

The linear model should make effective predictions for mpg since the adjusted R-squared value is relatively high. 68.25 percent of the variation in the data can be explained by the model we fitted. 

# Suspension Coil Summary

The variance of the PSI of the suspension coil summary is 62.29356 which is less than the 100 limit, but that's the value if we combine all the manufacturing lots together. We have three lots with 50 vehicles in each lot and for the first two lots the variance is 0.9795918 for Lot 1 and 5.469388 for Lot 2.

However for Lot3 the variance is 170.2861 which is greater than 100. There is either a problem in recording PSI readings in Lot1 and Lot2 or there's a problem in recording PSI readings in Lot3. Othwerwise Lot3 vehicles have issues. More investigation will need to be done to reconcile why the values are so different.

If we were to trust the data as is, then Lots1 and Lots2 beat the standard. However Lot3 fails.

# Suspension Coil T-Test

The p-value for our t-test is .06028. Which means we fail to reject our null hypothesis. What was our null hypothesis?

Null hypothesis: mean = 1500
Alternate hypothesis: mean does not equal 1500.

Since our p-value is greater than .05, which is the most common signficance level, we lack the evidence to say the
mean of our data is sigificantly different from 1500. Note: that the absence of proof is not the proof of the absence.

# Design Your Own Study

Cost of the vehicle and fuel efficiency are often big considerations for wanting to buy a vehicle. I am assuming most
buyers would be interested in the performance and cost of their vehicle before they consider aesthetics such as its
color or spoilers/fins.

I would get more research data on cheaper materials, which generally increases the car weight. This will also affect the mpg. The challenge would be to maintain mpg at lower cost. A research question I would propose how much flexible room do we have with material quality used to manufacture the vehicle in relation to fuel efficiency (mpg). 

Our null hypothesis: Cost of material, cheap vs. expensive, *has no* effect on fuel economy.
Our alternatve hypothesis: Cost of material, cheap vs. expensive, *has* an effect on fuel economy.

I would compare the means between cars made with cheap materials versus expensive materials. To do this, best kind of statistical test would be the t-test. The means of fuel efficiency (mpg) would also be needed.