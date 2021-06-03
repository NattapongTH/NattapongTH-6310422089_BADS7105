# <p align="center"> Product Recommendation  </p>
***
# Output:
![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2007%20%E2%80%93%20Product%20Recommendation%20(Google%20Survey)/Photo/1.%20Result.JPG)

# Concept:
- Product recommendation is basically a filtering system that seeks to predict and show the items that a user would like to purchase. It may not be entirely accurate, but if it shows you what you like then it is doing its job right.

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2007%20%E2%80%93%20Product%20Recommendation%20(Google%20Survey)/Photo/3%20Recommend.png)

 
- After classroom survey (purchasing history of many item as 1. used to buy ("เคยซื้อ") and 2. never buy it ("ไม่เคยซื้อ")), the raw data is cleaned by replace NULL with never buy it. check data profiling, etc.

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2007%20%E2%80%93%20Product%20Recommendation%20(Google%20Survey)/Photo/2.%20Raw%20data.JPG)

- Then, criteria of basket analysis consist of
	1. 'Lift' > 1.01 --> Result =  416,718 row
	2. Limit item only 1 in 'Antecedents' and 'Consequents', Set 'Support' > 0.55 and set 'Confidence' > 0.91 --> Result = 29 row (my target is lower than 30)
                             
![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2007%20%E2%80%93%20Product%20Recommendation%20(Google%20Survey)/Photo/4.%20result%20from%20basket%20analysis.JPG)

- The result can apply for product recommendation. 

# Addtional for Community Detection:

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2007%20%E2%80%93%20Product%20Recommendation%20(Google%20Survey)/Photo/5.%20Community%20detection.png)

- Community detection algorithms are used to evaluate how groups of nodes are clustered or partitioned, as well as their tendency to strengthen or break apart.
- 1st result of Community Detection

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2007%20%E2%80%93%20Product%20Recommendation%20(Google%20Survey)/Photo/6.%20basis%20community%20detection.JPG)

- The popular method for community Detection consist of 3 type 
	
1. Degree Centrality

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2007%20%E2%80%93%20Product%20Recommendation%20(Google%20Survey)/Photo/7.%20first%20community%20detection.JPG)
	
2. Betweenness Centrality

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2007%20%E2%80%93%20Product%20Recommendation%20(Google%20Survey)/Photo/8.%202nd%20community%20detection.JPG)

3. Closeness Centrality

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2007%20%E2%80%93%20Product%20Recommendation%20(Google%20Survey)/Photo/9.%203rd%20community%20detection.JPG)