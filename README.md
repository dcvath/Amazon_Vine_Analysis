# Amazon Vine Analysis

## Overview of Analysis

### Purpose
The purpose of this analysis was to analyze Amazon video game reviews written by members of the paid Amazon Vine program and those written by non-paid Amazon members to determine if there's any bias for the paid review. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products; in this case, video games. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. I conducted this analysis for Jennifer at SellBy to submit to SellBy stakeholders. 

### Description of Project
In this project, I analyzed the Amazon video games dataset. I used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I used PySpark to determine if there was any bias toward favorable reviews from Vine members in the video game dataset. Then, I wrote a summary of the analysis, which is the document you are currently reviewing.

## Results
Using bulleted lists and images of DataFrames as support, address the following questions:

- How many Vine reviews and non-Vine reviews were there?


- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars? 


- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

## Summary
In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.
