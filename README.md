# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
![image](https://github.com/maryamt95/MechaCar_Statistical_Analysis/blob/main/resources/deliver%201%20pic.JPG)



mpg = (6.267)vehicle_length + (0.0012)vehicle_weight + (0.0688)spoiler_angle + (3.546)ground_clearance + (-3.411)AWD + (-104.0)

From the above output we can see that:

1. The vehicle length, and vehicle ground clearance are statistically likely to provide non-random amounts of variance to the model. That is to say, the vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype. Conversely, the vehicle weight, spoiler angle, and All Wheel Drive (AWD) have p-Values that indicate a random amount of variance with the dataset.

2. The p-Value for this model, p-Value: 5.35e-11, is much smaller than the assumed significance level of 0.05%. This indicates there is sufficient evidence to reject our null hypothesis, which further indcates that the slope of this linear model is not zero.

3. This linear model has an r-squared value of 0.7149, which means that approximately 71% of all mpg predictions will be determined by this model. Relatively speaking, this multiple regression model does predict mpg of MechaCar prototypes effectively.


## Summary Statistics on Suspension

Total summary :

![image](https://github.com/maryamt95/MechaCar_Statistical_Analysis/blob/main/resources/total_summary.JPG)

Lot summary :


![image](https://github.com/maryamt95/MechaCar_Statistical_Analysis/blob/main/resources/lot_summery.JPG)

When looking at the entire population of the production lot, the variance of the coils is 62.29 PSI, which is within the 100 PSI variance requirement.

Similarly, Lot 1 and Lot 2 are well within the 100 PSI variance requirement; with variances of 0.98 and 7.47 respectively. However, Lot 3 shows much larger variance in performance and consistency, with a variance of 170.29. It is Lot 3 that is disproportionately causing the variance at the full lot level.


## T-Tests on Suspension Coils

Conducting t-test on the suspension coil data to determine whether there is a statistical difference between the mean of this provided sample dataset and a hypothesized, potential population dataset. Using the presumed population mean of 1500, we find the following:

There is a summary of the t-test results across all manufacturing lots:

![image]( https://github.com/maryamt95/MechaCar_Statistical_Analysis/blob/main/resources/one%20sample%20test.JPG)

True sample mean is 1498.78 , with a P-value of 0.06028. which is higher than teh common signifcance level of 0.05.
Hnce , there is not enough evidence to supprt rejecting the null hypothesis .the mean of all three lots is statistically similar o the presumed populaion mean of 1500.

Looking at the individual lots :

1. Lot 1 sample actually has the true sample mean of 1500. With a p-Value of 1, clearly we cannot reject (i.e. accept) the null hypothesis that there is no statistical difference between the observed sample mean and the presumed population mean (1500).
2. Lot 2 has essentially the same outcome with a sample mean of 1500.02, a p-Value of 0.61; the null hypothesis cannot be rejected, and the sample mean and the population mean of 1500 are statistically similar.
3. However, Lot 3 is a different scenario. Here the sample mean is 1496.14 and the p-Value is 0.04, which is lower than the common significance level of 0.05. All indicating to reject the null hypothesis that this sample mean and the presumed population mean are not statistically different.


![image](https://github.com/maryamt95/MechaCar_Statistical_Analysis/blob/main/resources/lots%20sampe%20test.JPG)


## Study Design: MechaCar vs Competition

There are many factors that consumers take into consideration when evaluating a car to purchase. Customers looking to purchase a car are looking for more than just a conveyance. They will be looking to buy a car that is an economical means to regularly transport themselves and their items on a reliable, regular basis.


### Metric to test

Safety Feature Rating ,Current Price (Selling),Engine (Electric, Hybrid, Gasoline / Conventional),Resale Value,Average Annual Cost of ownership (Maintenance),MPG (Gasoline Efficiency)

### Hypothesis: Null and Alternative

Null Hypothesis (Ho): MechaCar is priced correctly based on its performance of key factors for its genre.
Alternative Hypothesis (Ha): MechaCar is NOT priced correctly based on performance of key factors for its genre.

### Statistical Tests
A multiple linear regression would be used to determine the factors that have the highest correlation/predictability with the list selling price ,which combination has the greatest impact on price (it may be all of them!)

