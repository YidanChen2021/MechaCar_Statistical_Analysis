# MechaCar_Statistical_Analysis
This project is brought out to conduct data analysis around the production datas of MechaCar to help the management of AutosRUs allocate issues and potential solve the problem for manufacturing team.

## Linear Regression to Predict MPG  
- The vehicle weight, spoiler_angle and AWD provide a random amount of variance, while the ground_clearancea and vehicle_length provide the most amount of non-random variance.   
- The slope is not zero as the p-value is less than 0.05.
- The R-squared value is 71%, which shows a pretty high rate of accuracy of the prediction. However, there might be other effectors that contributes to the mpg variability. 

## Summary Statistics on Suspension Coils  
![Total_Summary](https://user-images.githubusercontent.com/93500353/154877536-78767101-e101-426a-8ffc-1f05d6bfd45b.png)
![lot_summary](https://user-images.githubusercontent.com/93500353/154877543-66c0d51f-fee7-4f22-bbda-a80dd8b1bcf5.png)
The production overall has the variance of coils at 62.29 PSI, which is within the 100PSI variance requirment. When we look deeper into each lot, lot 1 and 2 are within the variance requirment with variances of 0.97 and 7.46. However, lot 3 has variance of 170.29, which is a lot higher beyong the variance requirment.  

## T-Tests on Suspension Coils

![T-Test Overall](https://user-images.githubusercontent.com/93500353/154878557-02f2e63f-2d56-4e2d-a1e5-eb7706bc6b61.png)
T-test result of all manufacturing lots overall

![T-test lot 1](https://user-images.githubusercontent.com/93500353/154878854-f53da1ee-71b0-4729-bcd0-e94dd4f104db.png)
T-test fot lot1  
![T-test lot 2](https://user-images.githubusercontent.com/93500353/154878885-70821d91-d166-4d8e-867d-2a40211c9f66.png)  
T-test for lot2  
![T-test lot 3](https://user-images.githubusercontent.com/93500353/154878915-291dd1b5-2c1f-49fc-b1ee-8cdf1a9dd41c.png)
T-test for lot3  
By looking at the t-test of all manufacturing lots together, the true mean of sample is 1498.78, with a p-value of 0.06. The p-value is slightly higher thant the signigicance level of 0.05, there is not evidance to support the rejecting of the null hypothesis. Therefore, the mean of all 3 lots is similar to the presumed population mean of 1500.  
When we look into the t-test result of each lot. Lot 1 and 2 are similarily indicating a similar sample mean and the population mean. As lot 1 and 2 have a sample mean of 1500 and 1500.02, which is equal or close to 1500. The p-value is at 1 and 0.61 respectively, which indicates that the null hypothesis cannot be rejected.
When it comes to lot 3, it comes with a sample mean of 1496.14 and the p-value is 0.04. Since the p-value is below 0.05, it indicates the null hypothesis rejection. The sample mean and the presumed population mean are not satisfically similar.   

## Study Design: MechaCar vs Competition  
When it comes to car purchasing, consumers will also be looking at the market price, mpg, annual maintenance cost and depreciation/resell value. After collecting datas from the above metrix from MechaCar and competitors, we can design the test by making the following hypothesis:  
- null hypothesis: MechaCar's market price is smilar to the same type of car designed by a competitor.
- Alternative hypothesis: MachCar's market price largely differentiate itself from same type of car from a competitor.  

At the end, we will perform t-test for all data and for individual companies. 
