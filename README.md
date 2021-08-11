# Amazon_Vine_Analysis

## Purpose 

The purpose of this analysis was to determine whether there is any bias toward favorable reviews written by Amazon Vine members vs. reviews written by those not part of Amazon's paid review program. Specifically, a dataset of 50,000 reviews related to Amazon purchases of lawn and garden goods was analyzed utilizing pySpark DataFrames and Python, working in Google Colab notebooks. To aid in the analysis, the raw data was filtered to pull out data where the product had a minimum of 20 votes, and of those at least 50% were helpful votes. We then broke this filtered data set into reviews written by Vine members, and those that were not. Finally, for each of these subsets we determined the total number of reviews, the number of 5 star reviews, and the percentage of 5 star reviews from the individual group total.

## Results 

![challenge16](https://user-images.githubusercontent.com/81761879/128968069-cfbedb7f-a37c-4c34-9863-545cf7e74059.PNG)
### Figure A. 

As shown in the table above, we can see that for reviews written by Vine members...
* there were 386 total reviews 
* of those, 176 reviews were 5 stars
* or about 45.6% of the groups total reviews
* 
For reviews written by non-Vine members...
* there were 48,717 total reviews
* of those, 24,026 reviews were 5 stars 
* or about 49.32% of the groups total reviews

## Analysis

From this analysis, it does not appear that there is any positivity bias for reviews written by Vine members. Indeed, non-Vine members actually had a higher percentage of 5 star reviews ( 49.32% vs 45.6%). It would seem Vine members are as critical if not more so in their reviews of products bought through Amazon vs non-Vine members. However, to further confirm this, it would be beneficial to further analyze the data by looking at reviews that were 4 stars or greater, and consider these as positive reviews, versus only looking at 5 star reviews. This would be a more realistic measure, and increase the sensitivity of picking up any favorability bias between the two groups. 
