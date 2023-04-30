# Amazon_coupons


# Will a Customer Accept the Coupon?

### Context
This project aims to identify the factors that influence a driver's decision to accept a coupon sent to their phone. The dataset from a survey on Amazon Mechanical Turk includes various driving scenarios, destinations, times, weather conditions, passengers, and coupon types. Participants were asked if they would accept a coupon for different venues, and their responses were labeled 'Y = 1' or 'Y = 0' depending on whether they accepted the coupon or not.



### Data

The dataset includes user attributes like gender, age, education, and income, as well as their frequency of visiting bars, coffee houses, takeaway food, and restaurants. It also contains contextual attributes such as driving destination, weather, time, and passenger, along with the location of the user, coupon, and destination. The coupons have an expiration period of either 2 hours or one day.


### Notes


- #### All of the work done, including observations and comments, is contained within the following Jupyter Notebook, which provides a comprehensive analysis.[Jupyter notebook](https://github.com/ZERARKAH/Amazon_coupons/blob/da30e4371936c06cc978ae41f135aadb3d0f6969/prompt.ipynb)
 
- In order to facilitate the follow-up analysis, it has been determined that certain columns, specifically which are currently defined as objects, must be treated as numerical.( expiration,CarryAway, Bar, CoffeeHouse,RestaurantLessThan20, age, income,and Restaurant20to50)
 
- I did remove all the duplicates from the data, and eliminated all the NaN values.

## Summary of Results and findings

- 57% of the total observations chose to accept the coupon, we can conclude that slightly more than half of the respondents were willing to use the coupon.

- The chart below shows that the most frequent venue type for which the coupon was accepted was 'coffee houses' followed by "less expensive restaurants" (under $20)." "Carry out & Take away and "Bars" had relatively lower frequencies, while "expensive restaurants" ($20 - $50)" had the lowest frequency among all the venue types. 

