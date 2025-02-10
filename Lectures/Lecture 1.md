---
tags:
  - Marinus
  - Lectures
  - FirstPass
Created: 2025-02-07
---
# What do they plan to teach?

Foundations of NLP techniques. 
- Basic concepts first then we move to word vectors, feed-forward neural networks, recurrent neural networks, encode-decoder models (transformers), attention, transformers.

Then we move onto understanding and ability to build systems for real world problems.

# Book

Speech and Language Processing - Textbook
- Dan Jurafsky and James H. Martin

Natural Language Processing Conference

And some more resources.

# Assignment and grading

- <mark style="background: #ADCCFFA6;">Assignments (groups of 3) </mark>(30%)
	- Part 1: n-gram Language Modelling
	- Part 2: Sentiment Analysis using Logistic regression
		- But this we have to implement ourselves, no scikit-learn 
- <mark style="background: #ADCCFFA6;">Project (group of 3)</mark> (40%)
	- Architecture from hugging face 
	- advises us to use Colab
	- Report on the process implementation (35%)
	- Presentation (5%)
		- four minute recording per group
- <mark style="background: #ADCCFFA6;">Written Exam (30%)</mark> (digital)

To Pass:
- complete all assignments
- 5 min in assignments (+ project)
- 5 min in written exam 

# What is NLP?

Concerned with designing and analysis of computational algorithms and representations used to process natural human language. [Eisenstein, 2018]

- <mark style="background: #BBFABBA6;">Computational algorithms:</mark> structured procedures of model to generate or classify text or speech. Allow computers to analyze, interpret, and generate text or speech
- <mark style="background: #BBFABBA6;">Representation:</mark> The way in which text or speech data is structured, encoded, or transformed so that a machine can process and manupulate it effectively. 

The challenge is finding a way to represent that piece of text while still retaining the meaning and information imbedded in that text.

Its not building text decoders, its finding a way to encode and decode that data to make it easier to build bigger systems.

Everything relies on the representation.

# NLP as an interdisciplinary field

Combines:
- Computational linguistics
- Machine Learning
- Deep learning 

# History

Georgetown Experiment 1954
"Within three to five years, machine translation will be solved"

## Rule based NLP

[[Rule-based NLP.canvas|Rule-based NLP]]

Used Eliza (Weizenbaum, 1966) as an example of a rule-based NLP

what matthijs said i should write:
- Main point: Understanding language is really hard.

# So why is language so difficult to understand?

1. The mapping between levels of linguistic representation (Morphology, Syntax, Semantics, Pragmatics) is very complex.
	1. Morphology: Structure
	2. Syntax: structure and grammatical rules
2. Application-specific representation choices 
	1. for machin translations, syntactic and semantic representations are crucial
	2. fro sentiment anaylysis, pragmatic cues like sarcasm and contextual sentiment shifts are essential.
3. Ambiguity at lexical, syntatic,, and semantic levels
4. Variability in dialects, accents, and linguistic diversity, we all have diffirent cultures
5. challenges in detecting humor sarcasm and irony
6. and another one

Everything is context dependent

Ambiguity
"Please have a seat." 
"Thanks" - takes seat

# Rules are hard - Lets learn from data

<mark style="background: #FFB86CA6;">The rise of statistical learning</mark> 

get the dates from lecture 

## Statistical Machine Translation

- parallel corpora 
	- need this to train a model
	- is a direct matching of a sentence in one language and another language
- you have to train a seperate model to do translations from russian to english and english to russian.

You have to hand craft some features of how the model should process the data, this is very tedious and now we have to count millions of datapoints to build features.

This brought us to:

# Deep leaning era

Large scale data. 
Models trained on millions of pairs
end-to-end designing of the model without intermediate steps of designing features.

this was the time when we started allowing deep Neural Networks to learn features and not us.

# Key Components of NLP
interdisciplinary field and enables machines to read, interpret and generate human language.

- level of linguistic analysis
- NLP Tasks & Application
- Computational Models in NLP
- Representation of Language in NLP
- Challenges in NLP

# Linguistic analysis

- Phonetics & Phonology: Study of sounds (speech recognition)
- Morphology: Understanding word formation (e.g., stemming, lemmatization)
- Syntax: Understanding sentence structure and grammatical rules. Parsing Parts-of-Speech tagging.
- Semantics: Meaning of language beyond syntax, especially within different contexts. (Sentiment analysis, speech act recognition)
- Pragmatics: ... missed it

# Different systems

- Translators
- Conversational
- Classification
- Question answering (QA)
- Summarization
- Text generation

## Computational models

- Rule-based
- statical learning  (not really discussed anymore) <mark style="background: #ABF7F7A6;">Assignment Part 1</mark>
- Neural Networks & deep learning

# Representation of Language in NLP

- Bag of Words (BoW): simple numerical representation of text
- Word Embeddings: Dense vector representation Word2Vec, CloVe, FastText
- Contextualized Embeddings: Meanign varies based on teh context like BERT, ElMo, GPT

# Challenges

- Ambiguity 
- Data sparsity
- Language Variability
- Ethical Concerns
How do we train a model with the changes in modern languages 

# NLP Pipeline

Firstly define your problem.

- Raw Text Input: initial unprocessed text
- Text Preprocessing: Cleaning, Tokenization, stopwords
- Feature extraction
- Model & Learning
- Evaluation & optimization

# Current Trend and Future Directions in NLP

LLM
- Rise of Large-scale transformer models has significantly improved NLP capabilities
	- Few-shot and zero-shot learning, reducing need for extensive labeled datasets
	- Transfer Learning: pre-trained on large corpora, can be fine tuned for specific tasks.

Explainable and Fair NLP
- Making NLP models more transparent, interpretable and fair

NLP for Low-resource Languages
- Multilingual representation learning to improve NPL performance in underrepresented languages.

and thats all.