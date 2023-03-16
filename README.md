# Movie Recommendation Model

# Overview
This end of phase 4 project for the Flatiron Online Data Science Course aims to develop a recommendation model capable of suggesting five movies to a user that they are highly likely to rate positively. The main objective is to provide an exceptional user experience by utilizing advanced data science techniques to tailor recommendations that match the user's preferences.

In addition to creating a recommendation model, I conducted an investigation to determine the best approach for enhancing the content of our libraries.  This will not only give our users more movies to watch, but with their feedback we will be able to improve the recommendations that our model can make.

# Business Problem
The task at hand is to build a recommendation model, to enable our streaming service (FlixGenius) to recommend movies to a user that they may rate highly.
As a secondary task FlixGenius wants to add more movies to the streaming library and have asked for some recommendations on what to add.

# Data 
The data is the MovieLens dataset from the GroupLens research lab at the University of Minnesota


# Results

### The Most and Least Common Genres in MovieLens library

Here we compare the amount of movies for each genre.  I was looking for insight into what is most popular and what is least popular.  From this graph the question that I asked myself is why there was such a big difference in the number of movies in the less common genres to the genres with more movies.   

![Alt text](http://localhost:8889/view/Untitled%20Folder/Ratings%20per%20Genre.png)

### Which Genres Dominate the Ratings

![Alt text](http://localhost:8889/view/Untitled%20Folder/Ratings%20per%20Genre.png)

With this graph my aim was to explore how popular genres were,  I was hoping to find insight that would show if genres with less representation were still being watched.  I found that the amount of ratins resembled the number of movies in the genre.

### How Ratings Vary Across Different Genres

![Alt text](http://localhost:8889/view/Untitled%20Folder/avg%20rating.png)

When ploting this bar graph, I was looking for any data that would give me insight into what genre do people like the most?  I found that there is not much of a difference.  All average ratings for a genre were between 3.5 and 4.  This told me that all the genres were popular, and that the lower genres were just under represented.

### Understanding the Variability of Ratings by Genre

![Alt text](http://localhost:8889/view/Untitled%20Folder/Genre%20Rating%20Distribution.png)

While creating the box and whisker plot, my attention was focused on examining the genres that were not well-represented in our movie library. By analyzing the distribution of ratings for these less-represented movies, I gained insightful information. I found that these genres are not disliked by the audience, as their rating distribution was similar to that of the more popular genres. Moreover, I observed that in some cases, these less-represented genres received higher average ratings, despite having lower ratings counts. In simpler terms, these genres received fewer negative ratings than other genres, and even though fewer people rated or watched them, those who did gave them higher ratings on average.

# Final Model Overview

After running 3 different types of models (collaborative based filtering, content based filtering, and a hybrid approach) I found the baseline collaborative model to have the best performance with an RMSE of 1.9.  While not great, it was much better then both other models which had RMSEs of 2.8.

![Alt text](http://localhost:8889/view/Untitled%20Folder/collab%20model%20metrics.png)
