---
title: "March 3, 2022: By Mingxiao Li and Damien Sileo"
excerpt: "Dynamic Key-value Memory Enhanced Multi-step Graph Reasoning for Knowledge-based Visual Question Answering; Zero-Shot Recommendations as Language Modeling"
header:
  teaser: assets/images/mingxiao_damien_seminar.png
#sidebar:
#  - nav: "jc-nav"
date: 2022-03-03
---

## Dynamic Key-value Memory Enhanced Multi-step Graph Reasoning for Knowledge-based Visual Question Answering

### Mingxiao Li

#### Abstract:
Abstract:
Knowledge-based visual question answering (VQA) is a vision-language task that requires an agent to correctly answer image-related questions using knowledge that is not presented in the given image. It is not only a more challenging task than regular VQA but also a vital step towards building a general VQA system.  Most existing knowledge-based VQA systems process knowledge and image information similarly and ignore the fact that the knowledge base (KB) contains complete information about a triplet, while the extracted image information might be incomplete as the relations between two objects are missing or wrongly detected. In this paper, we propose a novel model named dynamic knowledge memory enhanced multi-step graph reasoning (DMMGR), which performs explicit and implicit reasoning over a key-value knowledge memory module and a spatial-aware image graph, respectively. Specifically, the memory module learns a dynamic knowledge representation and generates a knowledge-aware question representation at each reasoning step. Then, this representation is used to guide a graph attention operator over the spatial-aware image graph. Our model achieves new state-of-the-art accuracy on the KRVQR and FVQA datasets. We also conduct ablation experiments to prove the effectiveness of each component of the proposed model.

## Zero-Shot Recommendations as Language Modeling

### Damien Sileo
#### Abstract:
Abstract:
Recommendation is the task of ranking items (e.g. movies or products) according to individual user needs. Current systems rely on collaborative filtering and content-based techniques, which both require structured training data. We propose a framework for recommendation with off-the-shelf pretrained language models (LM) that only used unstructured text corpora as training data. If a user u liked "Matrix" and "Inception", we construct a textual prompt, e.g. "Movies like Matrix, Inception, <m>" to estimate the affinity between u and m with LM likelihood. We motivate our idea with a corpus analysis, evaluate several prompt structures, and we compare LM-based recommendation with standard matrix factorization trained on different data regimes.
