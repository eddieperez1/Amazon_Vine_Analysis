# Amazon_Vine_Analysis

The folowing dataset was analyzed for Vine and non-vine 5 star reviews from watches sold on amazon. [Link to Amazon datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt) and [Link to Watches Dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Watches_v1_00.tsv.gz)

## Overview of the analysis

The goal of this analysis is to analyze Amazon reviews written by members of the paid Amazon Vine program. First, ETL is performed on the data using pyspark and Amazon Web Services(AWS) to load the data into Postgres pgAdmin and then analyze the vine table to compare Vine vs non-Vine reviews. The ETL can be found in [Amazon_Reviews_ETL.ipynb](/Amazon_Reviews_ETL.ipynb) using google colab.

### Installation and Services Used in this Project
- postgre pgAdmin
- AWS account
- Google Colab 

## Results

Vine reviews are paid and non-Vine reviews are non-paid.
![Results of Paid vs Unpaid](/screenshots/Results%20of%20paid%20vs%20unpaid.PNG)

### Summary of Results
- 47 Vine reviews and  8362 non-Vine reviews
- 15 Vine reviews were 5 stars and 4332 non-Vine reviews were 5 stars
- 31.91% of Vine reviews were 5 stars and 51.81% of non-Vine reviews were 5 stars


## Summary

There is no positivity bias for reviews in the Vine program since the percentage of Vine 5 star reviews is lower than non-Vine 5 star reviews. An additional analysis that can be performed is find if there is positivity bias for reviews in verified purchasers. 