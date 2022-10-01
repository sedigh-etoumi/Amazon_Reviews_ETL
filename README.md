# Amazon_Reviews_ETL

Overview: 
  In the assignment we are going to analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows           manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who     are then required to publish a review. So we are going to transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I’ll     use PySpark, to determine if there is any bias toward favorable reviews from Vine members in your dataset.

Analysis and Results:
- Filter the data and create a new DataFrame or table to retrieve all the rows where the total_votes count is equal to or greater than 20 as the following.
![]
