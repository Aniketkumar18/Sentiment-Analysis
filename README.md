# Sentiment Analysis using RNN

## In this project we will implement a recurrent neural network that performs Sentiment Analysis

Here we will use a dataset of movie reviews, accompanied by sentiment labels: positive or negative

**First**, we'll pass in words to an embedding layer. We need an embedding layer because we have tens of thousands of words, so we'll need a more efficient representation for our input data than one-hot encoded vectors. You should have seen this before from the Word2Vec lesson. You can actually train an embedding with the Skip-gram Word2Vec model and use those embeddings as input, here. However, it's good enough to just have an embedding layer and let the network learn a different embedding table on its own. In this case, the embedding layer is for dimensionality reduction, rather than for learning semantic representations.

**After** input words are passed to an embedding layer, the new embeddings will be passed to LSTM cells. The LSTM cells will add recurrent connections to the network and give us the ability to include information about the sequence of words in the movie review data.

**Finally**, the LSTM outputs will go to a sigmoid output layer. We're using a sigmoid function because positive and negative = 1 and 0, respectively, and a sigmoid will output predicted, sentiment values between 0-1.