![download1](https://user-images.githubusercontent.com/130615319/235323865-4ba2f0a6-702d-4c74-8ab2-7a66c73c1997.png)
**********************************

 - The grapgh bellow shows that people accept more coupons if the weather is better.
 
 ![download2](https://user-images.githubusercontent.com/130615319/235325448-d2fcefde-6b3a-4e71-8e25-618fea5a07e1.png)
 **********************************
 
 ## 1- Investigating the Bar Coupons
 - Bellow is the percentage of bar coupons that were accepted: 41.19%
 ![download3](https://user-images.githubusercontent.com/130615319/235326612-61e5efd0-f236-456e-950f-49f3e913920a.png)
 
Bellow: 
- Acceptance rate for those who went to a bar 3 or fewer times a month: 37.24%
- Acceptance rate for those who went to a bar more than 3 times a month: 76.17%
- Note:
Acceptance rate for those who went to a bar 3 or fewer times a month: 37.24% Acceptance rate for those who went to a bar more than 3 times a month: 76.17% We can conclude that individuals who go to a bar more than 3 times a month are more likely to accept bar coupons compared to those who go to a bar 3 or fewer times a month. 

- Note: 
This suggests that frequent bar-goers have a higher interest in bar promotions and are more likely to take advantage of the coupons offered.
![download4](https://user-images.githubusercontent.com/130615319/235326714-734e5ef9-b193-4a11-aec8-35aa1a82bbf6.png)

*********************************************************






- Acceptance rate for drivers who go to a bar more than once a month and are over the age of 25: 68.98%
Acceptance rate for all other drivers: 33.73%

- Note:
 We can conclude that drivers who go to a bar more than once a month and are over the age of 25 are more likely to accept bar coupons compared to all other drivers. This indicates that targeting bar promotions to this specific demographic group (drivers over 25 who frequent bars more than once a month) may yield higher coupon acceptance rates and possibly higher sales or customer engagement.


**********************************************************


- Acceptance rate for drivers who go to a bar more than once a month, have passengers not kids, and have occupations other than farming, fishing, or forestry: 68.53%
Acceptance rate for all other drivers: 29.46%
 
- Note:
Acceptance rate for drivers who go to a bar more than once a month, have passengers not kids, and have occupations other than farming, fishing, or forestry: 68.53% Acceptance rate for all other drivers: 29.46% We can conclude that drivers who go to a bar more than once a month, have passengers that are not kids, and have occupations other than farming, fishing, or forestry are more likely to accept bar coupons compared to all other drivers. 
 
 *************************************************
 
 Compare the acceptance rates between those drivers who:
- go to bars more than once a month, had passengers that were not a kid, and were not widowed OR
- go to bars more than once a month and are under the age of 30 OR
- go to cheap restaurants more than 4 times a month and income is less than 50K.
 ![download5](https://user-images.githubusercontent.com/130615319/235327114-11f23962-9156-4fd0-a13f-3dd950516859.png)

 #### Conclusion1:
 
Based on these observations, what do you hypothesize about drivers who accepted the bar coupons?
Based on the observations, we can hypothesize that drivers who accepted the bar coupons are more likely to have certain characteristics. These drivers tend to:

- Visit bars more frequently (more than once a month).
- Be over the age of 25, especially when compared to all other drivers.
- Have passengers that are not kids.
- Work in occupations other than farming, fishing, or forestry.
- Not be widowed.
- Additionally, factors such as going to cheap restaurants more than 4 times a month and having an income less than 50K may also influence the acceptance rate of bar coupons, but the effect is less pronounced compared to the factors listed above.

*************************************
  ## 2- Investigating the coffee house and determine the characteristics of passengers who accept these coupons
  - After calculating the proportions of each category in categorical variables:
  
  
  ![download7](https://user-images.githubusercontent.com/130615319/235330691-8527fb5d-ec4b-4e7e-b257-9065432d846a.png)
  
- In conclusion, passengers who accepted coffee house coupons were more likely to have no urgent destination, be alone or with friends, experience sunny weather, and accept the coupon around mid-morning or early evening. They were also more likely to be single without children and have some college education or a bachelor's degree. Unemployed and student passengers showed the highest acceptance rates for coffee house coupons.
  
 Bellow:
 - Education Distribution by gender 
 
 ![download11](https://user-images.githubusercontent.com/130615319/235331709-08ffb97c-32d4-4332-bff4-d087a9568a56.png)
 
   - We can clearly see that the proportions are pretty close between genders, the Bachelors degree and people with some college- no dgree are more likely to accept coupons.
   
 
 ![download1010](https://user-images.githubusercontent.com/130615319/235331941-643253ee-8ad6-4abe-bdf5-2c8a435e9780.png)
  

  ![download99](https://user-images.githubusercontent.com/130615319/235332000-eb6183d7-994e-4284-ad48-63e43f20b09c.png)
![download88](https://user-images.githubusercontent.com/130615319/235332008-d80f9d08-b184-404b-b7ad-2708194a1441.png)
![download77](https://user-images.githubusercontent.com/130615319/235332012-862cad82-05d7-49c0-8682-e127cbefa90d.png)

![download66](https://user-images.githubusercontent.com/130615319/235332013-748b484f-e852-4dbe-86e7-d86b877a2b85.png)
![download55](https://user-images.githubusercontent.com/130615319/235332015-e7d0be30-5583-4604-a49e-f8b883166466.png)
![download33](https://user-images.githubusercontent.com/130615319/235332018-14de0f16-3b26-4ee8-a23f-fff4e2731194.png)
![download22](https://user-images.githubusercontent.com/130615319/235332022-0f598888-3da0-4829-8b63-e555f12be3f0.png)
  
  *************************************************************************
  ### Correlations between Categorical Variables and Coupon Acceptance
  
  ##### Conclusion:

  The result shows the correlation coefficients between the target variable (Y) and each categorical variable.
A positive correlation coefficient means that there is a positive association between the variable and the target variable. In this case, destination and passanger have positive correlation coefficients, which means that there is a higher chance of accepting the coupon when the destination is No Urgent Place or the passanger is Alone or with Friends.

A negative correlation coefficient means that there is a negative association between the variable and the target variable. In this case, time, gender, maritalStatus, and has_children have negative correlation coefficients, which means that there is a lower chance of accepting the coupon when the time is 10PM, the passenger is male, the driver is unmarried or divorced, or the driver has children.

A correlation coefficient close to 0 means that there is no significant correlation between the variable and the target variable. In this case, weather, education, and occupation have correlation coefficients close to 0.
  ![download222](https://user-images.githubusercontent.com/130615319/235332160-4e4f4854-78bf-4367-aed2-65e8cdc150a1.png)

![download111](https://user-images.githubusercontent.com/130615319/235332148-9cd90ee1-9b39-4781-bbe3-658d170fa32b.png)

![download333](https://user-images.githubusercontent.com/130615319/235332153-4524faa5-f80c-4b3e-8f73-47df09f1b93f.png)
  

  
  
  **********************************************************
  
  #### Final Conclusion:
  
  we can now provide a more comprehensive overview of the differences between customers who accepted coupons and those who didn't:

Coupon Type: Customers have varied preferences when it comes to coupon types. For example, some types of coupons, such as those for less expensive restaurants and coffee houses, might be more appealing than bar coupons. In fact, the overall acceptance rate for coffee house coupons was 50%, while bar coupons had a lower acceptance rate of 41%, with 785 accepted and 1121 not accepted.

Demographics and Behavior: A customer's age, gender, marital status, education, income, and frequency of visiting certain establishments can also impact their decision to accept or reject a coupon. For instance, drivers over the age of 25 who went to a bar more than once a month had an acceptance rate of 69%, compared to a 34% acceptance rate for all other drivers. Similarly, drivers who went to bars more than once a month, had passengers that weren't kids, and had occupations other than farming, fishing, or forestry also had an acceptance rate of 69%, while all other drivers had a rate of only 29%.

Weather and Temperature: Both weather conditions and temperature can affect coupon acceptance rates. Customers might be more willing to accept coupons on sunny days as opposed to rainy or snowy days. The data shows that the acceptance rate for sunny weather was 59%, while it dropped to 46% for rainy weather and 48% for snowy weather.

Time of Day: The time when a coupon is delivered can also influence a customer's decision. People might be more inclined to use coupons during popular meal times rather than early morning or late evening. The acceptance rate was the highest at 10 AM (63%) and the lowest at 10 PM (43%).

Passenger: Who is in the car with the customer can also impact their decision to accept a coupon. For example, customers might be less likely to accept a bar coupon if they have a minor passenger in the car. The data reveals that the acceptance rate was the highest when a friend was the passenger (60%) and the lowest when the customer was alone (43%).

In conclusion, a range of factors, such as coupon type, user demographics, behavior, weather, temperature, time of day, and passenger presence, can play a role in whether a customer chooses to accept or reject a coupon. To boost the likelihood of coupon acceptance, businesses should consider these factors when crafting their offers for potential customers.

Businesses can increase sales by tailoring coupon offers to customer preferences and trends, focusing on timing, demographics, and popular coupon types to create more appealing and effective promotions.
  

#### Next steps:
the results of this analysis provide valuable insights into the factors that influence customer coupon acceptance. By understanding these factors, businesses can target their promotions to specific demographic groups and optimize their marketing strategies for better returns on their promotional efforts. However, it's important to keep in mind that the results of this analysis are based on average values and may not apply to all customers in the same way. Further research and analysis may be necessary to gain a more comprehensive understanding of coupon acceptance behaviors.
