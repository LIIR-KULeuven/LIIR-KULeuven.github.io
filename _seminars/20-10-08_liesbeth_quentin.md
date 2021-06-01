---
title: "October 8, 2020: By Liesbeth Allein and Quentin Meeus"
excerpt: "In-depth review about Checkworthiness, by Liesbeth and how to leverage BERT models to generate speech features holding semantic information, by Quentin."
header:
#  image: https://www.cebap.org/storage/cebap/fact-fake.jpg
  teaser: https://www.cebap.org/storage/cebap/fact-fake.jpg
#sidebar:
#  - nav: "jc-nav"
date: 2020-10-08
---


## Checkworthiness in Automatic Claim Detection Models: Definitions and Analysis of Datasets

### Liesbeth Allein


Public, professional and academic interest in automated fact-checking has drastically increased over the past decade, 
with many aiming to automate one of the first steps in a fact-check procedure: the selection of so-called checkworthy claims. 
However, there is little agreement on the definition and characteristics of checkworthiness among fact-checkers, 
which is consequently reflected in the datasets used for training and testing checkworthy claim detection models. 
After elaborate analysis of checkworthy claim selection procedures in fact-check organisations and analysis 
of state-of-the-art claim detection datasets, checkworthiness is defined as the concept of having a spatiotemporal 
and context-dependent worth and need to have the correctness of the objectivity it conveys verified. 
This is irrespective of the claim’s perceived veracity judgement by an individual based on prior knowledge and beliefs. 
Concerning the characteristics of current datasets, it is argued that the data is not only highly imbalanced and noisy, 
but also too limited in scope and language. Furthermore, we believe that the subjective concept of checkworthiness 
might not be a suitable filter for claim detection. (https://arxiv.org/pdf/2008.08854.pdf) 

## Speech to Semantics: A representation learning approach

### Quentin Meeus


In this work, we are trying to leverage the performance of pretrained NLP models such as BERT to learn to generate 
speech features that hold semantic information. We are using a transformer encoder-decoder network in a student / teacher 
framework to predict the representations produced by DistilBERT. The model is trained on the Corpus Gesproken Nederlands. 
We evaluate the trained features on a speech-to-intent task with two unobserved datasets.