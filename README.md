![gallery](https://user-images.githubusercontent.com/98708792/233799969-6ab045cb-b142-491c-b889-cffd29f1e98e.jpg)

# Car-predicion-model
### Problem Statement
A Chinese automobile company Geely Auto aspires to enter the US market by setting up their manufacturing unit there and producing cars locally to give competition to their US and European counterparts.

They have contracted an automobile consulting company to understand the factors on which the pricing of cars depends. Specifically, they want to understand the factors affecting the pricing of cars in the American market, since those may be very different from the Chinese market. The company wants to know:

- Which variables are significant in predicting the price of a car
- How well those variables describe the price of a car

Based on various market surveys, the consulting firm has gathered a large dataset of different types of cars across the Americal market.

### Business Goal
You are required to model the price of cars with the available independent variables. It will be used by the management to understand how exactly the prices vary with the independent variables. They can accordingly manipulate the design of the cars, the business strategy etc. to meet certain price levels. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

### Results 

![image](https://user-images.githubusercontent.com/98708792/233800087-6eba9a53-a658-4396-8cb4-d257ef746d6d.png)
#### Inference :

1. `Toyota` seemed to be favored car company.
2. Number of `gas` fueled cars are more than `diesel`.
3. `sedan` is the top car type prefered.

![image](https://user-images.githubusercontent.com/98708792/233800152-6b93fccc-d2fe-4ee1-8700-1bb7a6902189.png)
#### Inference :

1. It seems that the symboling with `0` and `1` values have high number of rows (i.e. They are most sold.)
2. The cars with `-1` symboling seems to be high priced (as it makes sense too, insurance risk rating -1 is quite good). But it seems that symboling with 3. value has the price range similar to `-2` value. There is a dip in price at symboling `1`.

![image](https://user-images.githubusercontent.com/98708792/233800187-c3bf49a5-8ba1-4c4a-96a1-91c8405a8a49.png) <br>
![image](https://user-images.githubusercontent.com/98708792/233800196-52af1b59-4023-4f97-b200-88474599348a.png)
#### Inference :

1. `ohc` Engine type seems to be most favored type.
2. `ohcv` has the highest price range (While `dohcv` has only one row), `ohc` and `ohcf` have the low price range.

![image](https://user-images.githubusercontent.com/98708792/233800234-b0e00905-b1eb-4503-9bc3-221b4fa3a518.png)<br>
![image](https://user-images.githubusercontent.com/98708792/233800244-15a920bb-0a0d-4073-9ec3-76bc4493be41.png)<br>
![image](https://user-images.githubusercontent.com/98708792/233800251-3f501d62-9a96-4fd0-9a7e-a188464e505a.png)<br>

#### Inference :

1. `Jaguar` and `Buick` seem to have highest average price.
2. `diesel` has higher average price than  gas.
3. `hardtop` and `convertible` have higher average price.

![image](https://user-images.githubusercontent.com/98708792/233800300-4dae812f-e247-47a6-85f8-014281e473c2.png)<br>
![image](https://user-images.githubusercontent.com/98708792/233800308-5be2275e-975c-4334-9436-b41cda521b12.png)

#### Inference :

1. `doornumber` variable is not affacting the price much. There is no sugnificant difference between the categories in it.
2. It seems aspiration with `turbo` have higher price range than the `std`(though it has some high values outside the whiskers.)
<br>
![image](https://user-images.githubusercontent.com/98708792/233800354-072904b3-75a8-4644-8c34-6f3a71c96e39.png)<br>
#### Inference :

1. Very few datapoints for `enginelocation` categories to make an inference.
2. Most common number of cylinders are `four`, `six` and `five`. Though `eight` cylinders have the highest price range.
3. `mpfi` and `2bbl` are most common type of fuel systems. `mpfi` and `idi` having the highest price range. But there are few data for other categories to derive any meaningful inference
4. A very significant difference in drivewheel category. Most high ranged cars seeme to prefer `rwd` drivewheel.
<br>
![image](https://user-images.githubusercontent.com/98708792/233800392-ee7ddc04-3bae-43e8-aaa4-5033691fb3df.png)<br>
#### Inference :

1. `carwidth`, `carlength` and `curbweight` seems to have a poitive correlation with `price`. 
2. `carheight` doesn't show any significant trend with price.

# Model Conclusion 
#### Inference :

1. *R-sqaured and Adjusted R-squared (extent of fit)* - 0.899 and 0.896 - `90%` variance explained.
2. *F-stats and Prob(F-stats) (overall model fit)* - 308.0 and 1.04e-67(approx. 0.0) - Model fir is significant and explained `90%` variance is just not by chance.
3. *p-values* - p-values for all the coefficients seem to be less than the significance level of 0.05. - meaning that all the predictors are statistically significant.



