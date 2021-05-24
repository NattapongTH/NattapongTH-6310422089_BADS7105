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

Result of Churn rate graph by use google studio

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2010_Churn%20Prediction%20(Supermarket%20Data)/Photo/6.%20Churn%20rate%20graph.JPG)

- Use same concept of 1st query to find gap of visiting

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2010_Churn%20Prediction%20(Supermarket%20Data)/Photo/4.%203rd%20query.JPG)

# Additonal:
- Create monthly dashboard by use google studio

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2010_Churn%20Prediction%20(Supermarket%20Data)/Photo/5.%20monthly%20dashboard.JPG)

# Recommendation:
- Finally, we should apply other tools such as customer segmentation, product recommendation, etc. and create action plan to reduce churn rate


