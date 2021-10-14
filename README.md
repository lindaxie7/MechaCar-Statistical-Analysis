# MechaCar_Statistical_Analysis
AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. We are going to review the production data for insights that may help the manufacturing team.

## The data we are working with:
MechaCar_mpg:
![Capture1](https://user-images.githubusercontent.com/38533045/137316096-888fb2e8-4823-4dcf-99b9-20a7bfaca4f2.JPG)

Suspension_Coil:



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
what metrics would be of interest to a consumer: for a few examples, cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating.
In your description, address the following questions:
What metric or metrics are you going to test?
What is the null hypothesis or alternative hypothesis?
What statistical test would you use to test the hypothesis? And why?
What data is needed to run the statistical test?
