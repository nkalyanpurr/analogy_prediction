# Analogical reasoning via word vectors

- [Analogical reasoning via word vectors](#analogical-reasoning-via-word-vectors)
  - [Introduction](#introduction)
  - [Running](#running)
  - [Results](#results)
  - [Sources](#sources)

## Introduction

The technique of representing words as vectors has roots in the 1960s with the development of the [vector space model](https://en.wikipedia.org/wiki/Vector_space_model) for information retrieval. In 2000 Bengio et al. provided in a series of papers the "Neural probabilistic language models" to reduce the high dimensionality of words  representations in contexts by "learning a distributed representation  for words". From then on word embeddings become a very exciting area of research.

Word embedding is the collective name for a set of language modeling and feature learning techniques in natural language processing where words or phrases from the vocabulary are mapped to vectors of[real numbers. Conceptually it involves a mathematical embedding from a space with many dimensions per word to a continuous vector space with a much lower dimension.

Much later, Mikolov et al. (see following note) proposed that simple algebraic operations could be applied to embeddings to find an analogy prediction. The notebook in this repository tries to do the same using word2vec vectors trained on the Google news dataset and GloVe vectors trained on the Common Crawl dataset.

> Mikolov,  T.,  Sutskever,  I.,  Chen,  K.,  Corrado,  G.  S.,  &  Dean,  J.  (2013). Distributed  representations  of  words  and  phrases  and  their  compositionality. In Advances in neural information processing systems (pp. 3111\-3119)

## Running

To run, you'll need 2 additional files -

- `GoogleNews-vectors-negative300.bin` - can be found [here](https://code.google.com/archive/p/word2vec/).
- `glove.840B.300d.txt` - can be found [here](https://nlp.stanford.edu/projects/glove/).

I've only run the notebook on a subset of the dataset, in the interest of saving time and computation resources.

## Results

On the train set -

```
word2Vec Accuracy =  64.76683937823834
Glove Accuracy =  61.20085339835416
```

On the test set -

```
word2Vec Accuracy =  66.66666666666667
Glove Accuracy =  33.333333333333336
```

## Sources

- Wikipedia article on word embeddings
- Material from ITCS 5111: Natural Language Processing