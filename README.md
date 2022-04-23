# SC1015-MINI-PROJECT
Anime Analysis Mini-Project for SC1015 - Introduction to Data Science and Artificial Intelligence

# Welcome to the Anime-Analysis Repository

## About

This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on anime from [The Anime Recommendations Database] on Kaggle (https://www.kaggle.com/datasets/hernan4444/anime-recommendation-database-2020?select=watching_status.csv). 
  
## Contributors

- @NoelWee -  Data Extraction, Data Cleaning, Exploratory Data Analysis, K-Means Model, K-Modes Model and Overall Analysis
- @Tharun - Data Extraction, Data Cleaning, Exploratory Data Analysis, Linear Regression, Polynomic Regression and Overall Analysis

## Problem Definition

- Based on various factors, how likely is someone to complete an anime?
- Input Variables: High Score (Score > 8/10), Studios, Genres, Sources, Age Ratings
- Output: Completion Percentage

## Models Used

1. Linear Regression
2. Polynomic Regression
3. K-Means
4. K-Modes

The exploratory data analysis for each input variable and their subsequent evaluation using machine learning techniques are in the following notebooks. We chose to exclude Episodes and Score from our input variables selection due to their high amount of outliers. 

1. [EDA for Episodes](https://github.com/nicklimmm/movie-analysis/blob/main/data-extraction.ipynb)
2. [High Score Analysis](https://github.com/nicklimmm/movie-analysis/blob/main/data-visualization.ipynb)
3. [Studios Analysis](https://github.com/nicklimmm/movie-analysis/blob/main/data-resampling-and-splitting.ipynb)
4. [Genres Analysis](https://github.com/nicklimmm/movie-analysis/blob/main/logistic-regression.ipynb)
5. [Sources Analysis](https://github.com/nicklimmm/movie-analysis/blob/main/neural-network.ipynb)\
6. [Age Ratings Analysis]

## Conclusions

- Contrary to common beliefs, just because an anime has a high Score (Score > 8), it does not mean it has a high completion rate. Our findings have concluded that not only is Score a bad input variable to predict Completion Percentage, but there does not even exist a relationship (linear/non-linear) between the two.

- Among the hundreds of Studios clustered using our K-Means model, the top 5 Studios (in terms of no. of anime produced) belonging to the best cluster are J.C Staff, Madhouse, Production I.G, OLM and Nippon Animation. Their high median Completion Percentage also reflects current trends, as the 5 Studios have produced many popular and widely-known animes, both past and present. Examples include Pokemon (1997), Hunter X Hunter (1999), Toradora (2006), One-Punch Man (2015) and Haikyuu! (2020)

- The best genres we have gathered from our analysis are Comedy, Drama, Fantasy and Game, all generally popular amongst viewers. Comedy also has the highest anime frequency count among all 40 unique genres we managed to gather.

- The best Sources for anime to originate from are Light Novel, Game and Digital Manga.

- R-17+ (Violence & Profanity) is the best Age Rating when it comes to Completion Percentage. Unsurprising, given how many popular anime such as Attack on Titan, Tokyo Ghoul and the Fate Series all belong to that Rating. In addition, a large bulk of anime watchers range from teens to young adults and hence, are greatly drawn towards such anime with the given Rating.



## Key Takeaways

- Handling and understanding our dataset
- Cleaning up our Dataset and preparing it for analysis
- Application of Linear Regression from sklearn
- The new aforementioned models and how they operate (Polynomic Regression, K-Means, K-Modes)
- Usage of Label encoding in order for our models to evaluate categorical data
- Using techniques other than R^2 and confusion matrix to evaluate the accuracy of our models, especially since K-Means and K-Modes are unsupervised (Elbow Test, Silhouette Analysis)
- Separation of individual clusters and evaluating the each cluster's statistics
- Drawing conclusions from our findings


## References

- Kaggle. Anime Recommendations Dataset
https://www.kaggle.com/datasets/hernan4444/anime-recommendation-database-2020?select=watching_status.csv [Accessed on 12 March]


- Imad Dabbura. K-means Clustering: Algorithm, Applications, Evaluation Methods, and Drawbacks https://towardsdatascience.com/k-means-clustering-algorithm-applications-evaluation-methods-and-drawbacks-aa03e644b48a [Accessed on 10 April]
