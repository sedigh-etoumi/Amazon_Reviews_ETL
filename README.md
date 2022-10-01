# Amazon_Reviews_ETL

Overview: 
  In the assignment we are going to analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows           manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who     are then required to publish a review. So we are going to transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I’ll     use PySpark, to determine if there is any bias toward favorable reviews from Vine members in your dataset.

Analysis and Results:
- Filter the data and create a new DataFrame or table to retrieve all the rows where the total_votes count is equal to or greater than 20 as the following.
![](https://github.com/sedigh-etoumi/Amazon_Reviews_ETL/blob/main/Resources/images/total_vote_count.png)

- Filter the new DataFrame or table created in Step 1 and create a new DataFrame or table to retrieve all the rows where the number of helpful_votes divided by             total_votes is equal to or greater than 50%.
![](https://github.com/sedigh-etoumi/Amazon_Reviews_ETL/blob/main/Resources/images/last_vine_df.png)

- Filter the DataFrame or table created in Step 2, and create a new DataFrame or table that retrieves all the rows where a review was written as part of the Vine program (paid), vine == 'Y'.
![](https://github.com/sedigh-etoumi/Amazon_Reviews_ETL/blob/main/Resources/images/paid_5star_count_unpaid.png)

Repeat the previous step, but this time retrieve all the rows where the review was not part of the Vine program (unpaid), vine == 'N'.
![](https://github.com/sedigh-etoumi/Amazon_Reviews_ETL/blob/main/Resources/images/total_paid_reviews.png)

Determine the total number of reviews, the number of 5-star reviews, and the percentage of 5-star reviews for the two types of review (paid vs unpaid).
![](https://github.com/sedigh-etoumi/Amazon_Reviews_ETL/blob/main/Resources/images/percentage.png)

Summary: As the percentage of 5 stars paied reviews up to 51% we can significantly notice there is a bias for reviews in the Vine program. 


 
