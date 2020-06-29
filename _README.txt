# WHU AI Hackathon Challenge I - Siemens AI Healthcare 
15/06/2020 - 22/06/2020

## Project description
As part of the first challenge of the WHU AI Hackathon series, we, Team HacKings, used a
piece of text describing Siemens' AI efforts in healthcare and analyzed it as a benchmark against
almost 20,000 company descriptions of AI startups scraped from Crunchbase to identify similarities
and ultimately come up with a list of 20 companies for Siemens to potentially invest in to enhance
their AI healthcare efforts.

## Approach
To identify the list of 20 companies with the best fit for Siemens' AI healthcare portfolio, based
on the companies' descriptions, we used different text similarity algorithms and implemented them 
using Python. Given the top 20 similar companies per algorithm we assigned points based on the
rank of a company with a higher similarity corresponding to a higher rank and, thus, a greater
number of points. Before applying any algorithmic calculations, we pre-filtered the list based on
specific categories related to healthcare and biotechnology. Additionally, we pre-processed the 
company description strings, removing punctuation, numbers, white space, and stopwords, and 
performing lemmatization. The pre-filtering and pre-processing methods used were equally applied
for each of the different algorithmic implementations.

## Algorithms
To identify text similarity between the benchmark string and the 20,000 company descriptions, we
employed the following algorithms to compare and cross-validate the results given different
approaches:

- Jaccard Similarity
- TFIDF
- Doc2Vec
- BERT

The rationale behind us using specifically these methods for assessing the text similarity is 
explained in the attached one-pager.

## Libraries / Packages
The following libraries / packages were used in the process of generating the attached solution:

- pandas
- numpy
- scipy
- sklearn
- gensim
- textacy
- re.py
- nltk
- sentence_transformers

Specific functions and methods used are to be found in the Jupyter Notebooks.

## File guide

- Challenge I - Team HacKings.pdf: Detailed description of analytical approach, rationale, and results
- Final Scoring_Top20.xlsx: Top 20 companies overall and Top 20 per algorithm
- Jaccard.ipnyb: Jaccard Similarity implementation code
- TFIDF.ipynb: TFIDF implementation code
- Doc2Vec.ipynb: Doc2Vec implementation code
- BERT.ipynb: BERT implementation code

Additionally, we included a PDF version of every Jupyter Notebook.
_______________________________________________________________________________________________________

## Disclaimer
We cannot guarantee, should the reader of this document try to replicate the solution we provided 
using our code, that the code will run as expected. In any case, such an instance would not be
subject to faulty code on our side, but could have numerous different causes, including a different
Python version installed on the reader's end, missing packages, a different OS, or other third-party
programs that prohibit the code from running properly. Moreover, note that this document does not,
in any way, acts as substitute for our actual solution provided as PDF and Excel files. Instead, this
README document is supposed to provide a high-level overview of what we did and the underlying
methodologies we used in the process.
_______________________________________________________________________________________________________

SB // TD
