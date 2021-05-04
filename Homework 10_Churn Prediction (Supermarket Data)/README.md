# <p align="center"> Churn Prediction  </p>
***
# Dashboard:
- Click [here](https://datastudio.google.com/s/nTkFiWUHqu4) to found dashboard

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2010_Churn%20Prediction%20(Supermarket%20Data)/Photo/0.%20Dashboard.JPG)

# Concept:
- Customer churn (or customer attrition) is a tendency of customers to abandon a brand and stop being a paying client of a particular business. The percentage of customers that discontinue using a company’s products or services during a particular time period is called a customer churn (attrition) rate.

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2010_Churn%20Prediction%20(Supermarket%20Data)/Photo/1%20Churn%20concept.png)

 
- Use google bigquery to calculate churn monitoring by seperate 5 groups
	- REPEAT = Customer who purchase in last month + purchase in current month
	- REACTIVATED = Customer who purchase in last 2 month + not purchase in last month + back to purchase again in current month  
	- New = Customer who start purchase in current month
	- CHURN = Customer who purchase in last month + not purchase in current month
	- GONE = Customer who not purchase in 2 month or more

- Code of query
- Click [here](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2010_Churn%20Prediction%20(Supermarket%20Data)/Query%20code.docx) to found code in word

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2010_Churn%20Prediction%20(Supermarket%20Data)/Photo/2.%20Query%20result.JPG)

- Then, use result to query again

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2010_Churn%20Prediction%20(Supermarket%20Data)/Photo/3.%202nd%20query.JPG)

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



