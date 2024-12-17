Will a Customer Accept the Coupon?

Context

Imagine driving through town and a coupon is delivered to your cell phone for a restaraunt near where you are driving. Would you accept that coupon and take a short detour to the restaraunt? Would you accept the coupon but use it on a sunbsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaraunt? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?

Overview

The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

Data

This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’. There are five different types of coupons -- less expensive restaurants (under $20), coffee houses, carry out & take away, bar, and more expensive restaurants ($20 - $50).

--------------------------------------------------------------------------------------------------------------------

Introduction :

Data is loaded to a Pandas dataframe , it is checked for the coulmns and data types. Then it is evaluated for null values and then null values are replaced wherever required or useful
For this project, we have replaced the null values for "Bar" and "CoffeeHouse" attributes by assuming that null values can be very well treated as 0. We have extensively used value_counts()
function on various attributes to understand the data well.

To visualize we have plotted bar plot for "coupon" column

![Screenshot (120)](https://github.com/user-attachments/assets/ca81b378-f8f3-4bc8-bc53-0e5f1705748f)


To visualize coupon acceptance based on temperature we have plotted coupon acceptance against temperature 



Overall 56.84% customers accepted the coupons

The analysis for this project is performed for two types of coupons 
 1. Bar Coupons
 2. Coffee House Coupons



Bar Coupon Analysis : 


Histogram of Bar Coupons is implemented against the temperature. 

![Screenshot (122)](https://github.com/user-attachments/assets/0bf09595-1abc-4920-8b70-d54d053da3b1)


Here is visualization of Bar Coupon acceptance based on how many times customer goes to a bar in a month

![Screenshot (123)](https://github.com/user-attachments/assets/1dcc4519-72b2-4759-a240-300bb7993940)



Summary for Bar Coupon Acceptance : 

We have filtered the data for Bar Coupons and we observed that overall 41% people accepted the Bar Coupons.

37% coupons were accepted for people who went less than 3 times to bar in a month whereas 76% coupons were accepted by people who went to bar more than 3 times in a month

69.52% people who are above age 25 and go to bar at least once a month accepted the coupons

71% people who go to bar more than once a month and who were NOT accompanied by kids and have business other than farming fishing and forestry accepted the coupons 

64.77% people who have salary less than 50K , are younger and go to cheaper restaurants accepted the coupons. 

So the people who go to bar more frequently or people who at least go once a month and not accompanied with kids and are older than 25 years will more likely to accept the coupons 



Coffee House Coupon Analysis : 


We have filtered the data for Coffee House Coupons and we observed that overall 50% people accepted the Coffee House Coupons.

here is visualization of coupon acceptance based on how many times customers go to Cofee House in a month

![Screenshot (124)](https://github.com/user-attachments/assets/6c2f2eb0-1ace-42c9-add4-e14be5818061)


Histogram visualization of Coffee House coupon acceptance based on temperature.

![Screenshot (125)](https://github.com/user-attachments/assets/02fc775e-744c-4fed-ae6b-5d22ddd84979)



Visualization to find out which age groups accept maximum coffee house coupons based on age.

![Screenshot (126)](https://github.com/user-attachments/assets/97ef038a-32e0-431d-ab92-fa97568986d6)



Summary for Coffee Coupon Acceptance : 

Overall 50% coffee coupons were accepted.

45% coupons were accepted for people who went less than 3 times to coffee house in a month whereas 67.5% coupons were accepted by people who went to coffee house more than 3 times in a month

63.84% people who are above age 25 and go to coffee house at least once a month accepted the coupons where as 55 % people who are younger than 25 years age have accepted the coupon.


50% people who have salary less than 50K and visit cheaper restaurants accepted the coupons 

58% people who are traveling to “no urgent destination” accepted the coupons where are only 40% of the people who are going to work or home accepted the coupon

So the people who go to coffee house more frequently or people who at least go once a month to coffee house and are older than 25 years will more likely to accept the coupons 








 
