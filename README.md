# Movie_Recommender_System

## Description: ##
Recommender System is a Deep Learning Application which is being widely used by the big MNC's to increase the revenue and improve user experience. They recommend products, show advertisements, and provide suggestions based on different factors like user's purchasing history, preferences and other relevant information. In this project a basic Movie Recommendation System is built which takes user and movie as its input and rating as it output. 

## Dataset ## 
[Dataset Link](https://grouplens.org/datasets/movielens/)
'ratings.csv' file is extracted from the Dataset Link. The data used in this project is in the form of a triplet (user, movie, rating). There are a total of 25000095 records. 80% of the data is used for training and the rest is used for testing.

## Concept ##
Usually the Movie and User features are categorical in nature and then we use the concept of Embedding layer to convert them into feature vectors. The Embedding layer maps each category into a dense vector in lower dimension where each dimension represents a learned feature or attribute associated with the category (they capture semantic and relationship). Embedding layer concept is generally used when we want to incorporate categorical data into our neural network. In this project, the userId and movieId are in the numerical format but feeding them directly into the neural network can imply ordinal relationship and hence neural networks might fail to understand the pattern. Using embedding layer allows our neural network to learn intricate patterns and user-movie relationship. 

## Implementation ##
The concept of embedding layer and feeding parallel input using Tensorflow with Keras API has been used in this project. First userId and movieId is converted into the embedding feature vectors. Both these features vectors are then concatenated and fed as input to the neural network and rating is passed as the output. The model's performance is checked by plotting the training and validation loss.
