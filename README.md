# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
![alt text](https://raw.githubusercontent.com/samnougues/MechaCar_Statistical_Analysis/main/image/Picture1.png)
This image above is linear regression done on data from MechaCar_mpg.
![alt text](https://raw.githubusercontent.com/samnougues/MechaCar_Statistical_Analysis/main/image/Picture2.png)
This is a summary of the linear regression done earlier.
Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
-A non-random amount of vehicle_length (with a p-value of 2.6E-12) and ground_clearance (with a p-vlaue of 5.21E-8) because they have a p-value < 0.5.
Is the slope of the linear model considered to be zero? Why or why not?
-No, the slope of the line is non-zero. This is because the p-value for the summary statistics is 5.35E-11, which is less than the alpha value of 0.05, and there is non-random variance in the data.
Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
-The R-Squared value of 0.7149, which means the mpg of MechaCar prototypes can be decently predicted using this model. The Adjusted R-Squared value of 0.6825, which means that the ability to predict the mpg of MechaCar prototypes is slightly lower but still a good predicter.

## Summary Statistics on Suspension Coils
The below chart is a summary statistics for the suspension coils for all lots.
![alt text](https://raw.githubusercontent.com/samnougues/MechaCar_Statistical_Analysis/main/image/Picture7.png)
The below chart is a summary statistics for the suspension coils for each individual lot.
![alt text](https://raw.githubusercontent.com/samnougues/MechaCar_Statistical_Analysis/main/image/Picture8.png)
-The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
-- The variance for all lots is 62.29356 PSI which is below the 100 PSI limit. However when one looks at the individual lots, lot 3 is 170.28612 PSI which higher than the 100 PSI limit. Lot 1 and Lot 2 is much lower with a variance of 0.97959 PSI for Lot 1 and  a variance of 7.46938 PSI for Lot 2

## T-Tests on Suspension Coils
The image below is the t-test p-value for all of the lots. The p-value of 0.06028 which is greater than the alpha of 0.05 meaning that the manufacturing lots  not significantly different than the population.
![alt text](https://raw.githubusercontent.com/samnougues/MechaCar_Statistical_Analysis/main/image/Picture3.png)
In Lot 1, the t-test gave a p-value of 1 which mean there is no significant difference between the Lot 1 and the general populations. As seen below:
![alt text](https://raw.githubusercontent.com/samnougues/MechaCar_Statistical_Analysis/main/image/Picture4.png)
In Lot 2, the t-test gave a p-value of 0.6072, which is higher than .05 mean alpha there is no significant difference between the Lot 2 and the general populations. As seen below: ![alt text](https://raw.githubusercontent.com/samnougues/MechaCar_Statistical_Analysis/main/image/Picture5.png)
In Lot 3, the t-test gave a p-value of 0.04168, which is lower than .05 alpha mean there is a significant difference between the Lot 3 and the general populations. As seen below: ![alt text](https://raw.githubusercontent.com/samnougues/MechaCar_Statistical_Analysis/main/image/Picture6.png)

## Study Design: MechaCar vs Competition
Further studies can be performed to determine MechaCar's standing against its competition in maintenance cost.

Metrics to be tested:

Maintenance cost 1 year after the car is bought, 5 years after car is bought, and 10 years after car is bought

Vehicle Weight: Independent Variable

The age of the car would be Independent Variable

Null and Alternative Hypothesis

Null Hypothesis: Maintenance of the MechaCar is the same as other cars.

Alternative Hypothesis: Maintenance of the MechaCar is not the same as other cars.

Statistical Test to be Used

A multiple linear regression will be used given the presence of one continuous, dependent variable, and several continuous independent variables.

Data Needed:

We would need to know the maintenance cost of MechaCars through the years. We would also need to know the maintenance cost of other types of cars
