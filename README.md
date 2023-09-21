# 100-days-of-data-science
## Motivation:
* Trying to get gud at machine learning, bc it's the future and it's cool
* I tend to get analysis-paralysis when it comes to choosing a project to work on
* With this challenge, I'll give myself space to work on small/toy projects to start and will organically grow to work on bigger challenges

## Goal
* Get hands-on practice with exploratory data analysis, training, and evaluation
* Apply the things I've learned in AI, ML, Deep Learning, Computer Vision, and AI System Design
* At the end, I want to be able to take on the [Google Contrails competition](https://www.kaggle.com/competitions/google-research-identify-contrails-reduce-global-warming)

## Log
### Day 13: 09/20/2023
* Learned how to use linear regression with time series
* Created features like time step and lag
* Also learning some basic plots with seaborn rather than just matplotlib

### Day 12: 09/19/2023
* Finished Spaceship titanic with final score 0.78232. Probably could have: used cross validation.
* Want to learn how to add features from within a pipeline. I think I was close but was having some issues in the end
* I think if I use a base thingy and implement fit and transform properly, then I can use them in a step in my pipeline.
* Tried using FunctionalTransformer to no avail
* Time for real dataset?

### Day 11: 09/18/2023
* Did around 30 min EDA and feature engineering on the Spaceship Titanic dataset on Kaggle

### Day 10: 09/17/2023
* Started SpaceTitanic dataset
* Want to do the Data Visualization course on Kaggle. Getting stuck googling how to use matplotlib properly to visualize the data

### Day 9: 09/16/2023
* Added pipeline for rfc on titanic dataset
* Added cabin letter feature from cabin

### Day 8: 09/15/2023
* Started applying what I learned this week to the titanic ML dataset. Think I just want to get a pipeline working with XGBoost, with added features, then move onto a new dataset

### Day 7: 09/14/2023
* Learned about data leakage and finished Kaggle's Intermediate ML tutorial. Pretty hard to identify!

### Day 6: 09/13/2023
* Learned about XGBoost through Kaggle's Intermediate ML tutorial. I guess for XGBoost we don't make the trees separately and have them learn from previous trees instead

### Day 5: 09/12/2023
* Learned how to pre-process categorical data using ordinal encoding and one-hot encoding
* Learned how to create pipelines to combine preprocessing and prediction/inference in the same step. So much cleaner!
* Learned how to use cross-validation. Should take a look at grid search at some point

### Day 4: 09/11/2023
* Started the intermediate machine learning Kaggle course
* Learned how to handle missing values with several methods (dropping, imputation, imputation with labeling)

### Day 3: 09/10/2023
* Started the Kaggle titanic dataset
* Did a lot more EDA and feature engineering -- some `NaN` values, features that may have caused memorization, some features that needed parsing
* Making a random forest gets an accuracy score of 0.825. Not too bad for first attempt?
* Tmrw going to pause from doing challenges and do those tutorials I listed yesterday. And then after that will try a NN or other classifier.

### Day 2: 09/09/23
* Making CNN to classify MNIST digit dataset
* Learning how to create datasets and dataloaders
* How loss & optimizer & a net relate must be through the net parameters, but it's not entirely clear how
* Not sure how CNN dimensions work
* I think it's bc there's no channels in the MNIST dataset. (This ended up being the problem, needed to add a dimension for a single channel. But I should brush up on the dimensionality of CNNs anyways)
* Watched StatQuest on CNNs https://youtu.be/HGwBXDKFk9I?si=7FruRffmcSn9G1b9
* Made my first Kaggle competiton submission. Ik these are toy problems but I'm learning things :)
* May try using some sort of ensemble for my next competition
* Things to do for tmrw: [Feature Engineering](https://www.kaggle.com/learn/feature-engineering) and [Data Visualization](https://www.kaggle.com/learn/data-visualization) and [Data Cleaning](https://www.kaggle.com/learn/data-cleaning) for EDA.

### Day 1: 09/08/23
* Decided to start working my way through Kaggle's Getting Started challenges.
* Working on the classic MNIST dataset. I must've done this before, but am doing it without following any tutorial this time and am learning a lot more along the way (not just hitting run on cells).
* Tried with some sklearn classification algorithms (svm.SVC, trees.DecisionTreeClassifier, neighbors.KNearestNeighborsClassifier), mostly with default settings and they performed well
* SVM seems to perform the best but is also the slowest
* Evaluation is hard bc have to choose the right metrics
* Here's the repo where I'll keep track of those notebooks: https://github.com/alexcjwei/getting-started-kaggle
* Tmrw: try CNN then move on

### Day 0: 09/07/23
* Read Andrew Ng's ["How to Build Your Career in AI" eBook](https://info.deeplearning.ai/how-to-build-a-career-in-ai-book#MYL-form)
* Need to remember my career is long -- all I have to do is start now and do a little every day

