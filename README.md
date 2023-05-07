# rog-SARTHAK.github.io


# SpaCy Tutorial
## Natural Language Processing or NLP:

NLP is a field of computational linguistics to process, parse and extract human language.
Some areas of NLP. Named Entity Recognition (NER), Part-of-Speech Tagging (POS), Syntactic Parsing, Text Categorization, Coreference Resolution, Machine Translation.

## Natural Language Understanding or NLU:

A sub-set of NLP is NLU. In this process, we deal with operations like Relation Extraction, Semantic Parsing, Question and Answering, Summarization, Paraphrasing, Sentiment Analysis.

## SpaCy:

SpaCy is a framework for NLP which works in Python.

The central data structures in spaCy are the Language class, the Vocab and the Doc object. The Language class is used to process a text and turn it into a Doc object. It’s typically stored as a variable called nlp. The Doc object owns the sequence of tokens and all their annotations. By centralizing strings, word vectors and lexical attributes in the Vocab, we avoid storing multiple copies of this data. This saves memory, and ensures there’s a single source of truth.

Text annotations are also designed to allow a single source of truth: the Doc object owns the data, and Span and Token are views that point into it. The Doc object is constructed by the Tokenizer, and then modified in place by the components of the pipeline. The Language object coordinates these components. It takes raw text and sends it through the pipeline, returning an annotated document. It also orchestrates training and serialization.

## SpaCy Architecture:

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/00.png" alt="import load" height="600" width="600" /> </p>

Img src: SpaCy documentation

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

### ent_type: 
In spaCy, ent_type refers to the entity type assigned to a particular token or span of text by the named entity recognition (NER) component of the spaCy pipeline. Named entity recognition is the process of identifying and categorizing specific named entities in text, such as people, organizations, locations, and dates. The ent_type attribute in spaCy provides information about the specific type of named entity that was identified by the NER component.

For example, consider the following sentence:

"Apple is looking to buy a startup in the UK for $1 billion."

The NER component in spaCy might identify "Apple" as an organization, "UK" as a geopolitical entity, and "$1 billion" as a monetary value. For each of these entities, spaCy assigns a specific ent_type attribute based on the entity's category, such as "ORG" for organizations, "GPE" for geopolitical entities, and "MONEY" for monetary values.

### ent_iob_:
In spaCy, ent_iob_ is another attribute that is used in conjunction with ent_type_ to represent the named entity recognition (NER) tags for each token in a document.

ent_iob_ is short for "inside-outside-beginning", and it indicates the position of a token relative to a named entity in the document. There are three possible values for ent_iob_:

"B": Beginning - this token is the first in a named entity.
"I": Inside - this token is inside a named entity, but is not the first.
"O": Outside - this token is not part of a named entity.

For example, consider the following sentence:

"The CEO of Apple, Tim Cook, announced a new product yesterday."

The NER component in spaCy might identify "Apple" as an organization and "Tim Cook" as a person. The ent_type_ attribute for the token "Apple" would be set to "ORG", and the ent_iob_ attribute would be set to "B" since it is the first token in the named entity. The ent_type_ attribute for the token "Tim Cook" would also be set to "PERSON", but the ent_iob_ attribute would be set to "I" since it is inside the named entity.

### lemma: .lemma refers to the base or dictionary form of a word. It is the form of the word that appears in a dictionary, and it is the form to which inflected forms (such as plurals or verb conjugations) can be reduced.

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

### Spacy nlp pipeline

The processing pipeline consists of one or more pipeline components that are called on the Doc in order. The tokenizer runs before the components. Pipeline components can be added using Language.add_pipe. They can contain a statistical model and trained weights, or only make rule-based modifications to the Doc. spaCy provides a range of built-in components for different language processing tasks and also allows adding custom components.

Text -> tokenizer -> tagger -> parser -> ner ... -> Doc

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/20.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/21.png" alt="token sent" width="700" height="400" /> </p>

### Rule based spacy

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/22.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/23.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/24.png" alt="token sent" width="700" height="400" /> </p>

### Spacy Matcher

Matchers help you find and extract information from Doc objects based on match patterns describing the sequences you’re looking for. A matcher operates on a Doc and gives you access to the matched tokens in context.

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/25.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/26.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/27.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/28.png" alt="token sent" width="700" height="400" /> </p>
