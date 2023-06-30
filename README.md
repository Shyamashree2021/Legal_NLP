# Introduction
This repository contains implementations and datasets made available in the following papers :

- Legal Case Document Summarization: Extractive and Abstractive Methods and their Evaluation accepted at AACL-IJCNLP 2022.
- A Comparative Study of Summarization Algorithms Applied to Legal Case Judgments accepted at ECIR 2019.
We provide the code base of various Extractive and Abstractive summarization algorithms applied to legal case documents. We also provide three summarization datasets from the Indian and UK Supreme Court case documents.

## Abstractive Summarization
we have used the legal Pegasus X-Sum Model. Pre-training with Extracted Gap-sentences for Abstractive Summarization Sequence-to-sequence model uses rule-based information extraction component, subject matter selection components, rules and several patterns for sentence creation. All abstraction techniques deal with specific topics and subgroups.
### What is legal Peagasus ?
In the field of natural language processing (NLP), the term "Pegasus" refers to a specific model developed by OpenAI. Pegasus is a transformer-based model specifically designed for text summarization tasks.
It was introduced in a research paper titled 
 "https://arxiv.org/abs/1912.08777#:~:text=PEGASUS%3A%20Pre%2Dtraining%20with%20Extracted%20Gap%2Dsentences%20for%20Abstractive%20Summarization"
### Summarization Methods
Scripts to fine-tune following model
- Legal-Pagasus
Model is available on https://huggingface.co/google/pegasus-xsum

### Requirements
- transformers 4.12.3
- pytorch 1.10
### Import and Load Model
- Import dependencies from transformers
- Load tokenizer
- Load model

## Extractive Summarization
We have used MMR for extractive summarization in our experiment .Maximal Marginal Relevance considers the similarity of keywords/keyphrases with the document, along with the similarity of already selected keywords and keyphrases. This results in a selection of keywords that maximize their within diversity with respect to the document. The Maximal Marginal Relevance (MMR) criterion strives to reduce redundancy while maintaining query relevance in re- ranking retrieved documents and in selecting appropriate passages for text summarization.
Summarization Methods
- MMR
### what is MMR ?
In the context of extractive summarization in natural language processing (NLP), "MMR" can refer to "Maximal Marginal Relevance." MMR is a method used to improve the diversity of the selected sentences in the summary while maintaining their relevance to the source document.
### Requirements
- spacy = 2.2.3
- nltk = 3.5
- sklearn = 0.21.3
- tqdm


