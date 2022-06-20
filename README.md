# Amazon_Vine_Analysis

## Overview
For this project we used ‘Amazon Review dataset’ and focused on ‘US Apparel product reviews’. The purpose was to analyze the validity of the Vine program to see if we should sell similar items via their platform. Vine Review program is an incentive based model that gifts customers free items so that they can review the product. We used PySpark to perform ETL based inspection and used an AWS RDS to connect to PostgreSQL. Their we finished the extracts and transformed the data via Pandas.

## Resources
  - Google Colab
  - Jupyter Notebook
  - AWS S3 and RDS 
  - PostgreSQL

## Roadmap
Step one was to extract the dataset from AWS via PySpark which we then transformed and loaded into AWS once again. Originally downloaded the file as a Jupyter notebook file but was modified in Google Colab so that we could so PySpark. The dataframe was then divided into four smaller dataframes for analysis. The dataframes were loaded into AWS RDS via PySpark then to PostgreSQL. The outputs were verified after being loaded in.
![customer_df]( https://github.com/gonzalesbarrett/Amazon_Vine_Analysis/blob/main/Images/Customers_df.png)
![products_df]( https://github.com/gonzalesbarrett/Amazon_Vine_Analysis/blob/main/Images/Products_df.png)
![reviews_df]( https://github.com/gonzalesbarrett/Amazon_Vine_Analysis/blob/main/Images/Review_df.png)
![vine_df]( https://github.com/gonzalesbarrett/Amazon_Vine_Analysis/blob/main/Images/Vine_df.png)


![product_verification]( https://github.com/gonzalesbarrett/Amazon_Vine_Analysis/blob/main/Images/Products_verification.png)
![reviews_verification]( https://github.com/gonzalesbarrett/Amazon_Vine_Analysis/blob/main/Images/Review_id_verification.png)
![customer_verification]( https://github.com/gonzalesbarrett/Amazon_Vine_Analysis/blob/main/Images/customer_verification.png)
![vine_verification]( https://github.com/gonzalesbarrett/Amazon_Vine_Analysis/blob/main/Images/Vine_verification.png)



The last table we utilized was the ‘vine_table’ so that we could filter reviews and compare the incentive based reviews (Vine) with reviews that were not apart of the Vine program. 

## Results
- Paid Vine Program
  - 33 total reviews
  - 15 5-star reviews
  - ***45.5%*** of vine reviews were 5-star

- Unpaid reviews
  - 45,388 total reviews
  - 23,733 5-star reviews
  - ***52.3%*** of unpaid reviews were 5-star


## Summary
The Vine program did not seem to have a positive return on investment, at least in the apparel category. The Vine program averaged a 45% five star review while reviews outside of the Vine program averaged a 52% five star review. One major caveat is that the number of reviews outside of the Vine program was 45,388 compared with 33 total Vine reviews. These numbers are difficult to compare due to the large variance between the two totals. It is unknown if the Vine reviews contributed to people trying the product but it seems unlikely due to the total number of products purchased outside of the program versus those from the Vine program. It would seem in this category incentivizing reviews did not have a significant impact on sales or desire. This would imply that Vine reviews do not hold a significant impact on customer sentiment.

![Screen Shot 2021-09-02 at 1 10 18 PM](https://user-images.githubusercontent.com/83378141/131887983-807ac118-b426-4db4-af18-209d85d2d80b.png)


