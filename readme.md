# Project Overview (Recommendations with IBM)  
In this project, we analyzed the interactions that users have with articles on the IBM Watson Studio platform, and make recommendations to them about new articles  they might like.

## Backgound
  IBM Watson Studio is a share platform for data science. The communnity members can access DS related articles, tutorials, dataset, etc. It's amazing idea to have a recommendation board available in the dashboard that shows the articles that are most pertinent to a specific user. We performed a study of the data available on the IBM Watson Studio platform to determine which articles to show to each user.

## Dataset
  * articles_community.csv
  * user-item-interactions.csv

## Components
  (The whole work is save in 'Recommendations_with_IBM.ipynb'.)

  * Basic Exploratory Data Analysis

  * Rank Based Recommendations (for new users)

  To get started in building recommendations, we find the most popular articles simply based on the most interactions. (Since there are no ratings for any of the articles, it is easy to assume the articles with the most interactions are the most popular and we might recommend to new users).

  * User-User Based Collaborative Filtering (Personal Recommendation)

  In order to build better recommendations for the users of IBM's platform, we looked at users that are similar in terms of the items they have interacted with. These items could then be recommended to the similar users. 

  * Content Based Recommendations

  Given the amount of content available for each article, there are a number of different ways in which someone might choose to implement a content based recommendations system. We planed to try some NLP methods to training the models and to develop a content based recommendation system, unfortunately we haven't done yet since the time limitation.

  * Matrix Factorization

  Finally, we completed a machine learning approach to building recommendations. Using the user-item interactions, we built out a matrix decomposition. Using  decomposition, we get an idea of how well we can predict new articles an individual might interact with.
