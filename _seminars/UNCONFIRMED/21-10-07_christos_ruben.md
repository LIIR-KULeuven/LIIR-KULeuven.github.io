---
title: "October 7, 2021: By Christos Theodoropoulos and Ruben Cartuyvels"
excerpt: "Imposing Relation Structure in Language-Model Embeddings Using Contrastive Learning; Discrete and Continuous Representations and Processing in Deep Learning"

"
header:
  teaser: assets/images/christos_seminar.png
#sidebar:
#  - nav: "jc-nav"
date: 2021-10-07
---

## Imposing Relation Structure in Language-Model Embeddings Using Contrastive Learning

### Christos Theodoropoulos

#### Abstract:
Abstract:
Though language model text embeddings have revolutionized NLP research, their ability to capture high-level semantic information, such as relations between entities in text, is limited. We propose a novel contrastive learning framework that trains sentence embeddings to encode the relations in a graph structure. Given a sentence (unstructured text) and its graph, we use contrastive learning to impose relation-related structure on the token level representations of the sentence obtained with a CharacterBERT (El Boukkouri et al., 2020) model. The resulting relation-aware sentence embeddings achieve near to state-of-the-art results on the relation extraction task using only a simple KNN classifier, thereby demonstrating the success of the proposed method. Additional visualization by a tSNE analysis shows the effectiveness of the learned representation space compared to baselines. Furthermore, we show that we can learn a different space for named entity recognition, again using a contrastive learning objective, and demonstrate how to successfully combine both representation spaces in an entity-relation task.

## Discrete and Continuous Representations and Processing in Deep Learning

### Ruben Cartuyvels
#### Abstract:
Abstract:
Discrete and continuous representations of content (e.g., of language or images) have interesting properties to be explored for the understanding of or reasoning with this content by machines. This position paper puts forward our opinion on the role of discrete and continuous representations and their processing in the deep learning field. Current neural network models compute continuous- valued data. Information is compressed into dense, distributed embeddings. By stark contrast, humans use discrete symbols in their communication with language. Such symbols represent a compressed version of the world that derives its meaning from shared contextual information. Additionally, human reasoning involves symbol manipulation at a cognitive level, which facilitates abstract reasoning, the composition of knowledge and understanding, generalization and efficient learning. Motivated by these insights, in this paper we argue that combining discrete and continuous representations and their processing will be essential to build systems that exhibit a general form of intelligence. We suggest and discuss several avenues that could improve current neural networks with the inclusion of discrete elements to combine the advantages of both types of representations.
