# Capstone_assignment

Introduction:
The goal for this project will be to predict the needed income to be able to afford a home in those counties listed in the dataset. As the prices inflate by 6.6% all over the United States in our current economical state, we will be able to calculate the average of the houses in the county and predict the new income the individual will need. I chose the states of Maryland and Virginia for this project as the data comes from my own work experience with my company. This can later be used to predict the average needed all throughout the country. If the pricing of homes constructed in certain counties areaffordable then people who will meet the income minimum will be able to purchase. I used the price range from the lower 500’s to a million-dollar homes which have been constructed and sold. This will also show the difference in the income needed to purchase a average home compared to an above average home. By doing this builders will be able to price home adequately for the incomes in that area.

Literature Review:


While researching I found an article that explains a similar situation in the United Kingdom. As Attanasio explained in the article “Changes to current and future expected income, to interest rates and to house prices are all likely to affect both the propensity individuals have to own rather than to rent and also the size (and value) of the house they would like to live in”(Attanasio, 2004, pg 1). Although this focuses a bit more on future expectations it gives insight on how the income to house price ratio is one sided. If the prices of homes were to be lower than the buyer or individual would be able to purchase a home rather than rent a home. They would be able to put the payment for “rent” into an actual mortgage payment, basically by renting one loses money as you are not certain that location will be yours. Although they did not solve my question, they based most of their research on the age and how successful the purchasers were at their current ages. I have not seen another analysis like what I plan on doing. 
While searching for similar research I came upon a short blog written by Cororaton, she explained how some buyers will be looking for cheaper houses although with the inflation coming in that will be impossible as it will cause the already high prices to sky rocket even more. Ultimately causing those purchasers to wait until after the economy has settled down. 

Data Exploration: 
	Since the data set that I am using was created myself, I will be all 6 of the variables which are ID which differentiates each home, County, Income_average which is the average income in that county, Price_Home_average which is the average home price in that area, Home_Price which is the price of the home which was built there, Address and the State of which it is in. I won’t need to scratch anything out as I only included what is necessary for this to work, I might end up adding 1 or 2 more variables if I need to.
	The methods I plan to use to be able to solve my question will be a standard regression model as it will compare 2 variables to see if it has an impact on the other. Also, I can use a logistic model which will work as I can use 2 variables to show if they have a positive or negative relationship. A pro for the logistic model is that it is easy to interpret but a con is that it won’t work if you don’t have a dependent and an independent variable. Also, for the standard regression it will work great with a clean data set but if it has any errors, it will provide it bad outcome with poor quality. Then K cluster method will be used to basically interpret the new incomes needed to see of the similarities that of the old incomes acquired. An glm was also used to show the distribution of both the old and new findings. The visual was made to help understand the difference better as it is not a big jump in numbers but it still impacts what individuals need to make. Then a tree model was brought into to reflect those new incomes for the prices of the homes. 
 
Summary statistics:
Price_Home_Average 
sum = $13,800,000    min = $339,000
mean = $511,111       max = $725,000
Income_average
sum = $2,892,922  min = $79,415
mean = $107,145.26   max = $141,111
Home_Price
sum = $28,654,459  min = $500,000
mean = $1,061,276.26  max = $7,880,857
County 
Montgomery = 3  Cecil = 2 
Loudoun = 2  Howard = 3
Frederick = 5   Prince George = 6 
Charles = 2  Fairfax = 4
State
VA = 6
MD = 21



Data Analysis:
	To start we began with a sorted set of data which was categorized by the county and ID values to differentiate which observation is from where. This was a year worth of data gathered by taking the location of projects done in those counties. The income data was gathered through the United States Census Bureau where they have the sorted out by counties. Since the dataset had multiple counties, I decided to break each county into smaller subsets. By doing so we could display the difference between each county such as their Income, Average price, and the current price of a house being sold in that area. After analyzing the data there we no missing values or duplicates. In the dataset all the counties seemed to have the same amount of observations but Prince George and Frederick county had a couple more than the others. 
	
	The first result we had was how the inflation percentage of 6.6 had on the income of individuals in those certain counties. Depending on their income the range that the income had to go up to satisfy the house prices was from $5,000 to $9,500. So if an individual was making $111,812 in Montgomery they now would have to make at least $120,000 to be able to comfortable afford a home in the high $500k. For those individuals in Loudon county the increase in income was nearly $9,500 which bumps up the total needed income to $150,500 to afford a $700k home over a 30 year loan. Continuing onto Cecil County the increase caused by the inflation an individual will need to make an extra $5,500 which brings up the total income to $84,600. In this case it is not a negative effect to this county as the recommended amount is $70,000 for a $340,000 house. They could easily find a more expensive house in that area and be able to afford it. Then onto Howard county the increase in the income was of $8,180, which then brings up the total income to $132,200 which puts them past the needed amount for a $575,000 home. In Frederick County the inflation amount to the income was not a drastic change compared to others, it was of about $6,600. Bringing up the total income needed in that county to $107,330 which well over being able to afford a $420,000 home.
	
	The County of Prince George was next on the list with the new increase needed of $5,700 to the new income. This raises up the income to $92,700 which puts them right above the margin of being able to afford a Home of $410,000. The baseline for that was $89,000 so it is a positive turn for that county. Next in Charles county the inflation amount was of $6,842 making it the 4th largest out of the 7 counties so far. It boosts up the income needed up to $110,500, this one seems to have a positive increase as it puts it over the old needed income of affording a $425000 home. Finally in Fairfax County the rise was of $8,349 which brings up the income up to $136,000 which allows the individual to afford a home of nearly $160,000. 
	Overall most new incomes are not too far off of being able to afford an average home in there counties. Others do have the ability to even buy a slightly more expensive home with the current market. Although there are many other factors that can affect it afterwards such as loan interest rates or if they already own a property.
