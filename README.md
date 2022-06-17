# Project 3 - Text Classification: Categorizing Music Genres



## Executive Summary


### Problem statement


    
Bassline, a small, up-and-coming company that handles social media management for musicians, receives an huge influx of fan posts and reviews for each client, largely focused in the genres of Metal and Hip Hop.  
Bassline is looking for a better way to categorize incoming reviews and fan posts by genre, in order to discover new and relevant trends and insights as they occur. They’re hoping to use what they discover to reshape their marketing strategy to better reflect their target audience.

   
   
   
### Description of data
    
#### Size (samples & features):



- hiphophead.csv (rows: 20700, features: 82)
- metal.csv (rows: 20700, features: 78)
- hiphop_metal.csv (rows: 41400, features: 81)



**All posts acquired from Reddit using PushShift API.**


##### Hiphopheads Post Pulls
https://www.reddit.com/r/hiphopheads/

    r/hiphopheads Posts Collected: 20700


##### Metal Post Pulls
https://www.reddit.com/r/Metal/

    r/Metal Posts Collected: 20700



 
##### Binary Classification Target:

- 'subreddit'




#### Model Evaluation:

- Baseline Model : 70% Accuracy


    
##### The Naive Bayes Classifier produced a better accuracy score.

- Naive Bayes () is the model chosen for production:

|Naive Bayes(BernoulliNB)|Model Performance|
|------|------|
|Accuracy Score: 1.0| This model predicted which category each post belonged to with 100% accuracy.|
|Precision Score: 1.0|Of the posts that the model predicted were accurately classed, 100% were true positives.|
|F1 Score: 1.0|Post that were actual positive were correctly predicted and post the were predicted were actual positive|


    
#### Primary Findings:

- Creating Youtube promotional content and sharing links could be an effective marketing strategy since most of the top 25 links are from Youtube.

- There is not much video content within either subreddit, so video marketing should focus more on using links to drive traffic to video content, preferably hosted on Youtube, rather than posting videos directly if advertising on subreddit or similar environment.
 
- 'FRESH' and 'Video' come up often within title posts of both classes.

##### Conclusions and Recommendations:

Naive Bayes was more effective at classifying the subreddit posts into their correct categories than the logistic regression models. It was able to accurately categorize subreddit posts with perfect accuracy on the test set, and satisfy the requirements for the company, Baseline, which allow them to focus on using the insight from the binary classification to gain insight that will propel their marketing strategy. The precision score is especially important to measure whether a post is a false positive, which could do more harm to Baseline's marketing campaigns, negatively affecting their business.

#### Next Steps

The model does exceptionally well on this particular dataset, but it is uncertain how well it would generalize on another dataset gathered from similar subreddits from the same genres.


##### Sources:

https://www.reddit.com/r/hiphopheads/



https://www.reddit.com/r/Metal/



https://github.com/pushshift/api

    

##### Credits for code:

https://scikit-learn.org/


https://www.statology.org/


