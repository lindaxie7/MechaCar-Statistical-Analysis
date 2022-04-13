 [R Code](https://github.com/lindaxie7/MechaCar_Statistical_Analysis/blob/main/MechaCarChallenge.Rmd) 
# MechaCar_Statistical_Analysis
AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. We are going to review the production data for insights that may help the manufacturing team.

## The data we are working with:
MechaCar_mpg:
![Capture1](https://user-images.githubusercontent.com/38533045/137316096-888fb2e8-4823-4dcf-99b9-20a7bfaca4f2.JPG)

Suspension_Coil:
![Capture2](https://user-images.githubusercontent.com/38533045/137316403-2e926067-b66f-428d-9319-1f0d88009458.JPG)


## Linear Regression to Predict MPG
- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

Vehicle weight, spoiler_angle & AWD provided a non-random amount of variance. The two variables that had the most amount of random variance are ground_clearance and vehicle_length

- Is the slope of the linear model considered to be zero? Why or why not?

No, the slope of the linear model is not considered to be zero, because the p value is 5.35e-11, it is very small, there is a significant linear relationship between the independent variables and the dependent variable 

- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

Yes, based on the summary(Mutiple R Square = 0.7149, big enough) and the plot, we can conclude that there is a significant, linear relationship between the independent variables and the dependent variable, it is predict effectively. 
![1](https://user-images.githubusercontent.com/38533045/136679215-18ff4a17-9b35-49a5-87b3-64bea3c00839.png)

![3](https://user-images.githubusercontent.com/38533045/136679249-f5ba4c59-c4c4-488f-bb00-ff7432dc3f15.png), 

![2](https://user-images.githubusercontent.com/38533045/136679257-adf973f9-19c8-4604-9d2d-82a7e272d22a.png)

## Summary Statistics on Suspension Coils
- The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

No, the current manufacturing data does not meet the specification that the suspension coils must not exceed 100 pounds per square inch, in the total_summary, we can see that the variance is 62.29356, which is less than 100 pounds per square inch. 
![Capture1](https://user-images.githubusercontent.com/38533045/137307289-8004a23b-ae64-4e29-9cf3-155a568f4c4f.JPG)


No, not all individually manufacturing lots meet this design specification, in the lot_summary, we can see that the variance for lot1 is 0.9795918, the variance for lot2 is 7.4693878, the variance for lot3 is 170.2861224, so only lot3 meets the specification that the suspension coils must not exceed 100 pounds per square inch.
![Capture2](https://user-images.githubusercontent.com/38533045/137307450-d1adffa8-e83b-4c53-8faa-e1c3ca92c183.JPG)

## T-Tests on Suspension Coils
- Determine if the PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.

p-value = 0.06028, which is greater than α 0.05, We do not have enough evidence to conclude that the true mean of all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.
![Capture1](https://user-images.githubusercontent.com/38533045/137311066-21e72ec3-40a4-478a-87f5-9ff241845c30.JPG)


- Determine if the PSI for each manufacturing lot is statistically different from the population mean of 1,500 pounds per square inch.

T-test on lot1, p-value = 1, which is greater than α 0.05, We do not have enough evidence to conclude that the true mean of all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.

T-test on lot2, p-value = 0.6072, which is greater than α 0.05, We do not have enough evidence to conclude that the true mean of all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.

T-test on lot3, p-value = 0.04168, which is less than α 0.05, We have strong evidence to conclude that the true mean of all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.
![Capture2](https://user-images.githubusercontent.com/38533045/137311213-f18ae87c-2008-4996-9f63-774a359418d0.JPG)

![Capture3](https://user-images.githubusercontent.com/38533045/137311290-8dfb977f-7316-4b04-aa5f-80ad24cad5e3.JPG)

## Study Design: MechaCar vs Competition
I have designed a statistical study in order to see how MechaCar vehicles perform against vehicles made by other maunfacturers. Potential metrics that consumers could find interesting in might include cost, city or highway fuel efficiency, horse power, maitenance cost, or safety rating.

Metric Tested:
Collecting data for comparable models across all major manufacturers for past 3 years for the following metrics to aim to analyze how competitively MechaCars are priced to their competition.
- Safety Feature Rating: Independent Variable
- Current Price (Selling): Dependent Variable
- Engine (Electric, Hybrid, Gasoline / Conventional): Independent Variable
- Average Annual Cost of ownership (Maintenance): Independent Variable
- MPG (Gasoline Efficiency): Independent Variable
 
 
Hypotheses:
- Null Hypothesis: MechaCars have no difference in pricing compared to its competitors, and have no differences in fuel efficiency or horse power in comparison to competitors.
- Alternative Hypothesis: MechaCars have different pricing in comparison to competitors and have differences in fuel efficiency and horse power compared to the competition.
Statistical Tests to be Performed

In this study we will use a two sample t-test to compare the means from the two populations. From there we will perform one-tailed t-tests in order to determine which means are greater than or less than the other.

Data Requirements:
In order to carry out this statistical test we will either need a collection of data from MechaCar and its competitors or (1) the mean of both samples, (2) the standard deviation of both samples, and (3) the number of observations.


