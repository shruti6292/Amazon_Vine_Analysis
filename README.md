# Amazon_Vine_Analysis

### Overview of the analysis: 

Analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. Main purpose of this analysis is then to determine if there is any bias toward favorable reviews from Vine members in our dataset.

### Procedure:

We haveaccess to approximately 50 datasets,each one containing reviews of a specific product, from clothing apparel to wireless products.
https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt

We picked music dataset and used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, we used PySpark, and Pandas to determine if there is any bias toward favorable reviews from Vine members in our dataset.
https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Music_v1_00.tsv.gz

### Results: After the analysis, we found, for our dataset

Number of Vine reviews:

![vine reviews](https://github.com/RGK73/Amazon_Vine_Analysis/blob/main/Images/total_vine_reviews.png)

and non-Vine reviews:

![non vine reviews](https://github.com/RGK73/Amazon_Vine_Analysis/blob/main/Images/total_non_vine_reviews.png)

For our music dataset number of Vine reviews with 5 stars were: 

![vine 5star reviews](https://github.com/RGK73/Amazon_Vine_Analysis/blob/main/Images/5star_vine_reviews.png)

For our music dataset number of non-Vine reviews with 5 stars were:

![non vine 5star reviews](https://github.com/RGK73/Amazon_Vine_Analysis/blob/main/Images/5star_non_vine_reviews.png)

Hence percentage of Vine reviews that were 5 stars is: 

![vine reviews](https://github.com/RGK73/Amazon_Vine_Analysis/blob/main/Images/percentage_5star_vine_reviews.png)

and percentage of non-Vine reviews that were 5 stars is: 

![vine reviews](https://github.com/RGK73/Amazon_Vine_Analysis/blob/main/Images/percentage_5star_non_vine_reviews.png)

### Summary: 

From the above analyzed data we concluded that there is no positivity bias for reviews in the Vine program. 
We could perform statistical analysis with this dataset to prove that music reviews are independent of paid vine reviewers.
Also. we could analyse other datasets like books, software, etc to confirm our findings.
