# BookRecommendation
Online book websites compete a lot over book sales and the number of users. A sound book recommendation system can attract users and sustain them. It is an important feature to have on your website. Our task is to develop a book recommendation system given users' data and ratings for specific books. 

The purpose of a book recommendation system is to predict buyers' interests and recommend books to them accordingly. A book recommendation system can take into account many parameters. I have used the collaborative filtering approach to develop my recommendation system. As a result, I developed two recommendation systems, one memory-based and one model-based. 

First, we do some EDA to understand the user demographics and rating distribution, followed by data cleaning(Null-value treatment) and feature engineering. The data is too big to develop a general recommendation system. So, we applied some minimum qualifying thresholds in the feature engineering step. This step also reduces the data size and addresses the cold start problem. 

I have applied two collaborative filtering approaches. First, I have used a memory-based collaborative filtering approach using k-nearest neighbours. 
Next, I used a model-based approach using singular value decomposition. I assumed some latent interactions between the users and items. I used this to recreate the user-item interaction matrix and ranked the ratings for recommendations. 

We choose to work with Top-N accuracy metrics, which evaluate the accuracy of the top recommendations provided to a user compared to the items the user has interacted with in the test set. The Top-N accuracy metric chosen was Recall@N which evaluates whether the interacted thing is among the top N items (hit) in the ranked list of 101 recommendations for a user. For example, the recall@5 for our recommendation system was 0.14, and recall@10 was 0.22.
