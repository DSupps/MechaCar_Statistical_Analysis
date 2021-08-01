# MechaCar_Statistical_Analysis

## Challenge Overview:
*AutoRU's newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing teams progress.

### Deliverables:
- Deliverable 1: Linear Regression to Predict MPG
- Deliverable 2: Summary Statistics on Suspension Coils
- Deliverable 3: T-Test on Suspension Coils
- Deliverable 4: Design a Study Comparing the MechaCar to the Competition


### Resources:
- Data Sources:
    - MechaCar MPG dataset
    - Suspension Coil dataset
    
- Software:
    - RStudio:

## Challenge Results:

## Linear Regression to Predict MPG

![deliverable1](https://user-images.githubusercontent.com/36451701/127780272-d3452b39-8b03-494b-b6da-593b47c1b247.png)

- According the summary results, vehicle length, ground clearence, and interecept are statistically unlikely to provide randomn results of variance to the linear model. In other words, vehicle length and ground clearence have a significant impact on mpg.
- The  p-value is much smaller then the significance level of 0.05. There is sufficient evidence that the slope of the linear model is not 0.
- With an R-squared of 0.71 there is a moderate to strong chance that this linear model is effective at predicting mpg. There is a 71% chance that the variability of mpg is explained using this linear model. 

## Summary Statistics on Suspension Coils

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.
![deliverable2_totalsummary_a](https://user-images.githubusercontent.com/36451701/127780570-daa54624-99e3-4cbf-8ec3-8b25e481805f.png)
![deliverable2_lotsummary_a](https://user-images.githubusercontent.com/36451701/127780578-5413115e-36bf-4f4f-bb38-eebb7c565b92.png)


- The current manufacturing data meets the design specification of not exceeding 100 psi for Lot 1 and Lot 2.
- Lot3 does not meet the design specification with a variance of 170 psi which exceeds the 100 threshold for this excercise.
- The reason for the high variance in Lot3 is due to outliers (see plot below).

![outliers](https://user-images.githubusercontent.com/36451701/127780533-caed2e0f-4d56-4dc3-bba2-c5d95f778c8d.png)




## T-Test on Suspension Coils

Deliverable 3 sample image
- Assuming our significance level is 0.05, our p-value is above our significance level.  Therefore, we do not have enough sufficient evidence to reject the null hypothesis and state that the two means are statistically similar. 

### Lot1

deliverable 3 lot1 sample image
- The p-value for Lot1 is smaller than the 0.05 significance level.  Therefore, there is enough evidence to reject the null hypothesis and conclude there is a difference in Lot1 mean compared to the population mean. 

### Lot2

deliverable 3 lot2 sample images
- The p-value for Lot2 is smaller than the 0.05 significance level.  Therefore, there is enough evidence to reject the null hypothesis and conclude there is a difference in Lot1 mean compared to the population mean. 

### Lot3

deliverable 3 lot3 sample image
- The p-value for Lot3 is larger than the 0.05 significance level.  Therefore, Lot3 is statistically similar to the population mean.


## Study Design: MechaCar vs Competition

The transport sector is one of the largest sources of CO2 emissions and a major source of air pollution.

Is the MechCar prototype better for our enviornment than it's competitors?

To test for MechaCar and it's competitors impact on the enviorment, we will perform a statistical analysis based on the following metrics:
     - CO2 Emissions
     - MPG
     
Null Hypothesis: There is no difference in CO2 emissions between MechaCar and its competitors.

Alternate Hypothesis: There is a difference in CO2 emissions between MechCar and its competitors. 

Statisitcal Test: T-Tests on CO2 Emissions

Data needed: CO2 emissions for MechCar and their competitors in a dataframe
