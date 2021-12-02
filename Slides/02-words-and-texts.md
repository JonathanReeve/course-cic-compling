---
title: "Computing in Context: Computational Linguistics"
subtitle: "Lecture 1: Words and Texts"
author: Jonathan Reeve
date: 29 October 2020
---
    
# Linguistics 

## Syntax

## Not this kind

![](https://media.giphy.com/media/ifdPjn6m4WyNlnXMTj/giphy.gif)

## Natural language syntax

 -  The structures of language
 -  E.g., Sentence structure

## Semantics

![](https://media.giphy.com/media/sKF481S11DIYg/giphy.gif)

 -  The meanings of language
 -  Lexical relations
 -  Ambiguity

# Computational Linguistics

## Also known as, or similar to

natural language processing, computational text analysis, digital humanities

# Common subfields / tasks

## Machine translation 

![](https://media.giphy.com/media/3oEduO5yKmG57QyUU0/giphy.gif)

## Natural language understanding

![](https://media.giphy.com/media/tnYri4n2Frnig/giphy.gif)

## Natural language generation 

E.g., chatbots

![](https://media.giphy.com/media/tKxvuLmOaKEDQ2hWie/giphy.gif)

## Other applications

 - Search engines
 - Grammar checkers
 - Text classification
 - Cultural analytics
 - So, so much more

## Programming languages

 - Can be done in most programming languages
 - Python, Java are the most common now
 - Lisp, Haskell, OCaML use a very different approach

# Computational Linguistics in Python

## Libraries 

 -  NLTK, The Natural Language ToolKit (biggest, oldest)
 -  SpaCy (newer, fastest, industry-standard)
 -  TextBlob (casual NLP)
 -  Pandas (data science)
 -  and many, many more

## Libraries are not magical 

![](https://media.giphy.com/media/12NUbkX6p4xOO4/giphy.gif)

## You can read the code

https://github.com/nltk

## You can write your own version

```python
def lexical_diversity(text): 
    return len(set(text)) / len(text) 
```

## Let's jump straight to the fun stuff

But backtrack when necessary

# The NLTK

## The book

 - http://www.nltk.org/book/
 - Very beginner friendly!

## Comes with Anaconda

Otherwise: `pip3 install nltk`

## NLTK Data

 - Does not come with Anaconda
 - Language data, corpora need to be downloaded
 - Run `nltk.download('book')` once on your computer

## NLTK Contents

 - test corpora (nltk.corpus)
 - lots of built-in functions
 - the `Text` object with its many methods

Try `dir(nltk)` and `help(nltk)`

# Some Advice

## Be curious

![](https://media.giphy.com/media/ptk7aim49C8qQ/giphy.gif)

 - Take things apart. Break things. (But make backups first.)
 - Use Jupyter checkpoints. 

## Don't despair

![](https://media.giphy.com/media/hrRJ41JB2zlgZiYcCw/giphy.gif)

Errors are your friends. 

## Your debugging friends

 - `print()` everything
 - Run `type()` on everything
 - Read documentation with `help()`
 - Get a list of methods with `dir()`

