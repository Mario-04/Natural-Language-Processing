---
tags:
  - Lecture
  - FirstPass
Created: 2025-02-20
aliases:
  - NLP_Lecture_3
---
Lecture slides here [[Lecture 3 - Vector Semantics & Embeddings]]

Extra lectures on Fridays for things like Transformers

# Content
1. Word meaning
2. TF-IDF
3. Word2Vec Basics
	1. Word2Vec training
	2. Evaluating Word2Vec Embeddings

# Word meaning: What do words mean?
- n-gram: count probability to represent meaning 
	- count index
	- Drawback: capturing words regularity instead of meaning
- Logic for meaning:
	- **Predicate logic**
- Captures structure but nnot words. Bank (finance) vs. Bank (riverbank)

## Lexical Semantics
- Semantic study of word meanings 
- 2 fundamental questions:

## Lemmas and senses
mouse (N) <- lemma
1. any of numerous small rodents <- sense
2. a hand-operated device that controls cursor <- sense

## Synonyms
Not all synonyms are the interchangeable
- my big sister / my large sister

relationship of approximate or rough synonymy 

## Similarity
Sharing elements of meaning
- car / bicycle
- horse / cow

## Relatedness
- coffe / tea -> similar
- coffee / cup -> related, not similar

## Semantic fields
Hospitals
- surgeon, scalpel, nurse 
Household

## Sentiment
- the intent of the person, what they are trying to say.
Affective meanings

# Vector semantics

standard way to represent word meaning in multidimensional space to accommodate features of words. meaning can be defined in different ways.
- emergently, we have words with meaning imbedded
- vectors: representing words -> <mark style="background: #D2B3FFA6;">embeddings</mark>
- <mark style="background: #CACFD9A6;">hyperparameters</mark> used to tune amount of <mark style="background: #D2B3FFA6;">dimensions</mark>

Idea: represent words by context (neighbouring words)

Distributional hypothesis
- meaning given by words that appear together frequently

e.g. the tella example from the lecture slides
- you can find the word you need by looking at context


# Cosine for similarity

- im helping rob pick a laptop

weighted prepresentation along with frequency
give words that are too frequent a penalty

Term Frequency (tf)
Inverse Document Frequency (idf)
TF-IDF = tf x idf

# Sparse vs dense vectors


# Word2Vec

Input: Large text corpora V, d
- V: pre-defined vocab
- d: dimensions of word vectors
- Text Corpora:
	- Wikipedia + Gigaword 5: 6B
	- Twitter: 27B
	- Common Crawl: 840B

(Mikolov et al 2013a)

Skip-gram: predict surrounding words bases on given word

one-hot encoding 

soft-max for something else

## Skip-gram
- large corpus
- use each word to predict other words in context
- <mark style="background: #ABF7F7A6;">Context</mark>
then our product is a weight matrix that embeds the word meaning
compute one word and move to the right

## Objective function
Maximise predictive accuracy 
Minimize objective function

Very in depth stuff

Need to go over at home

Intrinsic vs. extrinsic.