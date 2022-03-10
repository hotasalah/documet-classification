# documet-classification
### Transfer Learning using pretrained word embeddings for document classification.

This example uses Embeddings for text classification depending on three main components: first, loading the pretrained word embeddings, then, finetuning these pretrained embeddings by classifying entire news articles, and finally, using a convolutional neural network to capture the spatial relationships between words.
Here I used the AG News dataset. To model the sequences of words in AG News, I used a SequenceVocabulary class, to bundle several tokens vital for modeling sequences. The Vectorizer class demonstrates how to use this class.
After describing the dataset and how the vectorized minibatches are constructed, the pretrained word vectors are loaded into the Embedding layer. Then, the model combines the pretrained Embedding layer with a CNN. In an effort to scale up the complexity of the model to a more realistic construction.
I also identify the places where I utilize dropout as a regularization technique.
Finally, I conclude the example by evaluating the model on a test set and discussing the results.
