# Computational Linguistics Lab 1: Exploring the NLTK

In a Jupyter notebook (either via Jupyter Lab or otherwise): 

1. Import the NLTK. 
2. You should've already downloaded the NLTK data by now, but if not, run `nltk.download('book')`. 
3. Import the NLTK test texts in your import cell, with `from nltk.book import *`. 
4. Choose a text to explore from among the test texts. 
5. Make concordances of a few different words. Maybe you'll want to choose some words that are common, and some that are uncommon.
6. Create dispersion plots of those words, showing where they appear in the corpus.
7. Use the `dir()` function on your chosen text to get a list of methods available to the `Text` object.
8. Try out a few of those methods for your `Text` object. For instance, try running `help(text6.collocations)` to see what the `.collocations()` method does. Then try running the method on your text. What does it do? For example, what does `.plot(10)` do?
9. Since a `Text` object is list-like, see what list methods will work with it. For example, try `mytext.count('someword')`, where `mytext` is your chosen text, and `someword` is a word of your choosing. 
10. Try any of the above methods in a `for` loop across a list of all text variables (`[text1, text2, text3...]`). For instance, you might want to try `.count('someword')`. Hint: to avoid `IndexError` problems when a word does not exist in the text, first check (`if someword in text`) that it exists. 
11. Finally, in a markdown cell, write about anything you noticed by performing the above tasks on your text. 

Submit your notebook on CourseWorks before 23:59 on Saturday.
