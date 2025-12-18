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
I first looked at all columns and ranked them by value and acceptance rate, I took the top 30 columns, which happen to show all acceptance rates of 59.55% and above<br>
Next, I observed the results and attempted to combine categories to see if any would yield even higher acceptance rates, following a similar drill down mentioned above.<br>

<h1>Key findings</h1>


<h1>Summary</h1>


