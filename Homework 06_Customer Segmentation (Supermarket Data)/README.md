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

5. After got K-Mean result, we should interpreting result

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2006_Customer%20Segmentation%20(Supermarket%20Data)/photo/8.%20Interpreting%20result.JPG)

6. Finally, we should apply other tools such as churn prediction, product recommendation, etc. and create action plan 
	
![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2006_Customer%20Segmentation%20(Supermarket%20Data)/photo/9.%20action%20plan.JPG)

- Another tool = Silhouette (only show result)
		
![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2006_Customer%20Segmentation%20(Supermarket%20Data)/photo/7.%20Sihouette.jpg)



