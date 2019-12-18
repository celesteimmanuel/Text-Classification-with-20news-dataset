# Text-Classification-with-20news-dataset

Programming language : Python

### Dataset

Dataset is famous 20 newsgroups dataset
you can find the dataset freely [here](https://archive.ics.uci.edu/ml/datasets/Twenty+Newsgroups)

### Requirements

+python 3.XXX

+Libraries:
  + nltk for preprocessing the text
  + os 
  + pickle to save the data-structures
  
### Code

+ Done the pre-processing i.e removing the stop words, symbols, numbers, stemming, upper to lower
+ Divide the data into train and test.
  + There are 20 folders where each folder contains around 1000 documents out of which 850 are used for training and 150 are for testing
+ construct the vocabulary and build frequency dictionary of each words
+ Since we are using * Naive Bayes * as classifier we have to use smoothing in order to generalise for un known words from test set.

+ for smoothing tried 1,5,10,100 as values.
+ Now when we give un known test document it will calculate the probabilty of test doc belongs to each class with different smoothing values and finds the most probable class.
