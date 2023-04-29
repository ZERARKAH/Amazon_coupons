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

![download1](https://user-images.githubusercontent.com/130615319/235323865-4ba2f0a6-702d-4c74-8ab2-7a66c73c1997.png)

- The chart shows that the most frequent venue type for which the coupon was accepted was 'coffee houses' followed by "less expensive restaurants" (under $20)." "Carry out & Take away and "Bars" had relatively lower frequencies, while "expensive restaurants" ($20 - $50)" had the lowest frequency among all the venue types.
 
 
The differences between customers who did and did not accept the coupons:

we can now provide a more comprehensive overview of the differences between customers who accepted coupons and those who didn't:

Coupon Type: Customers have varied preferences when it comes to coupon types. For example, some types of coupons, such as those for less expensive restaurants and coffee houses, might be more appealing than bar coupons. In fact, the overall acceptance rate for coffee house coupons was 50%, while bar coupons had a lower acceptance rate of 41%, with 785 accepted and 1121 not accepted.

Demographics and Behavior: A customer's age, gender, marital status, education, income, and frequency of visiting certain establishments can also impact their decision to accept or reject a coupon. For instance, drivers over the age of 25 who went to a bar more than once a month had an acceptance rate of 69%, compared to a 34% acceptance rate for all other drivers. Similarly, drivers who went to bars more than once a month, had passengers that weren't kids, and had occupations other than farming, fishing, or forestry also had an acceptance rate of 69%, while all other drivers had a rate of only 29%.

Weather and Temperature: Both weather conditions and temperature can affect coupon acceptance rates. Customers might be more willing to accept coupons on sunny days as opposed to rainy or snowy days. The data shows that the acceptance rate for sunny weather was 59%, while it dropped to 46% for rainy weather and 48% for snowy weather.

Time of Day: The time when a coupon is delivered can also influence a customer's decision. People might be more inclined to use coupons during popular meal times rather than early morning or late evening. The acceptance rate was the highest at 10 AM (63%) and the lowest at 10 PM (43%).

Passenger: Who is in the car with the customer can also impact their decision to accept a coupon. For example, customers might be less likely to accept a bar coupon if they have a minor passenger in the car. The data reveals that the acceptance rate was the highest when a friend was the passenger (60%) and the lowest when the customer was alone (43%).

In conclusion, a range of factors, such as coupon type, user demographics, behavior, weather, temperature, time of day, and passenger presence, can play a role in whether a customer chooses to accept or reject a coupon. To boost the likelihood of coupon acceptance, businesses should consider these factors when crafting their offers for potential customers.

Businesses can increase sales by tailoring coupon offers to customer preferences and trends, focusing on timing, demographics, and popular coupon types to create more appealing and effective promotions.



Customer Coupon Acceptance Report
This report summarizes the findings from an analysis of a dataset that describes the likelihood of a customer accepting a coupon for a restaurant, coffee house, bar, or other food venue. The data was collected via a survey on Amazon Mechanical Turk and includes demographic information about the customer (such as age, marital status, education, occupation, and number of times they visit a specific venue), contextual information about the driving scenario (such as weather, time of day, passenger, and location), and coupon information (such as the type of coupon and time before it expires).

Summary of Results
The analysis found that certain demographic and contextual factors significantly influence the acceptance rate of coupons. Some of the key findings are:

Drivers who go to bars more frequently (more than once a month) and are over the age of 25 have a higher acceptance rate (68.98%) compared to all other drivers (33.73%).

Drivers who visit coffee houses more frequently (1-3 times a month) and are over the age of 25 have a higher acceptance rate (65.11%) compared to all other drivers (41.81%).

Drivers with friends as passengers have the highest acceptance rate for coffee coupons (67.60%), followed by drivers with their partner as a passenger (59.33%). Drivers who are alone or have kids as passengers have lower acceptance rates (52.56% and 49.62%, respectively).

The acceptance rate for bar coupons is higher for drivers who go to a bar more than 3 times a month (76.17%) compared to those who go 3 or fewer times a month (37.24%).

The acceptance rate for drivers who go to cheap restaurants more than 4 times a month and have an income less than $50K is around 60%.

Conclusion
In conclusion, the results of this analysis provide valuable insights into the factors that influence customer coupon acceptance. By understanding these factors, businesses can target their promotions to specific demographic groups and optimize their marketing strategies for better returns on their promotional efforts. However, it's important to keep in mind that the results of this analysis are based on average values and may not apply to all customers in the same way. Further research and analysis may be necessary to gain a more comprehensive understanding of coupon acceptance behaviors.
