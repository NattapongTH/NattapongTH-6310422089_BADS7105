# <p align="center"> Customer Lifetime Value </p>
***

# Concept:
- Customer Lifetime Value (CLV) represents the average amount of money a customer is expected to spend on a specific organisation or brand over their entire lifetime.
- Step of work
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
- Survey interesting and frequency of student about food, hobby and content 

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2001_Analysis%20of%20Customer/Photo/9.%20Survey.jpg)

- Result of the survey 

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2001_Analysis%20of%20Customer/Photo/9.%20Result%20of%20Survey.JPG)

- Summary topic table 

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2001_Analysis%20of%20Customer/Photo/9.%20Topic%20summary%20from%20Survey.JPG)


# Data preparation:
- Convert ranking to numbering such as "สนใจอย่างมากที่สุด" = 7, "สนใจอย่างมาก" = 6, ... , ไม่สนใจอย่างมากที่สุด = "1"

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2001_Analysis%20of%20Customer/Photo/9.%20Convery%20ranking%20to%20numbering.JPG)

- Convert birthday to zodiac type as Libra (ราศีตุลย์), Scorpio (ราศีพิจิก), ...

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2001_Analysis%20of%20Customer/Photo/9.%20DOB.jpg)

# Analysis concept:  
- The top average score is the most favorite of each zodiac  
 
# Result:  
- Food: Love "Japanese" but Eat "Thai"

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2001_Analysis%20of%20Customer/Photo/9.%20Food%20summary.JPG)

- Hobby:
	- Aries, Gemini, Cancer, Leo, Libra and Aquarius are love home activity (Reading and Watching movie/series/youtube)
	- Taurus, Scorpio and Capricorn are love outdoor activity (Travel)
	- However, all of zodiac spend time on youtube higher than other activities

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2001_Analysis%20of%20Customer/Photo/9.%20Hobby%20summary.JPG)

- Content:
	- Food, Travel and Politics are recommend. 

![alt](https://github.com/NattapongTH/NattapongTH-6310422089_BADS7105/blob/main/Homework%2001_Analysis%20of%20Customer/Photo/9.%20Content%20summary.JPG)