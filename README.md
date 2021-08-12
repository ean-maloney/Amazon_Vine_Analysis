# Amazon Vine Analysis

## Overview 
In this analysis I look at US Amazon reviews in the Sports category and compare the distributions of reviews between users participating in the Vine program and those not. As Amazon explains on their website: 

>"Amazon Vine invites the most trusted reviewers on Amazon to post opinions about new and pre-release >items to help their fellow customers make informed purchase decisions. Amazon invites customers to >become Vine Voices based on their reviewer rank, which is a reflection of the quality and >helpfulness of their reviews as judged by other Amazon customers. Amazon provides Vine members with >free products that have been submitted to the program by participating vendors."

The goal of this analysis is to determine whether those in the Vine program give a significantly different number of 5-star reviews than normal customers.

## Results
I separated my initial dataset of all reviews into two dataframes, one for those in the Vine program and one for other Amazon users.

These dataframes were filtered to include only those reviews with 20 or more votes and 50% or more helpful votes from other Amazon users.

The distribution for non-Vine members was as follows, with 61,948 reviews total:

![image](https://user-images.githubusercontent.com/80861610/129233920-b712ff27-f4a3-4fc5-b3fc-6480c1dce35d.png)

And for Vine members, with 334 total reviews:

![image](https://user-images.githubusercontent.com/80861610/129233783-f1b733f0-7913-4e81-bc12-2cc2588c4cfb.png)

The non-Vine members gave 5 stars in ~53% of their reviews, while the Vine members gave 5 stars in ~42% of their reviews.

## Summary
From the results it seems that there is not a bias towards giving 5 star reviews for the Vine program members. In fact they give products a 5 star review less frequently than normal Amazon users (42% v. 53% of the time). 

Additionally, the median rating gives by Vine members was 4 stars, whereas for non-Vine users it was 5 stars. The mean rating was however slightly higher for Vine members. I attribute this to Vine members being less prone to giving extreme (1 or 5-star ratings).
