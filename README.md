# Amazon Vine Analysis

## Overview of Analysis

### Purpose
The purpose of this analysis was to analyze Amazon video game reviews written by members of the paid Amazon Vine program and those written by non-paid Amazon members to determine if there's any bias for the paid review. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products; in this case, video games. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. I conducted this analysis for Jennifer at SellBy to submit to SellBy stakeholders. 

### Description of Project
In this project, I analyzed the Amazon video games dataset. I used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I used PySpark to determine if there was any bias toward favorable reviews from Vine members in the video game dataset. Then, I wrote a summary of the analysis, which is the document you are currently reviewing.

## Results
Below, please find the results of the analysis:

- How many Vine reviews and non-Vine reviews were there?
There was a total of 94 PAID Vine reviews and a total of 40,471 non-Vine/non-paid reviews.

<img width="471" alt="Paid_Nonpaid_Reviews" src="https://user-images.githubusercontent.com/85654649/138193818-e3803345-18fe-4d4d-85c2-5519ad974d68.png">

- How many Vine reviews were 5 stars? 
There was a total of 48 PAID Vine 5-star reviews.
<img width="806" alt="5star_paid_reviews" src="https://user-images.githubusercontent.com/85654649/138193949-9769cf6d-0d88-4d16-af2c-4fe4e43c1df8.png">

- How many non-Vine reviews were 5 stars? 
There was a total of 15,663 non-Vine/non-paid 5-star reviews.
<img width="789" alt="5star_nonpaid_reviews" src="https://user-images.githubusercontent.com/85654649/138194084-4bdcacce-8597-40cb-ad2a-7c04123e7ed5.png">

- What percentage of Vine reviews were 5 stars?
51.06% of the Vine paid reviews were 5 stars.
<img width="736" alt="5star_paid_reviews_percent" src="https://user-images.githubusercontent.com/85654649/138194866-540e8c85-f681-44f4-899c-a360d4fe87c8.png">

- What percentage of non-Vine reviews were 5 stars?
38.70% of the non-Vine/non-paid reviews were 5 stars.
<img width="757" alt="5star_nonpaid_reviews_percent" src="https://user-images.githubusercontent.com/85654649/138195021-4dea06f9-f8c6-4657-ae43-7edc82d70a3d.png">


## Summary
Based on the analysis, it's clear that there is a positivity bias with the Vine PAID reviews, when compared to the non-Vine/unpaid reviews. As indicated above, 51.06% of the Vine PAID reviews were 5 stars, compared to the non-Vine/non-paid 5 star reviews, which were only 38.70%, which is a different of 12.36%. In addition, there was a larger sample size of non-Vine/non-paid reviews of 40,471, compared to the Vine PAID reviews of only 94. A larger sample size is typically indicative of a more accurate sampling. I would recommend SellBy conduct one additional analysis by adding in verified purchases to the analysis to determine if this impacts the positivity bias as there could be positive reviews added in the non-Vine program; however, the purchases may not have been made and those could have been added by a competitor.
