# BUILDING A MOVIE RECOMMENDATION SYSTEM

This is a self project done by me Chibuike Victor Akujuobi and reviewed by my friends Teyira Peter Geo-Needam & Emmanuel Ugochukwu. This project was done to enable us strengthen our skills in Python and Machine learning.

In this project, I will walk you through the basics of recommendation systems then build a movie recommendation system that calculates the pairwise cosine similarity scores for all movies based on their Cast, Tagline, Keywords, Directors, and Genres, then recommend movies with the highest similarity scores to the user’s input.

All steps taken are as follow:

1. Importing necessary libraries: I imported the necessary python libraries to be used in this project such as numpy & pandas which are very important for data analysis and manipulation. Then I imported TfidVectorizer and cosine_similarity and finally utilized the get_close_matches from the python module Difflib. A further explanation on all these are given in the ipynb file.

2. Data collection & Preprocessing: In this step I imported my data and did a little bit of data preprocessing to replace any rows having NaN values with a space/empty string, so it does not generate an error while running the code.

3. Feature Selection: I selected the features most relevant to this project, considering our problem at hand. Hence, the chosen features were keywords, cast, tagline, genres & director.

4. I combined relevant features into a single feature and converted it into a feature vector using the TfidVectorizer().

5. I calculated the similarity score on the feature vector using the cosine_similarity() function.

6. I created a list with all the movie names provided in the dataset.

7. I got the user's input "Movie Name".

8. Then I got the closest match to the user input from the list created in step 6 using the get_close_matches() function.

9. I got the index of the user's input i.e movie name.

10. I created a fuction called similarity_score that applied the cosine similarity on the index of the user input.

11. Then I sorted the similarity_score in a reverse way to get the highest first similarity score first.

12. Then used a loop fuction to print out 30 movies with high similar_scores.

I'd appreciate your feedback on this and of course there's always room for improvement in this recommedation system as each recommender system has its advantages and limitations. Definitely we can use more data from places like IMDB website to improve our models recommendation or use collaborative filtering method or hybrid models that uses content based and collaborative filtering methods together. A simple recommender provides general recommendations that might match the user’s taste. Collaborative filtering can provide accurate recommendations but it required a large amount of information about a user’s previous history and attitude. On the other hand, content-based filtering needs little information about the user’s history to provide a good recommendation, but it’s limited in scope as it always needs an item with pre-tagged characteristics to build its recommendations.
