**A brief description of the purpose of the program and what it is doing.**

This program builds a movie recommendation system using a small sub-set extracted from the UCI’s IMDB data set to answer the question “Given a movies a dataset, what are the 5 most similar movies to a movie query?” by applying k-Nearest Neighbors algorithm in Python. The given sub-set contains a list of 30 movies and information about their IMDB rating, as well as the different genres they can be classified under. To answer the given question, when the kNN algorithm is applied on the data, similarity is based solely on the included genres and the IMDB ratings of the movies. Thus, even though the dataset includes “Movie ID” and “Label” columns, these columns are ignored (dropped) during the process of predicting the 5 similar movies. Additionally, since the movie that’s being used to predict – “The Post” – isn’t included in the given sub-set, a feature vector in form of a dictionary is created for the movie then this feature vector is used to look for the 5 similar movies.

**The Needed libraries, modules, and classes**
- The Pandas library is needed to load the CSV file from the URL into a DataFrame object. 
- The “NearestNeighbors” class from the “sklearn.neighbors” module in Python’s Scikit-learn library is also needed to find the k-nearest neighbors – the similar movies –  of a point from the dataset – “The Post”.

**How to install and run the code along with datasets to be able to run the program successfully.**

To be able to install and run the code successfully, the dataset must be read as a csv file into the notebook and all the needed libraries and modules need to be installed/imported. Each block of code must also be run individually and in a sequential order (one after another). 

**Acknowledgement**

The path used to access the data was provided by Prof. Arin Brahma (GitHub username: ArinB) using the link “https://raw.githubusercontent.com/ArinB/MSBA-CA-Data/main/CA05/movies_recommendation_data.csv”
