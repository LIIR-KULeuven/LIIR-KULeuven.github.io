---
title: "September 2, 2021: By Christos Theodoropoulos"
excerpt: "Imposing Relation Structure in Language-Model Embeddings
Using Contrastive Learning"
header:
  teaser: 
#sidebar:
#  - nav: "jc-nav"
date: 2021-09-02
---

## Imposing Relation Structure in Language-Model Embeddings
Using Contrastive Learning

### Christos Theodoropoulos

#### Abstract:
Abstract:
Though language model text embeddings have revolutionized NLP research, their ability to capture high-level semantic information, such as relations between entities in text, is limited. We propose a novel contrastive learning framework that trains sentence embeddings to encode the relations in a graph structure. Given a sentence (unstructured text) and its graph, we use contrastive learning to impose relation-related structure on the token level representations of the sentence obtained with a CharacterBERT (El Boukkouri et al., 2020) model. The resulting relation-aware sentence embeddings achieve near to state-of-the-art results on the relation extraction task using only a simple KNN classifier, thereby demonstrating the success of the proposed method. Additional visualization by a tSNE analysis shows the effectiveness of the learned representation space compared to baselines. Furthermore, we show that we can learn a different space for named entity recognition, again using a contrastive learning objective, and demonstrate how to successfully combine both representation spaces in an entity-relation task.
