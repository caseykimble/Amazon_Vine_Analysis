# Amazon Vine Analysis

### Overview of Analysis

  The purpose of this study was to analyze Amazon product reviews and determine if a bias existed amongst paid reviewers from the Amazon Vine review program, which is a program that allows companies to provide products to customers in exchange for a review, essentially a paid incentive to leave a review. I performed an ETL process to extract, transform and load the transformed data into pgAdmin. I then used PySpark to further analyze the data and determine the number of paid vs. unpaid 5-star reviews based on a dataset for reviews of camera products. 

### Results

I began by filtering the reviews to show only those that had at least 20 votes, to find reviews that were more likely to be helpful and avoid division by zero errors while transforming the data. 

<img width="1090" alt="Screen Shot 2022-12-08 at 8 51 00 PM" src="https://user-images.githubusercontent.com/105175961/206621907-6dac9f0d-d929-44b4-a837-06e21dd1cf5d.png">

* As seen in the images below, it appears that although the Amazon Vine review program is a popular program, it is still a small minority of reviews overall, with 607 Vine (paid) reviews vs. 50,522 unpaid reviews. This puts the overall percentage of paid reviews vs. total reviews at barely over 1%.


<img width="581" alt="Screen Shot 2022-12-08 at 8 49 44 PM" src="https://user-images.githubusercontent.com/105175961/206621067-639053bd-37e8-467e-a552-d10c16754d93.png"><img width="622" alt="Screen Shot 2022-12-08 at 8 50 11 PM" src="https://user-images.githubusercontent.com/105175961/206621084-f23053d9-9f69-4db8-902d-c68cfbe75771.png">

* The number of 5-star reviews from customers of the Amazon Vine program (in other words, paid reviews) was 257 out of 607 reviews, for a percentage of  was 42.3%. The number of 5-star reviews from average, unpaid Amazon customers was 25,220 out of 50,522 total reviews, for a percentage of 49.9%. This shows us that standard Amazon customers are just slightly more likely to leave a 5-star review than Amazon Vine customers. 

### Summary 

From my analysis of camera reviews left on Amazon, there does not appear to be any kind of bias in the reviews of paid reviewers who may have received incentive in the form of free product in exchange for a review. In fact, customers that were not incentivized in any way to leave a review were slightly more likely to leave a 5-star review, with 49.9% of unpaid customers leaving 5-star reviews, vs. only 42.3% of paid customers leaving 5-star reviews.


Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement. For further analysis, it may be helpful to look into all reviews (regardless of star rating) for paid vs. unpaid customers, instead of just 5-star reviews, or to potentially look at all reviews regardless of star rating or number of total votes on those reviews, as newer reviews may be just as helpful but not have many votes on them yet. 
