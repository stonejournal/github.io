---
layout: page
title: Methods
#subtitle: 
---

### Text Analysis Methods and Procedures

I performed my data analysis using the Python programming language within Jupyter notebooks (available though my project's GitHub repository). I had some very basic exposure to Python in Dr. Cameron Blevins' “Introduction to Digital Humanities” class at Northeastern University in the fall of 2019. In 2020 I had the opportunity to continue these studies with Dr. Laura Nelson in her “Analyzing Complex Digitized Data” class. I’m very grateful to Dr. Nelson for allowing me to work with my own data set for class assignments. These assignments were where I worked out the text analysis techniques used for this project and her feedback was very helpful as I worked through my code. Using Python allowed me to take advantage of the tools within Python’s Natural Language Toolkit (NLTK) for text processing and the Genism library for the word vector analysis portion of the project.

All of the Jupyter notebooks with my project code can be found in a GitHub Repository. (note: still need to create repository and add link)

### Data Pre-Processing
 
The scanned text arrived from HathiTrust in a “Pairtree” format. According to the [Pairtree project description](https://pypi.org/project/Pairtree/), Pairtree is a “a filesystem hierarchy for holding objects that are located by mapping identifier strings to object directory (or folder) paths two characters at a time.”  Essentially the text arrived as many hundreds of separate small text files within 28 numbered folders (one for each journal). These files generate the text-searchable portion of the digitized journal images. The small text files are numbered sequentially within the folders. To reassemble the journals I wrote a Python program that sorts the files by their file number in the folder and then opens each file and pastes it into a single text document. Separate issues are in chronological order within the journals, but some journals only contained partial years and a few spanned over two years.
 
Over the summer of 2020 I manually separated the journals out into individual monthly issues. This was a long and painful process due to the poor quality of the scanned text which made searching for particular keywords (like month names) an unreliable method of finding issue breaks. I investigated additional pre-processing, but decided not to edit the contents of the files more than splitting them up into issues. All other pre-processing was done within Python as part of the code for each analysis method.

### Text Analysis Methods

**Word Frequency Over Time**
As part of this work I made lists of words to use as “safety,” “health,” and “environmental” keywords.  These lists were developed through reading some sample issues and finding words that occurred in articles with related topics, through looking at modern words associated with these topics as well as finding synonyms and antonyms for those words.  One limitation of this approach is that many words can be used in multiple contexts that are extremely different from one another. For this reason my keyword lists were iterative -- I looked at a large number of words in my initial lists and then narrowed down the final lists to remove some of the more problematic multiple-use words (for instance "crushed" which was also pulling up crushed stone which is part of the quarry industry's product line and thus was appearing frequently) or words that almost never appeared.

The Python code for this process opens each document, converts the text to lowercase, uses NLTK tools to split the text into individual words (with punctuation separated from words) and searches the list of individual words for matches to each word provided in the keyword list. The output of this code is count of how many instances of each of these words appears within each issue. I entered the final counts into an Excel spreadsheet (using the OpenRefine program to tidy up the data). In the spreadsheet I normalized the word counts to their appearance per 1000 words to accommodate the fact that not all the issues have the same number of words. This allows numbers of words in each issue to be compared directly to other issues. I then converted the spreadsheets to .csv files that I re-loaded into python to make visualizations of word use over time using Python’s “Matplotlib” and “Seaborn” visualization packages. 

*[Results for this method can be found here](https://alsven.github.io/reswordfreq/)*

**Keywords In Context**
For my Keyword in Context text analysis the Python code uses NLTK’s “concordance” function.  This function allows me to search the text for a specific word, and then returns each instance of that word along with approximately 30 characters that appear on either side of the word.  In the code I wrote for this exercise I processed the text to be all lowercase, but did not remove strange characters or punctuation -- NLTK’s built-in tokenizing function separates punctuation from words so they do not affect the word search process.

The word frequency over time process was invaluable to informing me which keywords were worth looking at in context -- some words did not appear at all so I didn’t need to find them in context. At the same time, using the keyword in context program helped determine that some words, such as “crushed” discussed above were almost never appearing in a safety, health, or environmental context. After I ran my code on the text of the journal issue I moved the results to spreadsheets so that I could look at them in one place. I wanted a location where I can store and evaluate the results easily to see if the words extracted are related or not related to the topic of my study.  I could have also done this in a text file, but I found I spreadsheet cells easier to work with.

*[Results for this method can be found here](https://alsven.github.io/reskeywords/)*

**Word Vector Analysis**
For this portion of the project I trained three Word2Vec models using the Gensim (“generate similar”) natural language processing library in Python. Word2Vec models transform words within a document into a vector in space. This allows relationships between words to be represented mathematically.  The model can determine how often words co-occur (or “are embedded nearby each other”) and allow those relationships to be expressed.  Querying the models allows for identifying semantic relationships between a keyword and other words that are used within similar contexts.

For the first model I uploaded all 266 texts (approximately 52,125,670 words total -- although as discussed in the “Corpus Creation” section, it is likely many of those “words” are ORC errors), processed them to be lower case, removed punctuation, and turned them into a list of individual words by sentence.  My preliminary results turned up several words that were pieces of hyphenated words (“effi-” and “ciency” and “en-” and “gine”). For my final models I did a find and replace during the preprocessing period to remove the hyphen and combine the word pieces together. I could then query my model for words on my keylist to see what other words were used in the same semantic context as well as create visualizations using the tools in the “Scikit-learn” Python data analysis package.

Because I was interested to see if language around safety changed over time I decided to perform the same keyword investigations on two smaller models. One model consisted of issues from 1888 through 1910, and the other consisting of all issues from 1911- 1922. Due to my missing issues these two models were roughly the same size -- about 20 million “words” each.

*[Results for this method can be found here](https://alsven.github.io/reswordvec/)*