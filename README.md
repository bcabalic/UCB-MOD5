# UCB-MOD5
Module 5 - Factors in Coupon Acceptance While Driving

<h1>Problem Statement</h1>
When sending out coupons we want to focus on sending coupons that have the best chance of being accepted within certain conditions.
For this approach I will search for combinations of conditions where the acceptance rate is higher than any single baseline condition.

<h1>Primary Question</h1>  
Is there a combination of driving conditions that result in higher acceptance rates than any one single condition?
The main goal is to distinguish between customers who accepted a driving coupon versus those that did not.  I will demonstrate that through visualizations, but will also investigate an business use case for targeting conditions where there is a high probability of coupon acceptance. 

<h1>Business Context</h1> 
In the context of business, it is possible to optimize a coupon sending campaign by focusing on conditions that are historically in favor for customer acceptance.
For the purpose of this project I will define that as a <b>65% or higher</b> acceptance rate.

<h1>Key Research Questions</h1>
There is a lot of data to process here. 121 unique values over 25 columns. In order to process this data in a way that makes sense, I will look for trends in acceptance starting from a general view then drill down to specific conditions.<br>
<br>Example drill down:<br><br>
- What is the difference between male and female acceptors?<br>
- What is the difference between male and female acceptors, when it is snowing vs. sunny?<br>
- What is the difference between male and female acceptors, when it is snowing vs. sunny AND the coupon is for an location near by?<br>

<h1>Preliminary data discovery</h1> 
- Looked at all key data including shape, columns, unique values in columns, NaN entries<br>
- I found the 'car' column mostly irrelevant<br>
- I found columns with 'NaN' still relevant, decided not to replace values<br>

<h1>My process</h1>
First, I looked at all columns and ranked them by value and acceptance rate, I took the top 30 columns, which happen to show acceptance rates of 59.55% and above.<br><br>
Next, I observed the results and attempted to combine categories to see if any would yield even higher acceptance rates, following a similar drill down mentioned above.<br><br>
Finally, I made inferences from the plots as to which characteristics of customers can be targeted for coupon campaigns.<br><br>

<h1>Key findings</h1>
If you look at my Jupyter notebook, I answered all the default questions. Additionally I hand picked 3 key findings:

<h3>COUPON ACCEPTANCE FOR RESTAURANTS < 20min AND WITH FRIENDS EXCEED 80%</h3>
- If restaurant is less than 20 min away the acceptance rate is 70.71%.<br>
- However if a customer is travelling with friends the acceptance rate goes up to <b>80.15%</b>!<br>
- Without friends, the acceptance rate is stil high: 66.73%<br>
- If sent a coupon for a restaurant <20 miles, friends travelling together are <b>13.42%</b> more likely to accept than a solo traveler.<br>
- This condition is also <b>9.44%</b> higher than the general average of coupons accepted for restaurants within 20 min.<br>

<h3>SINGLES ARE LIKELY TO ACCEPT CARRYOUT/TAKEAWAY OR RESTAURANTS <20min AWAY</h3>
- The coupon acceptance rate for single people is 60.6% overall.<br>
- However, if coupon is for CarryOut/TakeAway or a Restaurant <20min away the acceptance rates jump to <b>75% and 73%</b> respectively! 

<h3>FOR 10am COUPONS THAT EXPIRE IN 1 DAY - FOCUS ON MALES, SINGLES, AND COFFEE!</h3>
- I sorted out the TOP 15 acceptance rates in this combined category: 10am coupons & 1-day expiration<br>
- Then I highlighted the TOP 3 counts (most relevant amount of customers)<br>
- If you're sending out a coupon at 10am with an 1d expiration - target these customers which have shown <b>65%+</b> acceptance rate historically:<br>
<br>
1. Males<br>
2. Singles<br>
3. Coffee coupons (will also attract customers that have been to a CoffeeHouse 1-8 times!)<br>

<h1>Summary</h1>


