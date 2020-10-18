# Spacy

#How to Train spaCy to Autodetect New Entities (NER) [Complete Guide]

spaCy is an open-source library for NLP. It is widely used because of its flexible and advanced features. Before diving into NER is implemented in spaCy, let’s quickly understand what a Named Entity Recognizer is.

Named Entity Recognition is a standard NLP task that can identify entities discussed in a text document. A Named Entity Recognizer is a model that can do this recognizing task. It should be able to identify named entities like ‘America’ , ‘Emily’ , ‘London’ ,etc.. and categorize them as PERSON, LOCATION , and so on. It is a very useful tool and helps in Information Retrival. In spacy, Named Entity Recognition is implemented by the pipeline component ner. Most of the models have it in their processing pipeline by default.

# Load a spacy model and chekc if it has ner
import spacy
nlp=spacy.load('en_core_web_sm')

nlp.pipe_names
#> ['tagger', 'parser', 'ner']
