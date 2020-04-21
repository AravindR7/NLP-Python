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
