# Amazon_Vine_Analysis
---------------------------------------------
# Over View on the project:
Since we worked with Jennifer on the SellBy project and it was so successful, I’ve been tasked with another, larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, I’ll have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. I'll need to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I’ll use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset. Then, i’ll write a summary of the analysis for Jennifer to submit to the SellBy stakeholders.

----------------------------------------------------------------------
# The challange main tools and results :
# Deliverable 1: Perform ETL on Amazon Product Reviews

with my knowledge of the cloud ETL process, I’ll create an AWS RDS database with tables in pgAdmin, pick a dataset from the Amazon Review datasets (Links to an external site.), and extract the dataset into a DataFrame. I'll transform the DataFrame into four separate DataFrames that match the table schema in pgAdmin. Then, I'll upload the transformed data into the appropriate tables and run queries in pgAdmin to confirm that the data has been uploaded.

1.customers table:

![this is picture](https://github.com/Farah86/Amazon_Vine_Analysis/blob/main/pics/customers1.png)

![this is picture](https://github.com/Farah86/Amazon_Vine_Analysis/blob/main/pics/customers2.png)

2.products table:

![this is picture](https://github.com/Farah86/Amazon_Vine_Analysis/blob/main/pics/producttable1.png)

![this is picture](https://github.com/Farah86/Amazon_Vine_Analysis/blob/main/pics/producttable2.png)

3.review table:

![this is picture](https://github.com/Farah86/Amazon_Vine_Analysis/blob/main/pics/reviewtable1.png)

![this is picture](https://github.com/Farah86/Amazon_Vine_Analysis/blob/main/pics/reviewtable2.png)

4.vine table:

![this is picture](https://github.com/Farah86/Amazon_Vine_Analysis/blob/main/pics/vinetable1.png)

![this is picture](https://github.com/Farah86/Amazon_Vine_Analysis/blob/main/pics/vinetable2.png)

# Deliverable 2: Determine Bias of Vine Reviews:

Using my knowledge of PySpark, Pandas, or SQL, I’ll determine if there is any bias towards reviews that were written as part of the Vine program. For this analysis, I'll determine if having a paid Vine review makes a difference in the percentage of 5-star reviews.

1.greater than 20 vine vote :

![this is picture](https://github.com/Farah86/Amazon_Vine_Analysis/blob/main/pics/greatervinevote.png)

2:helpfule vine vote review:

![this is picture](https://github.com/Farah86/Amazon_Vine_Analysis/blob/main/pics/helpfulvinevote.png)

3.review vine vote review:

![this is picture](https://github.com/Farah86/Amazon_Vine_Analysis/blob/main/pics/reviewvinevote.png)

4.retrive review vine votes:

![this is picture](https://github.com/Farah86/Amazon_Vine_Analysis/blob/main/pics/rreviewvinevote.png)


# Deliverable 3: A Written Report on the Analysis:

1.Overview of the analysis: ( already explaind in the first of the readme page)

2.Results:
we had 3 main questions to answer:
.How many Vine reviews and non-Vine reviews were there?

![this is picture](https://github.com/Farah86/Amazon_Vine_Analysis/blob/main/pics/totalpaidreview.png)

and for the unpaid review it was=39869

.How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

![this is picture](https://github.com/Farah86/Amazon_Vine_Analysis/blob/main/pics/5starreviewpaid.png)

and for the unpaid review it was=21005

.What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

![this is picture](https://github.com/Farah86/Amazon_Vine_Analysis/blob/main/pics/precentage5starreview.png)

and for the unpaid review it was=52.68504351751988

3.Summary:

Based on the results i could'nt see any positive bias as to whether the paid Vine participants are producing more positive reviews of products compared to the non-Vine (unpaid) participants,same thing would go withe precentage and the compaired between  paid and unpaid 5 star viewers .
i would suggest that we go for less than 5 star viewres maybe the diffrent will appear more ...
