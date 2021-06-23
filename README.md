# Amazon Vine Analysis

## **Amazon Vine Analysis Overview:** 
The purpose of this project is to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. In this part of the project, I've chosen to analyze the luggage dataset reviews and used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. I used PySpark to determine if there is any bias toward favorable reviews from Vine members in the dataset.  The following summary of the analysis will be provided to Jennifer to submit to the SellBy stakeholders.

## **Amazon Vine Analysis Results:**
 ### Vine (Paid) Reviews
 
 ![paidreviews_df](Images/paidreviews_df.PNG)
 
 - The number of reviews written by paid Vine program members was **21**.  
 - The number of five-star reviews written by paid Vine program members was **10**. 
 - The percentage of Vine paid reviews that were five stars was **47.62%**. 
 
 ### Non-Vine (Unpaid) Reviews 
 
 ![unpaidreviews_df](Images/unpaidreviews_df.PNG)
 
 - The number of reviews written by unpaid or non-Vine customers was **6,690**.  
 - The number of five-star reviews written by unpaid or non-Vine customers was **3,448**. 
 - The percentage of unpaid or non-Vine customer reviews that were five stars was **51.54%**.


## **Amazon Vine Analysis Summary:** 
There are far fewer luggage reviews written by paid Vine members (21) vs. unpaid Vine customers (6,690). If you solely look at the percentages of five-star reviews as the benchmark, there is not a big difference so it doesn't appear that there's a positivity bias from paid Vine members.  My recommendation is that this needs to be explored further by doing an analysis on the one-star through four-star ratings from vine members and non-vine customers.  I also recommend performing the same analysis of other products' datasets to determine if there are similar results.  




