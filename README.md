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

* The first t-test determines if the PSI across all manufacturing lots is statistically different from the population mean of 1500 PSI. The p-value is above the common 0.05 percent. Therefore, we do not have sufficient evidence to reject the null hypothesis, and the two means are statistically similar.

* 

* 

* 


## 

Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.
