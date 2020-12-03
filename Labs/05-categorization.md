# Computational Linguistics Lab 5: Categorization

Make a rudimentary categorizer that will guess whether a given text is written by Jane Austen or G.K. Chesterton. Your function should take any text as input, and return either "This looks like Jane Austen" or "This looks like G.K. Chesterton." 

Then, test your function using two new texts: 
 - a novel by either Austen or Chesterton which is *not* included in the Gutenberg NLTK corpus. 
 - a text of your choosing

Write 1-2 paragraphs about what you notice happening.

Here's one way you might do this: 

1. Load the Austen/Chesterton novels from the Gutenberg corpus. 
2. Create a document-term matrix of them, using TfidfVectorizer from Scikit-learn. Initialize it with the top 400 most frequent words.
3. Reduce the dimensions of your matrix from 400 to 2. 
4. Have your function compare components 0 and 1 with your test texts.

Here's another way you might do this:

1. Load the Austen/Chesterton novels from the Gutenberg corpus. 
2. Create a document-term matrix of them, using TfidfVectorizer from Scikit-learn. Initialize it with the top 400 most frequent words.
3. Find about 5 words are that are distinctive for either Austen or Chesterton.
4. Compare the frequencies of those five words with the frequencies of the test texts. (NB: you'll probably want to make sure that your test texts have enough words in them for word frequencies to be meaningful.)

And here's yet another way: 

1. Read [the NLTK book, Chapter 6, section 1.3 on document classification](http://www.nltk.org/book/ch06.html). 
2. Use that method (`i.e., nltk.NaiveBayesClassifier.train(train_set)`) to train a Naive Bayes Classifier. 
3. Use `classifier.classify()` to classify your test texts.
