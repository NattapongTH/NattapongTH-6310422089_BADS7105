# <p align="center"> Customer Segmentation  </p>
***
# Dashboard:


![alt](https:)

# Concept:
- Customer segmentation is the process of dividing customers into groups based on common characteristics so companies can market to each group effectively and appropriately.

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2006_Customer%20Segmentation%20(Supermarket%20Data)/photo/1.%20concept%20of%20customer%20segmentation.png)

 
- I will use K Mean method that the concept consist of
	- Starts with a first group of randomly selected centroids, which are used as the beginning points for every cluster, 
	- And then performs iterative (repetitive) calculations to optimize the positions of the centroids 

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2006_Customer%20Segmentation%20(Supermarket%20Data)/photo/2.%20K%20mean%20concept.png)

- Step of work
	- Click [here](https://www.kaggle.com/nattapongthanngam/kmean2) to found dashboard

	1. Prepare data by google bigquery (Require data = Customer ID, Spending and Visiting of each date)

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2006_Customer%20Segmentation%20(Supermarket%20Data)/photo/3.%20Data%20preparation.JPG)

	2. Follow code until amount of centroid selection step, use elbow method to select proper centroild 

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2006_Customer%20Segmentation%20(Supermarket%20Data)/photo/4.%20Number%20of%20centroid%20selection.jpg)

	3. Map centroid result with coustomer_id

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2006_Customer%20Segmentation%20(Supermarket%20Data)/photo/6.%20Map%20centroid.JPG)

	4. Check distribution of spending and visiting in each centroid
	
![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2006_Customer%20Segmentation%20(Supermarket%20Data)/photo/5.%20K_mean%20vs%20total%20spending.jpg)

	- The result of customer segmentation = High, Medium and Low spending customer
	
- 2 = I separate Churn only 2 step (1. Churn in Current month Churn and 2. Churn in Previous month)   
		
![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005_CLV%20Dashboard%20(Supermarket%20Data)/Photo/5.%20Status%20of%20customer%20by%20month.jpg)

- 1 = Customer who do not be register membership

5. Moreover, I want to show GAP between last visiting and 2nd last visiting

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005_CLV%20Dashboard%20(Supermarket%20Data)/Photo/6.%20GAP%20of%20visiting.JPG)

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

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005_CLV%20Dashboard%20(Supermarket%20Data)/Photo/8.%20Product%20recommendation.JPG)

- Top 5 Best seller
	- To maximize discount efficiency, top 5 best seller base on life stage
	- It can apply for "Market Basket Discounts"

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2005_CLV%20Dashboard%20(Supermarket%20Data)/Photo/9.%20Best%20seller.JPG)




