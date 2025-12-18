# UCB-MOD5
Module 5 - Factors in Coupon Acceptance While Driving

<h1>Problem Statement</h1>
When sending out coupons we want to focus on sending coupons that have the best chance of being accepted within certain conditions.
For this approach I will search for combinations of conditions where the acceptance rate is extremely high.

<h1>Primary Question</h1>  
Is there a combination of driving conditions that result in higher acceptance rates than any one single condition?
The main goal is to distinguish between customers who accepted a driving coupon versus those that did not.  I will demonstrate that through visualizations, but will also investigate an business use case for targeting conditions where there is a high probability of coupon acceptance. 

<h1>Business Context</h1> 
In the context of business, it is possible to optimize the coupon sending campaign by focussing on conditions that are in our favor for the customer to accept the coupon.
I will define that as a <b>60% or higher</b> acceptance rate.

<h1>Key Research Questions</h1>
There is a lot of data to process here. 121 unique values over 25 columns. In order to process this data in a way that makes sense, I will look for trends in acceptance starting from a general view then drill down to specific conditions.<br>
<br>Example drill down:<br><br>
- What is the difference between male and female acceptors?<br>
- What is the difference between male and female acceptors, when it is snowing vs. sunny?<br>
- What is the difference betwwen male and female acceptors, when it is snowing vs. sunny AND the coupon is for an location near by?<br>

<h1>Preliminary data discovery</h1> 
- Looked at all key data including shape, columns, unique values in columns, NaN entries<br>
- I found the 'car' column mostly irrelevant<br>
- I found columns with 'NaN' still relevant, decided not to replace values<br>

<h1>My process</h1>
I first looked at all columns and ranked them by value and acceptance rate, I took the top 30 columns, which happen to show all acceptance rates of 59.55% and above.<br>
Next, I observed the results and attempted to combine categories to see if any would yield even higher acceptance rates, following a similar drill down mentioned above.<br>

<h1>Key findings</h1>
If you look at my Jupiter notebook, I answered all the default questions. Additionally I hand picked 3 key findings:

<h2>FINDING 1 - RESTAURANTS < 20 min AND WITH FRIENDS</h2>
If restaurant is less than 20 min away the acceptance rate is 70.71%.
*However if a customer is travelling with friends the acceptance rate goes up to <b>80.15%</b>!
Without friends, the acceptance rate is stil high: 66.73%

If sent a coupon for a restaurant within 20 miles, a group of friends travelling together is 13.42% more likely to accept the coupon than somone travelling solo.
This condition is also 9.44% higher than the general average of coupons accepted for restaurants within 20 min.

<h2>FINDING 2 - SINGLE PEOPLE ACCEPTANCE RATE</h2>
The coupon acceptance rate for single people is 60.6% overall. 
However, if the coupon is for CarryOut/TakeAway or a Restaurant < 20min away the acceptance rates jump to 75% and 73% respectively! 

<h2>FINDING 3 - 10am COUPONS THAT EXPIRE IN 1 DAY</h2>
I sorted out the TOP 15 acceptance rates in this combined category. Then I highlighted the TOP 3 counts (most relevant amount of customers)

If you're sending out a coupon at 10am with an 1d expiration - target these individuals (highest sample count in this set) which have shown 65%+ acceptance rate historically:

1. Males
2. Single people
3. Coffee coupons (will also attract customers that have been to a CoffeeHouse 1-8 times!)

<h1>Summary</h1>


