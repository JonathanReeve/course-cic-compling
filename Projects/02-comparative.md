# Project 2: Comparative Linguistics

Computing in Context: Computational Linguistics

Due November 23rd at 23:59.

## In Preparation

1. Make sure you've watched all the prior lecture videos from the video library, or have attended all the lectures.
2. Spend some time learning Esperanto. 

 - [Duolingo](https://www.duolingo.com/) is a game-like language learning app, which allows you to learn Esperanto. 
 - [Lernu.net](https://lernu.net/en/kurso/nakamura) provides an alternative learning method. 

[A useful cheat sheet for Esperanto grammar may be found here on Lernu](https://lernu.net/en/gramatiko). 

At minimum, understand common word endings: 

 - Nouns end in -o 
 - Past tense verbs end in -is
 - Conditionals (would, could) end in -us
 - Objects end in -n

and understand that word order in Esperanto is flexible: 

 - Adamo manĝas pomon. (Adam is eating an apple.)
 - Pomon manĝas Adamo. (Adam is eating an apple.)
 - Manĝas pomon Adamo. (Adam is eating an apple.)
 
and that words in Esperanto are not limited to a single part of speech, but may be modified at will: 

- _Eble_: maybe
- _Eblas_: that could be
- _Eblis_: that could have been
- _Eblo_: a possibility
- _Ebleto_: a mild possibility
- _Maleblo_: an impossibility

Thus, _la vetero belas_, or "the weather is beautifulling." 

## The Assignment

1. Choose a work that was originally written in English, and has been translated into Esperanto. Ideally it would be a work you've already read. [Project Gutenberg contains a number of works in Esperanto](http://www.gutenberg.org/browse/languages/eo). 

Here are some possibilities: 

 - [La Aventuroj de Alicio en Mirlando](http://www.gutenberg.org/ebooks/17482)
 - [Robinsono Kruso](http://www.gutenberg.org/ebooks/11511)
 - [La Falo de Uŝero-Domo](http://www.gutenberg.org/ebooks/17425)
 - [Hamleto, Reĝido de Danujo](http://www.gutenberg.org/ebooks/37279)

2. Download both the Esperanto version, and the original English version. Clean each text of Project Gutenberg license material, and paratext (tables of contents, and so on). Load each text into Python variables. 

3. Choose a tokenizer to use which will handle both English and Esperanto. Note that you will likely need a language-agnostic tokenizer, since `nltk.word_tokenize()` will not behave as expected with Esperanto. Tokenize each text.

4. Compare your pair of texts computationally, using *five* of the analyses below. After each analysis, write 1-2 paragraphs where you discuss your results. (Thus, a minimum of five paragraphs total.)

--- 

## The Analyses

(Choose *five*.)

1. Write an ad-hoc POS tagger for Esperanto, using your knowledge of its word endings. It doesn't have to be complete, but should handle JJ, NN, VRB, and PRP. Use this to POS-tag your Esperanto text. Compare the proportions of POSes between the Esperanto and English text, which you can tag with `pos_tag()`. What are the differences between the two? 
2. How many words are in each text? Find a sentence or two that are translations of one another, but have a big difference in word length. Explain why one needs more or fewer words than its translation.
3. Compare the most frequent trigrams, or 4-grams, or 5-grams, of each. Are there some that don't seem to have counterparts in the other language? 
4. Familiarize yourself with Esperanto [suffixes](https://lernu.net/en/gramatiko/sufiksoj) and  [prefixes](https://lernu.net/en/gramatiko/prefiksoj). Choose a few to identify and discuss. For example, `-aĉ-` expresses poor quality. So _domo_, house, becomes _domaĉo_, a badly constructed house that's falling apart. Write a Python function to find any `-aĉo` (or `-aĉe`, `-aĉa`, etc.) words in your text. What are the English equivalents of those? Do these highlight any aspects of the text for you?
5. Choose several people (characters, in fiction, or real people, in nonfiction) that appear in your text. For each, write a function to collect all the adjectives you see in the same sentences as those people's names. What do you notice about them? Are they roughly the same in both languages? 
6. What are the kinds of things (or people, or concepts) that are more likely to be the grammatical objects (-n endings, in Esperanto) of sentences? What about grammatical subjects? Are these different between the English and the Esperanto versions? (To find grammatical subjects and objects in English, use [dependency parsing](http://www.nltk.org/book/ch08.html).)
7. Familiarize yourself with the concept of an _idiom_. Esperanto has almost no idioms. Find 2-3 idiomatic phrases in your English text, and find their Esperanto translations. How are they worded unidiomatically in Esperanto? What happens when you try to put the idiomatic phrase into Google Translate, and then translate it back again?
8. Divide your texts into two or more sections. For example: the beginning of the text, the middle of the text, and the end of the text. You might also split your text on chapters. What words occur more in one category than the other? (Consider counting punctuation marks, too!) How are these different between the two languages? 
9. Compare plural nouns between your two texts. (NNS, NNP, or NNPS in English, -j in Esperanto.) What kinds of things are more or less likely to be plural? How do these differ between languages? 
10. Choose several medium-infrequent word roots from your Esperanto text. (A word root is the bare word, without prefixes or suffixes.) Do a concordance for your word root using [tekstaro.com](https://tekstaro.com/). (Select `ĉiuj` to select all texts.) Then search Project Gutenberg English texts for the English cognates of those words. (You might try Googling `word site:gutenberg.org lang:eng`, for instance.) How are they similar or different?
11. Write a Python function to find the longest word in a text. Run that program on both of your texts. If the longest Esperanto word is a compound word, what are its constituent words or word fragments? How are those rendered in the original English?

Submit a single .ipynb file to CourseWorks with yourUNI\_project2 as the name. So, for example, I would submit jpr2152\_project2.ipynb.
