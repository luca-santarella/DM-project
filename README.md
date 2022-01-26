# DM-project
## Data Mining project A.Y. 2021/2022

The project consists in data analysis based on the use of data mining tools assigned by the prof. Anna Monreale for the Data Mining course.
## DATASET DESCRIPTION
The dataset to be analyzed is composed of information about some tennis matches. Data
are organized in .csv file:
* tennis_matches.csv where each row represents a match
* male_players.csv
* female_players.csv<br>

### Task 1: Data Understanding and Preparation
Task 1.1: Data Understanding: Explore the dataset with the analytical tools studied
and write a concise “data understanding” report assessing data quality, the
distribution of the variables and the pairwise correlations.
Task 1.2: Data Preparation: Improve the quality of your data and prepare it by
extracting new features interesting for describing the player profile and his behavior
derivable from matches. These indicators have to be extracted for each player.
Subtasks of DU
* Data semantics for each feature that is not described above and the new one
defined by the team
* Distribution of the variables and statistics
* Assessing data quality (missing values, outliers, duplicated records, errors)
* Variables transformations
* Pairwise correlations and eventual elimination of redundant variables

### Task 2: Clustering analysis
Based on the player’s profiles explore the dataset using various clustering techniques.
Carefully describe your decisions for each algorithm and which are the advantages provided
by the different approaches.
Subtasks
* Clustering Analysis by K-means:
1. Identification of the best value of k
2. Characterization of the obtained clusters by using both analysis of the
k centroids and comparison of the distribution of variables within the
clusters and that in the whole dataset
3. Evaluation of the clustering results
* Analysis by density-based clustering:
1. Study of the clustering parameters
2. Characterization and interpretation of the obtained clusters
* Analysis by hierarchical clustering
1. Compare different clustering results got by using different merging
strategies
2. Show and discuss different dendrograms using the different merging
strategies
* Final evaluation of the best clustering approach and comparison of the clustering
obtained
Explore the opportunity to use alternative clustering techniques
in the library: https://github.com/annoviko/pyclustering/

### Task 3: Predictive Analysis
Consider the problem of predicting for each player a label that defines if s(he) is a high
ranked player or a low ranked player (binary task) by exploiting the feature related to the
rank of the players.
The student need to:
1. Define a player profile that enables the above player classification. For this task, you
can exploit the profile created for the clustering task, by adding or removing features,
depending on the results previously obtained.
2. Compute the label for any customer. The extraction of the label can take advantage
of several features related to the rank, such as loser_rank, winner_rank,
loser_rank_points, winner_rank_points, etc. An example of simple label can be
derived by:
* computing the average rank per player by exploiting loser_rank, winner_rank
* select a threshold for discretizing in two categorical labels the class.
Note that you can define in different ways the labels.
3. Perform the predictive analysis comparing the performance of different models,
discussing the results and discussing the possible preprocessing that you applied to
the data for managing possible problems identified that can make the prediction hard.
Note that the evaluation should be performed on both training and test set.

### Task 4.1: Time Series Analysis

Consider the dataset of time series CityGlobalTemperature2000-2009.csv containing for 100
cities the temperature measurements (mean and standard deviation over a month). The goal
of the task is to find groups of similar cities with respect to the temperature trends.