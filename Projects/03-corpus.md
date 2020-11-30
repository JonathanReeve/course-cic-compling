# Project 3: A Corpus Analysis

1. Assemble your own corpus of four or more English texts, each containing more than 500 words each. Don't use any of the built-in NLTK texts, but make your own. Here are some ideas: 

 - Scripts from a TV show you like. (Subtitles may also work just as well.)
 - Character speech from _Hamlet_, categorized by character. 
 - All the episodes (chapters) of James Joyce's novel _Ulysses_
 - All (or some of) the tales from _The Canterbury Tales_
 - Ten different translations of the same book, from another language into English
 - All the novels by a single prolific writer you've read
 - Book reviews, and the texts of the books they're reviewing
 - Biographies of writers, and what those writers wrote
 - A diachronic corpus, containing scientific articles from a single discipline, from 1900 to 2020
 - News articles, from a variety of left- and right-leaning publications, about the recent pandemic

You may want to organize your corpus first as a series of plain text files, and read each file into Python. Alternatively, put everything in one file, and add unique markers (like `@@@@@`) that you can use to divide the text later (`.split('@@@@@')`). Please do not copy and paste text into a Jupyter cell. 

Load your corpus into _a single variable_, like a nested dictionary or a nested list, that _contains labels_. 

For example, if you were using the _Canterbury Tales_: 

```python
cantTales = {"knight": "...the text of the knight's tale would be here ..."
             "miller": "...the text of the knight's tale would be here" 
            }
```

If you were using a more hierarchical corpus, like a TV show with episodes and seasons, it would look more like this: 

```python
tvShow = {"season-1": 
            {"episode-1": "...the text of S1E1 would be here ...", ... } 
          "season-2": 
            {"episode-1": "...the text of S2E1 be here", ... }
}
```

2. As a "sanity check," to make sure your corpus doesn't have text problems, print out a small (~200 characters) random segment of each text. You can use the `random` library to generate a random integer between zero and the length of your text, and then use that to select the indices you need for slicing.

3-4. Show some basic text statistics about each text in your corpus. Choose _four_ of these: 

 a. Length, in tokens, of each section
 b. Type/token ratio of each section
 c. Part-of-speech distribution for each section
 d. Ratio of male pronouns to female pronouns 
 e. Readability score for each
 
5-10. Conduct some more advanced text analysis of your corpus. Choose _two_ of the following analyses. Make sure to label them with (a), (b), and so on, so that we know which you've chosen. For each, write 2-4 paragraphs where you interpret what you see happening.

 a. A comparative stylometric analysis of your corpus texts. Create a scatter plot with your results. Then, try your analysis again, but use content words, rather than style words. 
 b. A categorizer. Sometimes it's fun to misuse a categorizer. For example, you might write a categorizer that determines the likelihood that a text is a scientific article, and then run that categorizer over a dozen Victorian novels, to determine novel that is the most "scientific." Evaluate your categorizer for accuracy. 
 c. A WordNet-based lexical categorizer. Use WordNet to categorize the words in your texts to a given depth. Create some sort of visualization with your results. 
 d. A trigram-model language generator. 
 e. A concordance for a few word/POS patterns, like "the best NN," but of any length, and which provides context. 
 f. An analysis of the most/least distinctive words of each of your texts. How do they compare with one another?
 g. A new analysis, of your invention. Feel free to contact me if you want some help in brainstorming. You'll want to explain your methods, as well as your results.

Submit your project as a Jupyter notebook file (.ipynb) no later than Monday, December 14. Remember that you can't use your late hours for this assignment. 

Make sure your notebook contains your code, the output of that code, and your discussions. 
