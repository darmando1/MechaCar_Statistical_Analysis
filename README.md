# MechaCar_Statistical_Analysis

## Project Overview
Staff has been approached to help maximize efficiency for AutosRUs' newest prototype the "MechaCar." Utilizing R Studio and statistical knowledge staff will look to review the production data to help the manufacturing team.

## Deliverable 1: Linear Regression to Predict MPG
Staff has been tasked with answering the below three questions:
  1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
  2. Is the slope of the linear model considered to be zero? Why or why not?
  3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

![LM Summary](https://github.com/darmando1/MechaCar_Statistical_Analysis/blob/main/Supporting%20Images/Linear_Regression_Summary.JPG)

Utilizing the linear regression summary pictured above and the resources from Lesson 15.7.2 the staff concludes the following:
  1. Based on the Pr(>|t|) values, "each Pr(>|t|) value represents the probability that each coefficient contributes a random amount of variance to the linear model." Based on the above summary, vehicle_length and ground_clearance are statistically unlikely to provide random amounts of variance to the linear model. In other words the vehicle length and ground clearance have a significant impact on the model.
  2. The p-Value for the model is 5.35e-11. This is enough to indicate that the slope of this linear model is NOT zero.
  3. The linear model has an r-squared value of 0.7149. "To quantify how well our linear model can be used to predict future observations, our linear regression functions will calculate an r-squared value. The r-squared (r2) value is also known as the coefficient of determination and represents how well the regression model approximates real-world data points. In most cases, the r-squared value will range between 0 and 1 and can be used as a probability metric to determine the likelihood that future data points will fit the linear model." In this case apprxoimately 71% of all mpg predictions will be determined by this model.

## Deliverable 2: Summary Statistics on Suspension Coils
The MechaCar Suspension_Coil.csv contains results form multiple production lots. Weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. Staff has been tasked with answering the following:

  1. The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

![Total Summary](https://github.com/darmando1/MechaCar_Statistical_Analysis/blob/main/Supporting%20Images/total_summary_deliv2.JPG)
![Lot Summary](https://github.com/darmando1/MechaCar_Statistical_Analysis/blob/main/Supporting%20Images/lot_summary_deliv2.JPG)
Utilizing the total_summary and lot_summary pictured above staff notes the following:
  1. The overall variance is 62.3 and thus satisfies the suspension coils not exceeding 100 pounds per square inch.
  2. Lots 1 and 2 are within the range however Lot 3 has a variance of 170 which significantly impacts the total_summary.

## Deliverable 3: T-Tests on Suspension Coils
Staff has been tasked with running a t-test that compares all manufacturing lots against mean PSI of the population. Likewise, staff has been tasked with comparing each manufacturing lot against mean PSI of the population to determine if the PSI for each manufacturing lot is statistically different from the population mean of 1,500 pounds per square inch.

Staff provides the following screenshots:
  1. ![t-test](https://github.com/darmando1/MechaCar_Statistical_Analysis/blob/main/Supporting%20Images/t_test_deliv3.JPG)
  2. ![Lot 1](https://github.com/darmando1/MechaCar_Statistical_Analysis/blob/main/Supporting%20Images/lot1_ttest_deliv3.JPG)
  3. ![Lot 2](https://github.com/darmando1/MechaCar_Statistical_Analysis/blob/main/Supporting%20Images/lot2_ttest_deliv3.JPG)
  4. ![Lot 3](https://github.com/darmando1/MechaCar_Statistical_Analysis/blob/main/Supporting%20Images/lot3_ttest_deliv3.JPG)

Staff notes the following:
  1. Based on image 1, the true mean across all lots are 1498.78 with a p-=Value of 0.06. Thus, the mean of all three of these manufacturing lots is statistically similar to the population mean of 1,500.
  2. The mean of Lot 1 is 1500 with a p-value of 1.
  3. The mean of Lot 2 is 1500.2 with a p-value of 0.6072.
  4. The mean of Lot 3 is 1496.14 with a p-value of 0.04168. Lot 3 is statistically different from the population mean of 1500 (which also shows above in deliverable 2).

## Deliverable 4: Study Design: The MechaCar vs Competition
The staff has been tasked with other metrics to determine the value of the MechaCar vs Competition. Some items could include...
  1. Horse Power
  2. Luxurious Design
  3. Manufacturing Costs vs Retail Pricing
  4. Fuel Efficiency
  5. Electric or Hybrid Capabilities
  6. AWD
  7. Safety Features
  8. Maintenance Costs

Some questions posed:
  1. What metric or metrics are you going to test?
  2. What is the null hypothesis or alternative hypothesis?
  3. What stistical test would you use to test the hypothesis and why?
  4. What data is needed to run the statistical tests?

An example would be whether or not providing an electric All-Wheel-Drive vehicle would be better than a vehicle that utilizes gas with similar specifications. The metrics tested would be vehicle weight as AWD vehicles weigh more, the costs of a fully electric vehicle vs the cost of a gasoline powered vehicle, the expected horse power/power of the vehicles, and the range of the vehicles. The statistical tests utilized would be linear models and t-tests.
