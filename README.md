# Amazon_Vine_Analysis

## Overview
Companies using Amazon can pay to have reviewers review their product through the Amazon Vine program. We have been asked to conduct an analysis to determine whether or not these reviewers are more likely to give 5-star reviews than non-paid reviewers. We chose to conduct our analysis using the Outdoor-goods dataset: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Outdoors_v1_00.tsv.gz.

## Results
- There are 103 Vine Reviews and 37372 non-Vine Reviews in the dataset (after filtering on reviews wiht 20+ votes and 50% helpful rating)

The Vine reviews DataFrame:

![]()

The non-Vine reviews DataFrame:

![]()

- There were 55 Vine Reviews that were 5-stars and 19723 non-Vine Reviews that were 5-stars.

- 53.40% of Vine Reviewers gave 5-stars compared to 52.77% of non-Vine Reviewers.

The full analysis from the Vine and non-Vine DataFrames can be seen here:

![]()



## Summary

There does not appear to be any bias from Vine Reviewers when it comes to giving a 5-star review. 53.40% and 52.77% are remarkably close, especially when there were only 103 Vine-Reviewers in the dataset.

A Chi-Squared test could be (and was) performed to determine whether or not there was any bias. For the analysis, reviews were categorized into 5-star, and not 5-star. Vine Reviewers and non-Vine Reviewers. p-value was 0.98, indicating that there is no difference in categorical frequency between groups.

![]()