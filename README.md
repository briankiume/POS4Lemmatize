# POS4Lemmatize
A simple function to quickly return the probable Part of Speech (POS) argument when lemmatizing.   

## Description 
The function only takes **1 word token** as an argument. 
>*Example:* was

## Usage
The code below shows its usage on a word token, within a document, within a corpus.  
```
lemmatizer = WordNetLemmatizer()
lemmatized_corpus = []
for doc in all_tokenized:
    lemmatized_doc = []
    for token in doc:
        lemmatized = lemmatizer.lemmatize(token, get_part_of_speech(token))
        lemmatized_doc.append(lemmatized)
    lemmatized_corpus.append(lemmatized_doc)
```
## Requirements
The following packages are required for the script to work:

* nltk
 
## License
MIT License. Copyright (c) 2022 Brian Kiume