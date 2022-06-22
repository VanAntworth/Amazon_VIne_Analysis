## Amazon_Vine_Analysis


# Overview of the analysis:

Picked a dataset from the Amazon Review datasets.

https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Kitchen_v1_00.tsv.gz

Extract the dataset into a DataFrame(google colab, pyspark)
<img width="1820" alt="Screen Shot 2022-06-22 at 9 56 33 AM" src="https://user-images.githubusercontent.com/99001393/175066036-9d96d3d5-5f1b-4541-b12f-345651c67dd4.png">

Transform the DataFrame into four separate DataFrames that match the table schema in pgAdmin
<img width="1342" alt="Screen Shot 2022-06-21 at 8 32 32 PM" src="https://user-images.githubusercontent.com/99001393/175066178-faf6cc57-5041-4467-9924-d624d26d179c.png">
<img width="1048" alt="Screen Shot 2022-06-21 at 8 32 48 PM" src="https://user-images.githubusercontent.com/99001393/175066190-618258d2-05c9-44c7-b53a-a0a1fb082074.png">
<img width="1142" alt="Screen Shot 2022-06-21 at 8 33 01 PM" src="https://user-images.githubusercontent.com/99001393/175066196-4d691c54-0fbf-475d-ab5d-6738c344c854.png">
<img width="1383" alt="Screen Shot 2022-06-21 at 8 33 20 PM" src="https://user-images.githubusercontent.com/99001393/175066208-b7e4df38-7fef-4161-b28f-77e09e08c4b3.png">


Upload the transformed data into the appropriate tables and run queries in pgAdmin to confirm that the data has been uploaded.
<img width="391" alt="Screen Shot 2022-06-22 at 10 02 18 AM" src="https://user-images.githubusercontent.com/99001393/175066570-c64411dd-a2a1-44b7-882e-baf30c0d2170.png">
<img width="805" alt="Screen Shot 2022-06-22 at 9 57 18 AM" src="https://user-images.githubusercontent.com/99001393/175066589-5cfd61e2-059e-4ca0-bca7-1f0a8c0afaa2.png">





# Purpose:
Determining if having a paid Vine review makes a difference in the percentage of 5-star reviews.

Results: 

* How many Vine reviews and non-Vine reviews were there?
  
  * Vine:1207
  * Non-Vine:97839

* How many Vine reviews were 5 stars? 

  * 509

* How many non-Vine reviews were 5 stars?

  * 45858

* What percentage of Vine reviews were 5 stars? 

  * 42%

* What percentage of non-Vine reviews were 5 stars?

  * 46%
<img width="1136" alt="Screen Shot 2022-06-22 at 10 27 54 AM" src="https://user-images.githubusercontent.com/99001393/175070562-de29b763-196a-4386-8170-a737d4352c35.png">

### Is there any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. 

Based on the data there is no positivity bias for paid vine reviews. That is evident based on the percentage of 5 star reviews per the divided groups (vine vs. nonvine).



Additional analysis that you could do with the dataset to support.

Additional analysis can be performed on 5-star reviews to obtain statistical distribution of each group(vine vs non-vine in jupyter notebook. 

