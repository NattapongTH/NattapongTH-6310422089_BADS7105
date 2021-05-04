# <p align="center"> Customer Lifetime Value </p>
***

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

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005_CLV%20Dashboard%20(Supermarket%20Data)/Photo/Raw%20data_CLV.JPG)

# Step of work:
1. I use excel to preview data first. It is not too big so I use excel function to convert date from YYYYMMDD to DD-MMM-YYYY
2. Use google bigquenry to summary data (Expected result = 1 line/(Customer_ID + Date + Total_Spending)

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005_CLV%20Dashboard%20(Supermarket%20Data)/Photo/1.%20GBQ%20for%20CLV.JPG)

3. Use python to calculate CLV by use Lifetime package
	- Click [here](https://www.kaggle.com/nattapongthanngam/clv-test-nattapong) to find my code
	- Let's me show some interesting result (1. Frequency/Recency matrix and 2. CLV result) 

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005_CLV%20Dashboard%20(Supermarket%20Data)/Photo/2.%20RF%20result.JPG) 

	- F/R matrix able to show "Expected number of future purchases for 1 unit of time" and "Probability Customer is Alive" 
	- For CLV result, I assume monthly discount rate=0.01 (~ 12.7% annually)

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005_CLV%20Dashboard%20(Supermarket%20Data)/Photo/3.%20CLV%20result.JPG)

4. After got CLV by customer, I merge result of Churn analysis, Customer segmentation and set segmentation name as 3+2+1

	- 3 = "Customer segmentation from K-Mean"
	- Click [here](https://www.kaggle.com/nattapongthanngam/kmean2) to find my code

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005_CLV%20Dashboard%20(Supermarket%20Data)/Photo/4.%20KMEAN%20result.jpg)

	- The result of customer segmentation = High/Medium/Low customer
	
	- 2 = I separate Churn only 2 step (1. Churn in Current month Churn and 2. Churn in Previous month)   
		
![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005_CLV%20Dashboard%20(Supermarket%20Data)/Photo/5..%20Status%20of%20customer%20by%20month.jpg)




