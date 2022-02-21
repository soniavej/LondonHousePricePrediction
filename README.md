# LondonHousePricePrediction

Objective:

1.The goal of the project is to understand the factors affecting the price of London housing market.
 
2.To create a best fit model using Linear Regression, to predict the average price  of London properties that fall within a user-defined search radius, which can be fine-tuned   by options such as property type and other attributes.

3.Residual Analysis

Background:

Independent Variables/Regressors
1. House Type - House, Flat/Apartment, New Development, Duplex, Penthouse, Studio,   Bungalow, Mews
2. Area in sq ft
3. No. of Bedrooms (0 to 10)
4. No. of Bathrooms(0 to 10)
5. No. of Receptions (0 to 10)
6. Location (574)   
7. Postcode

Dependent/Target Variable
1.Price (in thousand Pounds)

Region:

<img src="https://user-images.githubusercontent.com/99994988/155001053-d148f27f-be29-4c0e-953f-5b2232e17f94.png" width="500" height="400" align="centre">

After Doing Anova test for all the 8 regions, we can statistically say that there is a difference of means in Regions. Therefore, Region do influence the Price .

Type:

<img src="https://user-images.githubusercontent.com/99994988/155001607-62166900-2885-4d1f-8157-326c41a6b9de.png" width="500" height="400" align="centre">

After Doing Anova test for all the 8 types of property, we can statistically say that there is a difference of means in types. Therefore, Type of the property do influence the Price .

Area:

<img src="https://user-images.githubusercontent.com/99994988/155001759-e0439fa9-0b8e-4366-abe8-a6b737aae605.png" width="500" height="400" align="centre">

This shows as the Area increases the Price also increases. 

Correlation Matrix:

<img src="https://user-images.githubusercontent.com/99994988/155002157-cb4547db-5378-41cd-86f6-2df9e78467a2.png" width="500" height="400" align="centre">


Linear Regression Model:

Model 1: Linear Regression with all the variables
  R squared is 54.38%, but vif is too high

Model 2: Linear Regression without Nrec, Nbath
  R squared is 54.38%, but vif is too high
  
Model 3: Linear Regression with Nbed, area, and region 
  R Squared is 53.02%
  
Model 4: Linear Regression with Area and Nbed
  R Squared is 50.87%
  
  
Conclusion:

Model 1 and Model 2 are rejected due to high VIF. Model 4 reduced the R-Squared and RMSE increased. Therefore, we accept Model 3 as the best fit linear regression Model. 53.02% of the variation in price is explained by this model.![image](https://user-images.githubusercontent.com/99994988/155002782-f0bbc40a-dd46-4ebb-989b-fbc29f13cfa6.png)

Residuals:

This Linear Regression Model is close to the best fit but there is a scope of improvement because of the following reasons:

1)It fails the test of homoscedasticity. This regression model's ability to predict price of the property is not consistent across all values . 

2)The residuals are not normally distributed. It shows some unexplored patterns which are not explained by this model.




