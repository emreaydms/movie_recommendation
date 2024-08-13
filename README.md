# Movie Recommendation System

To start with recommendation systems, i made a movie recommendator which have:

## 1. Simple Recommender

A popularity-based recommender provides generic suggestions to all users by prioritizing movies with high ratings and popularity (often incorporating genre). The underlying assumption is that widely acclaimed and popular films have a broader appeal. This approach does not tailor recommendations to individual preferences.
Implementation is straightforward: movies are ranked by rating and viewership, and the top-rated or most popular titles (potentially filtered by genre) are presented as recommendations.

## 2. Content Based Recommender
The recommender we built in the previous section has significant limitations. It offers generic recommendations to all users, disregarding individual preferences. For example, a person who enjoys romantic movies but dislikes action films would find little value in our Top 15 chart, even when filtered by genre.

Consider a user who adores "Dilwale Dulhania Le Jayenge," "My Name is Khan," and "Kabhi Khushi Kabhi Gham." It's reasonable to infer their preference for Shah Rukh Khan and Karan Johar's work. Yet, even a romance-specific chart might not accurately reflect their taste.

To enhance personalization, we'll develop a content-based filtering engine that calculates movie similarity based on specific metrics. This approach suggests movies similar to those a user has liked. We'll create two such recommenders using:

* Movie overviews and taglines
* Movie cast, crew, keywords, and genre

Due to computational constraints, we'll work with a subset of the available movie data.

## 3. Metadata Based Reccommender

## 4. Collaborative Filtering

Our content-based recommendation engine has some significant limitations. It can only suggest movies similar to a specific movie, making it ineffective at capturing diverse tastes and providing recommendations across various genres. Additionally, the engine is not personalized; it does not consider individual user preferences and biases. As a result, anyone querying our engine for recommendations based on a particular movie will receive the same suggestions, regardless of their unique tastes.

To address these shortcomings, we will implement a technique called Collaborative Filtering to enhance our recommendation system. Collaborative Filtering leverages the preferences and behaviors of similar users to predict how much a particular user will enjoy a product or service they have not yet experienced. By analyzing patterns in user interactions, this method allows us to make personalized recommendations that better reflect individual tastes and preferences.

## 5. Hybrid Recommander

And finally, i tried to bring together techniques we have implemented in the content based and collaborative filter based engines

* Input: User ID and the Title of a Movie
* Output: Similar movies sorted on the basis of expected ratings by that particular user.

## 6. Dataset

I used https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset/data as dataset.
