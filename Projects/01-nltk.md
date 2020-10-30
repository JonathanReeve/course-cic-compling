# Project 1: Using the NLTK

Computing in Context: Computational Linguistics

Due November 9th at 23:59.

## In preparation

1. Make sure you've watched Lecture 1, in the video library of the main course CourseWorks page.
2. Read [Chapter 1 of the NLTK book.](http://www.nltk.org/book/ch01.html).

## The assignment

Use the NLTK to do an exploratory analysis of a text or corpus of your choosing. The text should be at least 1000 words, be written in English, and could be one of the built-in texts, or another text of your choosing. You could even choose to analyze your own writing. Note that your text must be in plain text format (not PDF or HTML) if you want it to work properly.

To make a new NLTK `Text()` object from a text file (we'll learn this in Lecture 2): 

1. Load the text file into a string
2. Tokenize the string with `nltk.word_tokenize()`
3. Call the `Text()` function on the list of tokens, and assign the result to a new variable.

Choose **5** of the analyses below. For each, discuss your results in one paragraph in a markdown cell. 

1. A dispersion plot of several words. Write about what you notice about the word distributions across the text or corpus. 
2. Concordances for several words. Write about what you notice about that word's contexts. 
3. A `FreqDist` word frequency distribution, with common words and their counts. Use a few methods available to the `FreqDist` object. Write about what you notice about the word frequencies.
4. A list of hapax legomena. What do this text's hapaxes say about it? 
5. A comparison of your text with another. Write about how your text diverges from others, and is distinctive. 
6. Generated language, using `.generate()`, emulating the language of your text.
7. Several windows of word frequencies: very frequent, medium-frequent, and infrequent. Write about where in these windows you see mostly syntactic words, and where you see mostly semantic words.
8. The text's collocations. Write about what you notice about the text's frequently-occurring words. 
9. The text's frequent bigrams and trigrams. To achieve this, you can combine `nltk.bigrams` and `nltk.FreqDist`. Write about the patterns you see among these lists.
10. A list of words from your text which match a given pattern. For example, you might want to look at words that end in "-ize" or "-ise," superlatives ending in "-est," or words beginning "ph-." (You can test for these using the Python string methods `.endswith()` and `.startswith()`). 

Submit a single .ipynb file to CourseWorks with yourUNI\_project1 as the name. So, for example, I would submit jpr2152\_project1.ipynb.
