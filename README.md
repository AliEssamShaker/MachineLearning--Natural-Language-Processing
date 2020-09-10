# MachineLearning--Natural-Language-Processing

Natural Language Processing:

Bag-Of-Words model: -

An example of the application, is the auto generated recommended reply texts when an email is received in Gmail for instance.

I created a Bag-Of-Words model for a dataset called Restaurant Reviews and used different machine learning models such as Naïve Bayes model to predict how well our NLP was or how well we were able to predict whether this review was a positive review (1) or a negative review (0). 

I start off by as usual importing the required libraries, then, importing the dataset. Following that, I clean the texts in the dataset to ease the learning process of our ML models.

The first library I am using is the “re library”, and this one will allow us to simplify the reviews.
I also import the nltk library which allows us to download the ensemble of the stopwords (Words that are not really necessary and do not help guide us e.g the, a, and, or, etc), and then I imported stopwords from the nltk.corpus library.
And then from the nltk.stem.porter I imported the PorterStemmer class, which I used to apply stemming on the reviews. Stemming is basically a process of taking only the root of a word that indicates enough about the meaning of this word, for example, let’s say there was such a review “Oh this place astonished me”, stemming would remove any conjugations and would transform the word “astonished” into “astonish” to simplify the reviews, and if we do not apply stemming we will end up with a column for the word “astonished” and another column for the word “astonish”, and since they pretty much give us the same guidance in terms of whether the review is positive or negative, it would be redundant to have both columns in our matrix. 

Following that, I start cleaning the data by iterating through the data set and cleaning every row and then appending the cleaner version to a list.

After the cleaning phase, I created the Bag of Words, split the dataset into a training set and a test set, trained the classification models on the training set, predicted the test set results, and lastly made the confusion matrix.








