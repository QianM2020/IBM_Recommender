Recommendations with IBM

# Introduction
  For this project I analyzed the interactions that users have with articles on the IBM Watson Studio platform, and make recommendations to them about new articles I think they will like.

  You can create your own account to become a part of IBM Watson Studio platform, and get a better understanding of their data by creating an account on the platform here.
  IBM Watson Studio platform, you could imagine having a recommendation board available here that shows the articles that are most pertinent to a specific user.


# Components
  The project will be divided into the following tasks
  (The whole work is save in 'Recommendations_with_IBM.ipynb'.)

  I. Exploratory Data Analysis
      The datasets are saved in:
        articles_community.csv
        user-item-interactions.csv

  II. Rank Based Recommendations

  To get started in building recommendations, first I find the most popular articles simply based on the most interactions. Since there are no ratings for any of the articles, it is easy to assume the articles with the most interactions are the most popular. These are then the articles we might recommend to new users (or anyone depending on what we know about them).

  III. User-User Based Collaborative Filtering

  In order to build better recommendations for the users of IBM's platform, we could look at users that are similar in terms of the items they have interacted with. These items could then be recommended to the similar users. This would be a step in the right direction towards more personal recommendations for the users. You will implement this next.

  IV. Content Based Recommendations (NOT completed)

  Given the amount of content available for each article, there are a number of different ways in which someone might choose to implement a content based recommendations system. I planed to try some NLP methods to training the models and to develop a content based recommendation system, but haven't done yet.

  V. Matrix Factorization

  Finally, I completed a machine learning approach to building recommendations. Using the user-item interactions, I built out a matrix decomposition. Using  decomposition, we get an idea of how well we can predict new articles an individual might interact with (spoiler alert - it isn't great). I also discuss which methods might be used to move forward, and how to test how well the recommendations are working for engaging users.
