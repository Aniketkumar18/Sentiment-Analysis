# Sentiment Analysis using RNN

## In this project we will implement a recurrent neural network that performs Sentiment Analysis

Here we will use a dataset of movie reviews, accompanied by sentiment labels: positive or negative

**First**, I passed words to an embedding layer. We need an embedding layer because we have tens of thousands of words, so we'll need a more efficient representation for our input data than one-hot encoded vectors. It's good enough to just have an embedding layer and let the network learn a different embedding table on its own. In this case, the embedding layer is for dimensionality reduction, rather than for learning semantic representations.

**After** input words are passed to an embedding layer, the new embeddings will be passed to LSTM cells. The LSTM cells will add recurrent connections to the network and give us the ability to include information about the sequence of words in the movie review data.

**Finally**, the LSTM outputs will go to a sigmoid output layer. I am using a sigmoid function because positive and negative = 1 and 0, respectively, and a sigmoid will output predicted, sentiment values between 0 - 1.

I have done sentiment analysis on customer reviews using RNN and LSTM.
