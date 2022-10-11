# Purpose

This analysis uses R to review production data on the MechaCar for insights that may help the manufacturing team with production troubles.

## Linear Regression to Predict MPG

![alt text](https://github.com/ajkriegz/MechaCarChallenge/blob/main/resources/mpg_regression.png "MPG Regression Analysis")

* The variables that seem to provide a non-random amount of variance to mpg values in this dataset are vehicle length and ground clearance.

* The slope of this linear model can be considered not zero because the p-value is much smaller than assumed significance levels, showing that there is sufficient evidence to reject the null hypothesis.

* The r-squared value is over .7, meaning this model can be considered an accurate predictor of MechaCar prototypes. 

## Summary Statistics on Suspension Coils

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. 

![alt text](https://github.com/ajkriegz/MechaCarChallenge/blob/main/resources/total_summary.png "Total Summary")

![alt text](https://github.com/ajkriegz/MechaCarChallenge/blob/main/resources/lot_summary.png "Lot Summary")

Looking at the total summary, the coils do not exceed 100 pounds per square inch. However, while the overall variance falls within acceptable guidelines, the lot summary shows that Lot3 exceeds this variance threshold. Lot1 and Lot2 are acceptable.

## T-Tests on Suspension Coils

![alt text](https://github.com/ajkriegz/MechaCarChallenge/blob/main/resources/coil_t-test.png "Population t-test")

* The first t-test determines if the PSI across all manufacturing lots is statistically different from the population mean of 1500 PSI. The p-value is above the common 0.05 threshold. Therefore, we do not have sufficient evidence to reject the null hypothesis, and the two means are statistically similar.

![alt text](https://github.com/ajkriegz/MechaCarChallenge/blob/main/resources/Lot1_t-test.png "Lot 1 t-test")

* The p-value is greater than the significance level, implying that there is greater than a one-in-twenty chance that the differences in means is due to chance. We do not have sufficient evidence to reject the null hypothesis, and the two means are therefore statistically similar.

![alt text](https://github.com/ajkriegz/MechaCarChallenge/blob/main/resources/Lot2_t-test.png "Lot 2 t-test")

* The p-value for lot 2 is smaller than our significance level. There is sufficient evidence to reject the null hypothesis, and therefore the difference in means between the population and this sample is statistically significant. Lot 2 did not exceed acceptable variance levels in the previous analysis heading, but the mean PSI is not equal to 0.

![alt text](https://github.com/ajkriegz/MechaCarChallenge/blob/main/resources/Lot3_t-test.png "Lot 3 t-test")

* The p-value for lot 3 is smaller than our significance level and therefore statistically significant. Variance and mean PSI are beyond expected measures.

## Study Design: MechaCar vs Competition

With inflated costs of fuel and both new and used vehicles, city and highway fuel efficiency, as well as upfront initial cost and future maintenance costs will be on many prospective consumers' radar. The analysis team recommends a statistical study to test MechaCar on these metrics versus competitor vehicles that are on or entering the market.

The base null hypothesis to investigate then either accept or reject is that these factors (fuel efficiency, cost, maintenance spending) have no measurable impact on each other. If there is enough evidence to reject this hypothesis, an alternative hypothesis would be that these factors do have a measurable impact on each other.

The recommended analysis type is ANOVA, or Analysis of Variance, in order to determine the impact of factors on MechaCar's fuel efficiency and initial cost as compared to its competitors. ANOVA will also be helpful in determining how significant or random the results of testing will be.

It will be necessary to collect internal and competitor data on a model's cost, projected (or realized) maintenance costs, and both highway and city fuel efficiency.