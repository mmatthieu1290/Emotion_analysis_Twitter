# Emotion_analysis_Twitter

I use the labeled database obtained from https://www.kaggle.com/datasets/aadyasingh55/twitter-emotion-classification-dataset. Its contains 416809 tweets in english, each tweet  has a label which is a natural number between 0 and 5. If the label is closer to 0, its means that the sentiment of the tweet is negative, else it is positive. The distribution of labels is the following: 34% has label 0, 29% has label 1, 8% has label 2, 14% has label 3, 11% has label 4 and 3,5% has label 5. 

After pre-processing, I use a Tokenizer in order to transform words to sequences and then, I use a neuron network which begins with an embedding layer, after a convolution layer, a global average pooling, a dense layer with 16 neurons and each one has a relu activation function, finally a leyer with 6 neurons (one neuron for each class) with a softmax activation function. 

The results are pretty good, the difference between true label and predicted label is less that 1 in 86% of the tweets.
