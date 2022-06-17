# MechaCar_Statistical_Analysis
Module #15


## Project Overview
AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

## Resources
- Data Source: MechaCar_mpg.csv, Suspension_Coil.csv
- Software: R version 4.2.0, RStudio version 2022.02.3+492

## Deliverable 1: Linear Regression to Predict MPG
Design a linear model that predicts the mpg of MechaCar prototypes using several variables (such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance) from the MechaCar_mpg.csv file.

### Figure 1: Linear Regression Results
![Deliveralbe 1](https://github.com/Jarney903/MechaCar_Statistical_Analysis/blob/main/analysis/Figure_1.jpg)
<br />

### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
- Vehical Length and Ground Clearance 
### Is the slope of the linear model considered to be zero? Why or why not?
- The P-Value are sufficient enough evidence to evidence to reject our null hypothesis, which means that the slope of our linear model is not zero.
#### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
- Not effectively, the r-squared value is 0.71, this is only 70% accurate, most likely due to overfitting of variables. 

## Deliverable 2: Summary Statistics on Suspension Coils,
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually?

### Figure 2: PSI Analysis for All Lots
![All Lots](https://github.com/Jarney903/MechaCar_Statistical_Analysis/blob/main/analysis/Figure_2.jpg)
<br />
- Current manufacturing data does meet the design specification for all manufacturing lots in total.

### Figure 3: PSI Analysis for Individual Lots
![All Lots](https://github.com/Jarney903/MechaCar_Statistical_Analysis/blob/main/analysis/Figure_3.jpg)
<br />
- Current manufacturing data does not meet the design specification for all manufacturing lots individually, Lot 3's variance is greater than 100 PSI.

## Deliverable 3: T-Tests on Suspension Coils
Using your knowledge of R, perform t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

### Figure 4: T-Test PSI Analysis for All Lots
![All Lots](https://github.com/Jarney903/MechaCar_Statistical_Analysis/blob/main/analysis/Figure_4.jpg)
<br />
- The mean is not equal to 1500, the P-Value is 6%, greater than the 5% significance level.

### Figure 5: T-Test PSI Analysis for Individual Lots
![All Lots](https://github.com/Jarney903/MechaCar_Statistical_Analysis/blob/main/analysis/Figure_5.jpg)
<br />
- Lot 1: The mean is equal to 1500, the P-Value is 100%
- Lot 2: The mean is very close to 1500, the P-Value is 6%, greater than the 5% significance level
- Lot 3: The mean is not equal to 1500, the P-Value is 4%, fewer than the 5% significance level


## Deliverable 4: Study Design: MechaCar vs Competition
Create a statistical analysis for MEchaCar vs Competition. Gather the following data points for the following (cost, city or highway fuel efficiency, horse power) and determine how MEchaCar performs based on Cost vs Fuel Efficiency, Cost vs Horse Power, and Fuel Efficiency vs Horse Power. 

## Address the following questions:
What metric or metrics are you going to test?
- Determine how MEchaCar performs based on Cost vs Fuel Efficiency, Cost vs Horse Power, and Fuel Efficiency vs Horse Power.

What is the null hypothesis or alternative hypothesis?
- Null hypothesis is there are no coorelations, alternative hypothesis is there are coorelations for the 3 metrics above. 

What statistical test would you use to test the hypothesis? And why?
- I would use the Summary Statitics to create a DataFrame based on the metrics and car manufacturor for vehical class, then you t-test to determine if the coorelations can be trusted. 

What data is needed to run the statistical test? 
- Gather the following data points for the following (cost, city or highway fuel efficiency, horse power).



