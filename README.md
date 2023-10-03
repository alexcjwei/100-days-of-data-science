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
### Day 25: 10/02/2023
* Increased the UNet encoder depth, and segmentation improved. We looked to be overfitting on the single example.
* However, I'm not sure why the DICE score was staying around 0.9. Need to look into that.

### Day 24: 10/01/2023
* Trained the model on a single data point to see if it would overfit
* The model did train a bit and was able to correctly classify some segmentation, but not all of it
* Wrote up some hypotheses as to why my model may be training but not overfitting and will look into them in the future (model complexity, bad initialization, learning rate).

### Day 23: 09/30/2023
* Verified the losses of the initial Unet I'd set up.
* Loss was 0 for examples without ground-truth masks, 0.9293 for examples with ground-truth masks.
* Want to visualize the outputs we're getting from the model next.

### Day 22: 09/29/2023
* Separated transformations out of training loop into dataset
* CUDA running out of memory when running! What do I do now...

### Day 21: 09/28/2023
* Set up Unet from `segmentation_models.pytorch` to train single epoch! 

### Day 20: 09/27/2023
* Visualized data from the Dataset to make sure I was loading data properly
* Turns out Python Enums start at 1 by default! Was debugging my plots for a while.

### Day 19: 09/26/2023
* Continued EDA on contrails dataset, consolidating my functions for visualizing code and looking at examples from train/validation set.
* Created a Pytorch Dataset and Dataloader to load my datasets! This was pretty great as I'd gotten stuck on this step of the process before. However, since my understanding of the data was better, this went smoothly and I could set it up by myself.

### Day 18: 09/25/2023
* Started some EDA on the contrails dataset. Converted the satellite data to RGB color scheme for visualization, and overlayed the masks.
* Created animation to watch the contrail sequence.

### Day 17: 09/24/2023
* Learned about trends and seasonality when working with time series.
* Want to pick a project that will help me grow technically (challenging enough to stretch skills but not so hard I won't succeed), and be a stepping stone to larger projects.

### Day 16: 09/23/2023
* Just made a pipeline to predict the health outcome of a horse. I am more confident in using the same preprocessing techniques (simple imputer, onehot) and the main classificatio algorithms on sklearn (random forest, svc, mlp, etc.). Would like to branch out more. Also wondering, how are machine learning research repos set up for data preprocessing, exploration, etc?

### Day 15: 09/22/2023
* Finished the Data Visualization course, where I learned about histograms and density plots and plotting multiple features using things like hue or jointplots. Seaborn is awesome! This course has helped me see how I can approach visualizing data, and how easy it can be.

### Day 14: 09/21/2023
* Learned more tools and plots for using seaborn (Line charts, bar charts, heatmaps, scatter plots)

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

