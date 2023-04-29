# Amazon_coupons


# Will a Customer Accept the Coupon?

Context


Imagine driving through town and a coupon is delivered to your cell phone for a restaraunt near where you are driving. Would you accept that coupon and take a short detour to the restaraunt? Would you accept the coupon but use it on a sunbsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaraunt? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?

Overview

The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

Data

This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’. There are five different types of coupons -- less expensive restaurants (under $20), coffee houses, carry out & take away, bar, and more expensive restaurants ($20 - $50). 


Data Description¶
Keep in mind that these values mentioned below are average values.

The attributes of this data set include:

User attributes
Gender: male, female
Age: below 21, 21 to 25, 26 to 30, etc.
Marital Status: single, married partner, unmarried partner, or widowed
Number of children: 0, 1, or more than 1
Education: high school, bachelors degree, associates degree, or graduate degree
Occupation: architecture & engineering, business & financial, etc.
Annual income: less than $12500, $12500 - $24999, $25000 - $37499, etc.
Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
Number of times that he/she buys takeaway food: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
Number of times that he/she goes to a coffee house: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
Number of times that he/she eats at a restaurant with average expense less than $20 per person: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
Contextual attributes
Driving destination: home, work, or no urgent destination
Location of user, coupon and destination: we provide a map to show the geographical location of the user, destination, and the venue, and we mark the distance between each two places with time of driving. The user can see whether the venue is in the same direction as the destination.
Weather: sunny, rainy, or snowy
Temperature: 30F, 55F, or 80F
Time: 10AM, 2PM, or 6PM
Passenger: alone, partner, kid(s), or friend(s)
Coupon attributes
time before it expires: 2 hours or one day.

Deliverables
 [Jupyter notebook](https://github.com/ZERARKAH/Amazon_coupons/blob/da30e4371936c06cc978ae41f135aadb3d0f6969/prompt.ipynb)
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
