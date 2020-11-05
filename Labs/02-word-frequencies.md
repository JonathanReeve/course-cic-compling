# Computational Linguistics Lab 2: Exploring Word Frequencies

In a Jupyter notebook (either via Jupyter Lab or otherwise): 

1. Import the NLTK. 
2. You should've already downloaded the NLTK data by now, but if not, run `nltk.download('book')`. 
3. Find a plain text file (.txt file) from the Internet. A good source for these is Project Gutenberg. 
4. Download that plain text file to your computer. Ensure that it has the proper extension (.txt) and that its contents are relatively clean, i.e., are not filled with HTML markup. You should be able to read the contents of the file. 
5. Clean the file, if necessary, of any paratext, like licenses, tables of contents, and so on. You can do this either manually or programmatically.
6. Read the text into Python, using `open()`. You may have to pass options to `open()` for specifying a UTF-8 encoding, or ignoring errors. Ensure that your text is now a Python string by using `type()`. 
7. Tokenize the text, using `nltk.word_tokenize()`. 
8. Create a `nltk.FreqDist` object with the tokens. Explore its word frequencies, hapaxes, and so on. 
9. Compare your text's word frequencies with that of another text (for example, one of the built-in texts from the NLTK). Does your text use "America" more than Nixon did, for instance? What are some words that only appear in one text, but not in the other? 

Submit your notebook on CourseWorks before 23:59 on Saturday.
