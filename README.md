# Product-Recommendation-System
A recommendation system that predicts top items for customers based on ratings 

## Dataset 
The dataset consists of Style Shuffle ratings from users on items. Users rate items in (multiple)
quizzes of 10 questions each. A quiz can either contain random questions, or “personalized
questions”. In the latter, the items shown in the quiz are chosen because we think the user will
like them, rather than selected at random from all available questions.

#### Columns

● User_id: identifies the user

● Quiz_type: “random” or “personalized”

● Quiz_number: indicates the sequence number of the quiz shown to a user. Thus, quiz_number = 1 indicates that this question is part of the first quiz the user rated.

● Question_number: indicates the sequence number of the question shown to a user across all quizzes the user has rated. Thus, this is an increasing sequence for each user.

● Item_id: identifies the item rated

● Rating: 1 indicates a like, 0 indicates a dislike

## Building a Recommendation System
1. Collaborative Filtering using k-Nearest Neighbours (kNN) to find clusters of users based on common item ratings. In other words, it uses historical item ratings of like-minded people to predict how someone would like/dislike an item. Method: Memory-Based Collaborative Filtering using Cosine and Pearson similarity metrics Used three variations of basic KNN models – KNNBasic, KNNwithMeans, KNNBaseline

2. Collaborative filtering using Matrix Factorization Method: Model-Based Collaborative Filtering using Singular Value Decomposition (SVD). Here, GridSearchCV method has been used for hyperparameter tuning

#### Performance Metric
Root Mean Square Error (RMSE)
