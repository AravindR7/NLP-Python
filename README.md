# NLP-spaCy-python

spaCy is one of the fastest Natural Language Processing framework in python.

Install spaCy using the command:

`pip3 install spacy`

# Spacy's language models

A language model is a statistical model that lets us perform NLP tasks such as POS-tagging and NER-tagging.

Download these models using:

`spacy download en` # english model
`spacy download de` # german model
`spacy download xx` # multi-language model

Download specific model for your spaCy installation:

`python3 -m spacy download en_core_web_sm`

Run the following command in your Python shell:
```
import spacy
nlp = spacy.load(‘en_core_web_sm’)
doc = nlp('This is nlp with spaCy')
```
When you call NLP on text , spaCy first tokenizes the text to produce a Doc object. Doc is then is processed in several different steps, which we also refer to as pipeline.

![Default pipeline](https://miro.medium.com/max/613/1*gP6Hm4OIjWwMz2rVHTaWJQ.png)

Tokenizing is task of splitting sentence into meaningful segments called tokens. These segments could be words, punctuations, numbers or other special characters that are building blocks of sentence.

SpaCy’s default pipeline also preforms rule based matching. This annotates the text with more information and adds value during preprocessing.

For the datailed explanation please do go through the blogs I have published on Medium

1. Natural Language Processing using spaCy in Python(part-1)
https://medium.com/analytics-vidhya/natural-language-processing-using-spacy-in-python-part-1-ac1bc4ad2b9c

2. Topic Modeling using Gensim-LDA-Python
https://medium.com/@AravindR07/nlp-using-spacy-and-topic-modeling-using-gensim-python-42c4574830d


# Text Summarization
Is a process of distilling most important information from source of text while preserving the meaning of the content.

Main idea:

Text processing(preprocessing).
Word frequency distribution - how many times each words appear in document.
Score each sentence depending on the words it contain and the frequency table.
Build summary by joining every sentence above a certain score limit.

#Similarity queries and text summarization blog:
https://medium.com/@AravindR07/similarity-queries-and-text-summarization-in-nlp-50ef4cf04f7b
