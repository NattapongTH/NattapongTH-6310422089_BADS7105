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
Click [here](https://www.kaggle.com/nattapongthanngam/clv-test-nattapong) to find my code  