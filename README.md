# Recommendation system for IBM

## Motivation

In this project, I built recoomendation system based on real data from the IBM Watson Studio platform. 


## Conclusion

We used Matrix Factorization with SVD to predict whether users will interact with articles and achieved the accuracy of 0.979 on a test data set with 10 latent features.

Unfortunately, we could not make predictions for most of the users in a test data set because of cold start problem. In fact, we could only make predictions for 20 users (2.93% of all users in a test dataset). When we run into cold start problem, we should implement content based and ranked based recommendations.

For users that have interacted with a few articles, a combination of rank-based recommendations, User-User Based Collaborative Filtering and Content Based Recommendations can be used.

The main drawback of the recommendations systems implemented above is that the findings are observational ('off-line'). To truly validate our assumptions, we need to run A/B test and divide the audience into groups where one of the groups should be a control group. This will help us determine the best approach and choose the best recommendation method or a combination of methods.

