# Airbnb_London_Sentiment_Price_Prediction

Data source : http://insideairbnb.com/ [9 Feb, 2021 London Archives] 
Content: Listings and Reviews

## Wrangling and Exploring Data  

Neighbourhood_group column is 100% missing, hence removed.
Last_review column’s missing values have been imputed by 0. Assumption: there are no reviews for those listings
Name identifiers have been removed since we have ids if needed

INSIGHTS:
Host 33889201 outmatches others by a lot (800+ listings)
Westminster is the neighbourhood with the most listings
Most listings are of the type: Entire home/apt or Private room

Price, no. of reviews and minimum nights are highly skewed 
For a better visualization, we remove extreme values of price during bivariate analysis.

Hotel rooms have the highest range in prices, closely followed by Entire home/apt.
In general,Hotel rooms and Entire home/apt are more expensive than Shared or Private rooms
Listings in central London have, in general, high availability
Most reviews are in English language out of 44 total languages

Hotel rooms have the highest range in prices, closely followed by Entire home/apt.
In general,Hotel rooms and Entire home/apt are more expensive than Shared or Private rooms
Listings in central London have, in general, high availability
Most reviews are in English language out of 44 total languages

## Review Sentiment Analysis

Business Use Case : Ease of processing feedback from customers
Methodology : Unsupervised learning English comments using Vader
Created variable : Sentiment Score (Range: -1 to  1, measuring positive/negative/neutral sentiment)
Bucketed Score as per industry standards to label sentiments as positive, medium, or negative.

Most comments are positive
People like when the place is clean and comfortable the host is friendly and the neighbourhood is centrally located.
Performance of most reviewed listing dropped in 2020 probably due to Covid
Highest Scored Listing-99241. Highest Scored Host- The Portobello Room
Note- Only considered listings, hosts with at least 50 reviews for point 4.



