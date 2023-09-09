# 100-days-of-data-science
## Motivation:
* Trying to get gud at machine learning, bc it's the future and it's cool
* I tend to get analysis-paralysis when it comes to choosing a project to work on
* With this challenge, I'll give myself space to work on small/toy projects to start and will organically grow to work on bigger challenges

## Goal
* Get hands-on practice with exploratory data analysis, training, and evaluation
* Apply the things I've learned in AI, ML, Deep Learning, Computer Vision, and AI System Design
* At the end, I want to be able to take on the [Google Contrails competition](https://www.kaggle.com/competitions/google-research-identify-contrails-reduce-global-warming)

## Getting Started
### Day 0: 09/07/23
* Read Andrew Ng's ["How to Build Your Career in AI" eBook](https://info.deeplearning.ai/how-to-build-a-career-in-ai-book#MYL-form)
* Need to remember my career is long -- all I have to do is start now and do a little every day

### Day 1: 09/08/23
* Decided to start working my way through Kaggle's Getting Started challenges.
* Working on the classic MNIST dataset. I must've done this before, but am doing it without following any tutorial this time and am learning a lot more along the way (not just hitting run on cells).
* Tried with some sklearn classification algorithms (svm.SVC, trees.DecisionTreeClassifier, neighbors.KNearestNeighborsClassifier), mostly with default settings and they performed well
* SVM seems to perform the best but is also the slowest
* Evaluation is hard bc have to choose the right metrics
* Here's the repo where I'll keep track of those notebooks: https://github.com/alexcjwei/getting-started-kaggle
* Tmrw: try CNN then move on


### Day 2: 09/09/23
* Making CNN to classify MNIST digit dataset
* Learning how to create datasets and dataloaders
* How loss & optimizer & a net relate must be through the net parameters, but it's not entirely clear how
* Not sure how CNN dimensions work
* I think it's bc there's no channels in the MNIST dataset. (This ended up being the problem, needed to add a dimension for a single channel. But I should brush up on the dimensionality of CNNs anyways)
* Watched StatQuest on CNNs https://youtu.be/HGwBXDKFk9I?si=7FruRffmcSn9G1b9
