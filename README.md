# rog-SARTHAK.github.io


# SpaCy Tutorial
## Natural Language Processing or NLP:

NLP is a field of computational linguistics to process, parse and extract human language.
Some areas of NLP. Named Entity Recognition (NER), Part-of-Speech Tagging (POS), Syntactic Parsing, Text Categorization, Coreference Resolution, Machine Translation.

## Natural Language Understanding or NLU:

A sub-set of NLP is NLU. In this process, we deal with operations like Relation Extraction, Semantic Parsing, Question and Answering, Summarization, Paraphrasing, Sentiment Analysis.

## SpaCy:

SpaCy is a framework for NLP which works in Python.

### Dependencies to get started:

Open Google colab notebook or Jupyter notebook and follow through the instructions and code.

### Find the dataset here:
https://github.com/rog-SARTHAK/rog-SARTHAK.github.io/tree/main/Dataset

### SpaCy Installation and loading:


<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/01. import load.png" alt="import load" width="600" /> </p>

### Load the dataframe:

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/02. open nlp data.png" alt="dataframe" width="500" /> </p>

### Text object and doc object difference:

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/04.text obj doc obj.png" alt="txt obj doc obj" width="500" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/05.png" alt="txt obj doc obj" width="500" height="600" /> </p>

SpaCy automatically detects characters with period like U.S.A.
SpaCy removed the punctuation mark like the parenthesis (U.S.A. or USA) and treated them as individual characters

If we split tokens by white space separation, it would look something like this

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/06.png" alt="txt obj doc obj" width="500" height="400" /> </p>


Sentence Boundary Detection (SBD) in NLP is identification of sentences ina text.
In english, abbreviation of word is also demarcated with period punctuation.
So we can't just split and demarcate a sentence just separated by period.

We will now tokenise entire text to sentence level

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/07.png" alt="token sent" width="700" height="400" /> </p>

To access one of the sentence we have to convert and access as a list

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/08.png" alt="token sent" width="700" height="100" /> </p>

Each individual token has a bunch of meta-deta buried within it
This meta-data is called attributes

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/09.png" alt="token sent" width="700" height="400" /> </p>

Printing Entity form

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/10.png" alt="token sent" width="700" height="400" /> </p>

lemma form, morphological form, parts of speech and dependency form

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/11.png" alt="token sent" width="700" height="400" /> </p>

lang_ , sentence morph

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/12.png" alt="token sent" width="700" height="400" /> </p>

### Spacy displacy

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/13.png" alt="token sent" width="300" height="100" /> </p>


<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/14.PoS.png" alt="token sent" width="700" height="400" /> </p>


### Named Entity Recognition or NER

Iterate over doc object

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/15.png" alt="token sent" width="700" height="400" /> </p>

We will now explore word vectors in spacy medium model

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/16.png" alt="token sent" width="700" height="400" /> </p>


<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/17.png" alt="token sent" width="700" height="400" /> </p>

Using word vectors with spacy

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/18.png" alt="token sent" width="700" height="400" /> </p>

Word embedding - apple and banana

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/19.png" alt="token sent" width="700" height="400" /> </p>

###Spacy nlp pipeline

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/20.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/21.png" alt="token sent" width="700" height="400" /> </p>

### Rule based spacy

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/22.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/23.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/24.png" alt="token sent" width="700" height="400" /> </p>

### Spacy Matcher

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/25.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/26.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/27.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/28.png" alt="token sent" width="700" height="400" /> </p>
