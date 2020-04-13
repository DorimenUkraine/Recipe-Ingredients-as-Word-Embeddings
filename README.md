# Recipes-Contexts-as Word Embeddings

Tree-based methods and ANNs have successfully been applied to predict the type of cuisine using a list of ingredients. 
Converting the ingredient list to a simple bag-of-words matrix, which is essentially a one-hot-encoded matrix, gives a prediction of accuracy of 78% on the Yummly recipes dataset.

### Can we use Word Embeddings to improve those results?

In this work, we use Gensim's Word2Vec implementation to convert a given list of ingredients to a fixed-length vector representation.
A cleaned recipe list and context vector representation gives classification accuracy of only 65%, which is lower than the baseline 78%.

So, is Word-Embedding bad?
Probably.
Probably Not.
There are caveats. 
For starters, the dataset has imbalanced classes.
Possibly, a more thorough (or maybe less thorough?) cleaning of data is needed.
Maybe the vectors built by Gensim need more tuning.

### Anyway, getting poor results is also good research, right?
