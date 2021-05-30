# <p align="center"> Customer Lifetime Value </p>
***
# Dashboard:
- Click [here](https://datastudio.google.com/s/nn9ahwywKto) to found dashboard

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005%20%E2%80%93%20CLV%20Dashboard(Supermarket%20Data)/Photo/0.%20Result.JPG)

# Concept:
- I design dashboard to use as routine. Therefore, the data is calculate base on 3 months (Apr - Jun 2008) 
- Customer Lifetime Value (CLV) represents the average amount of money a customer is expected to spend on a specific organisation or brand over their entire lifetime.
- Design concept of work
	- Use Lifetime package in Python to calculate CLV
	- Merge result with other homework (Churn analysis, Customer segmentation) to group custmer
	- Match proper compaign to each segment of customer

- Lifetime package in python 
	- Use Recency, Frequency and Monetary (RFM) Analysis to calculate CLV Calculation
	- The RFM matrix segments the contact base based on recency, frequency, and monetary value of purchases for a specified period.
		1. Average purchase value = total sales/orders.
		2. Purchase frequency = orders/contacts.
		3. Customer value = average purchase value × purchase frequency.

# Source:
- Open data from dunnhumby (I highlight some interesting topic)

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005%20%E2%80%93%20CLV%20Dashboard(Supermarket%20Data)/Photo/Raw%20data_CLV.JPG)

# Step of work:
1. I use excel to preview data first. It is not too big so I use excel function to convert date from YYYYMMDD to DD-MMM-YYYY
2. Use google bigquenry to summary data (Expected result = 1 line/(Customer_ID + Date + Total_Spending)

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005%20%E2%80%93%20CLV%20Dashboard(Supermarket%20Data)/Photo/1.%20GBQ%20for%20CLV.JPG)

3. Use python to calculate CLV by use Lifetime package
	- Click [here](https://www.kaggle.com/nattapongthanngam/clv-test-nattapong) to find my code
	- Let's me show some interesting result (1. Frequency/Recency matrix and 2. CLV result) 

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005%20%E2%80%93%20CLV%20Dashboard(Supermarket%20Data)/Photo/2.%20RF%20result.JPG) 

	- F/R matrix able to show "Expected number of future purchases for 1 unit of time" and "Probability Customer is Alive" 
	- For CLV result, I assume monthly discount rate=0.01 (~ 12.7% annually)

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005%20%E2%80%93%20CLV%20Dashboard(Supermarket%20Data)/Photo/3.%20CLV%20result.JPG)

4. After got CLV by customer, I merge result of Churn analysis, Customer segmentation and set segmentation name as 3+2+1

- 3 = "Customer segmentation from K-Mean"
	- Click [here](https://www.kaggle.com/nattapongthanngam/kmean2) to find my code

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005%20%E2%80%93%20CLV%20Dashboard(Supermarket%20Data)/Photo/4.%20KMEAN%20result.jpg)

	- The result of customer segmentation = High, Medium and Low spending customer
	
- 2 = I separate Churn only 2 step (1. Churn in Current month Churn and 2. Churn in Previous month)   
		
![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005%20%E2%80%93%20CLV%20Dashboard(Supermarket%20Data)/Photo/5.%20Status%20of%20customer%20by%20month.jpg)

- 1 = Customer who do not be register membership

5. Moreover, I want to show GAP between last visiting and 2nd last visiting

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005%20%E2%80%93%20CLV%20Dashboard(Supermarket%20Data)/Photo/6.%20GAP%20of%20visiting.JPG)

6. Set name of each group
	- EPIC = Low spending customer
	- LEGENDARY = Medium spending customer
	- CELESTIAL = High spending customer
	- CHURN = Customer who do not visit shop in this month
	- GHOST = Customer who do not visit shop longer than 2 month
	- SHADOW = Non-member customer


7. Set campaign idea
	- For membership
		- Special New Year Gift = To make premium member impact (only CELESTIAL member)
		- Special Birthday Discount = To make premium member impact (only CELESTIAL and LEGENDARY member)  
		- Market Basket Discounts = To create brand loyalty. market basket analysis able to reduce churn rate (only CELESTIAL, LEGENDARY and EPIC member) 
	- For churn customer
		- Special Coupon Discount (1D expired) = To make special attractiveness (only CHURN member)
		- Coupon Discount (Top 5 Best Seller) = To make special attractiveness (only CHURN and GHOST member)
	- For non-member
		- New Member Discount = To convince non-member customer to be member (only non-member)
	- For all
		- "Pack set" such as (5 free 1), (11 free 1), etc. --> To upsell (stretch spending)
		- "Premium Gift" such as buy 5 give plastic bag, buy over 1,000 give glass = To upsell (stretch spending)
		- Common Discount via mobile application, line program, website, etc. --> To increase brand awareness

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005_CLV%20Dashboard%20(Supermarket%20Data)/Photo/7.%20Creating%20value%20from%20clustering%20results.JPG)

8. Additonal
- Product recommendation
	- Click [here](https://www.kaggle.com/nattapongthanngam/recommendation-nattapong) to found dashboard
	- It can apply for "Market Basket Discounts"

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005%20%E2%80%93%20CLV%20Dashboard(Supermarket%20Data)/Photo/8.%20Product%20recommendation.JPG)

- Top 5 Best seller
	- To maximize discount efficiency, top 5 best seller base on life stage
	- It can apply for "Market Basket Discounts"

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005%20%E2%80%93%20CLV%20Dashboard(Supermarket%20Data)/Photo/9.%20Best%20seller.JPG)

- Monthly dashboard 
	- Use to monitor shop performance. It can use for preformance monitoring after campaign implementation

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005%20%E2%80%93%20CLV%20Dashboard(Supermarket%20Data)/Photo/12.%20monthly%20dashboard.JPG)











