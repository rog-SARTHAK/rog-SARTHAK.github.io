# rog-SARTHAK.github.io


# SpaCy Tutorial
## Natural Language Processing or NLP:

NLP is a field of computational linguistics to process, parse and extract human language.
Some areas of NLP. Named Entity Recognition (NER), Part-of-Speech Tagging (POS), Syntactic Parsing, Text Categorization, Coreference Resolution, Machine Translation.

## Natural Language Understanding or NLU:

A sub-set of NLP is NLU. In this process, we deal with operations like Relation Extraction, Semantic Parsing, Question and Answering, Summarization, Paraphrasing, Sentiment Analysis.

## SpaCy:

A framework for NLP which works in Python.

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

Spacy displacy

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/13.png" alt="token sent" width="300" height="100" /> </p>


<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/14.PoS.png" alt="token sent" width="700" height="400" /> </p>


## Named Entity Recognition or NER

Iterate over doc object

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/15.png" alt="token sent" width="700" height="400" /> </p>

We will now explore word vectors in spacy medium model

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/16.png" alt="token sent" width="700" height="400" /> </p>


<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/17.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/18.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/19.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/20.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/21.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/22.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/23.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/24.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/25.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/26.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/27.png" alt="token sent" width="700" height="400" /> </p>

<p align="left"> <img src="https://raw.githubusercontent.com/rog-SARTHAK/rog-SARTHAK.github.io/main/Img/28.png" alt="token sent" width="700" height="400" /> </p>

#### H4
##### H5
###### H6

Alternatively, for H1 and H2, an underline-ish style:

Alt-H1
======

Alt-H2
------


Emphasis, aka italics, with *asterisks* or _underscores_.

Strong emphasis, aka bold, with **asterisks** or __underscores__.

Combined emphasis with **asterisks and _underscores_**.

Strikethrough uses two tildes. ~~Scratch this.~~



1. First ordered list item
2. Another item
⋅⋅* Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
⋅⋅1. Ordered sub-list
4. And another item.

⋅⋅⋅You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

⋅⋅⋅To have a line break without a paragraph, you will need to use two trailing spaces.⋅⋅
⋅⋅⋅Note that this line is separate, but within the same paragraph.⋅⋅
⋅⋅⋅(This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

* Unordered list can use asterisks
- Or minuses
+ Or pluses




[I'm an inline-style link](https://www.google.com)

[I'm an inline-style link with title](https://www.google.com "Google's Homepage")

[I'm a reference-style link][Arbitrary case-insensitive reference text]

[I'm a relative reference to a repository file](../blob/master/LICENSE)

[You can use numbers for reference-style link definitions][1]

Or leave it empty and use the [link text itself].

URLs and URLs in angle brackets will automatically get turned into links. 
http://www.example.com or <http://www.example.com> and sometimes 
example.com (but not on Github, for example).

Some text to show that the reference links can follow later.

[arbitrary case-insensitive reference text]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com






Here's our logo (hover to see the title text):

Inline-style: 
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

Reference-style: 
![alt text][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 2"






```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```
 
```python
s = "Python syntax highlighting"
print s
```
 
```
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```








var s = "JavaScript syntax highlighting";
alert(s);



s = "Python syntax highlighting"
print s




No language indicated, so no syntax highlighting in Markdown Here (varies on Github). 
But let's throw in a <b>tag</b>.



Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].  

You can also use words, to fit your writing style more closely[^note].

[^1]: My reference.
[^2]: Every new line should be prefixed with 2 spaces.  
  This allows you to have a footnote with multiple lines.
[^note]:
    Named footnotes will still render with numbers instead of the text but allow easier identification and linking.  
    This footnote also has been made with a different syntax using 4 spaces for new lines.
    
    
    
    
Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the 
raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3




> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote. 




<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>



