---
title: "April 15th, 2022: By Nathan Cornille and Victor Milewski"
excerpt: "Critical Analysis of Deconfounded Pretraining to Improve Visio-Linguistic Models; Finding Structural Knowledge in Multimodal-BERT"
header:
  teaser: assets/images/victor_nathan.jpg
#sidebar:
#  - nav: "jc-nav"
date: 2022-04-15
---

## Critical Analysis of Deconfounded Pretraining to Improve Visio-Linguistic Models

### Nathan Cornille

#### Abstract:
Abstract:
An important problem with many current visio-linguistic models is that they often depend on spurious correlations. A typical example of a spurious correlation between two variables is one that is due to a third variable causing both (a “confounder”). Recent work has addressed this by adjusting for spurious correlations using a technique of deconfounding with automatically found confounders. We will refer to this technique as AutoDeconfounding. This article dives more deeply into AutoDeconfounding, and surfaces a number of issues of the original technique. First, we evaluate whether its implementation is actually equivalent to deconfounding. We provide an explicit explanation of the relation between AutoDeconfounding and the underlying causal model on which it implicitly operates, and show that additional assumptions are needed before the implementation of AutoDeconfounding can be equated to correct deconfounding. Inspired by this result, we perform ablation studies to verify to what extent the improvement on downstream visio-linguistic tasks reported by the works that implement AutoDeconfounding is due to AutoDeconfounding, and to what extent it is specifically due to the deconfounding aspect of AutoDeconfounding. We evaluate AutoDeconfounding in a way that isolates its effect, and no longer see the same improvement. We also show that tweaking AutoDeconfounding to be less related to deconfounding does not negatively affect performance on downstream visio-linguistic tasks. Furthermore, we create a human-labeled ground truth causality dataset for objects in a scene to empirically verify whether and how well confounders are found. We show that some models do indeed find more confounders than a random baseline, but also that finding more confounders is not correlated with performing better on downstream visio-linguistic tasks. Finally, we summarize the current limitations of AutoDeconfounding to solve the issue of spurious correlations and provide directions for the design of novel AutoDeconfounding methods that are aimed at overcoming these limitations.

[Full paper](https://www.frontiersin.org/articles/10.3389/frai.2022.736791/full)

## Finding Structural Knowledge in Multimodal-BERT

### Victor Milewski

#### Abstract:
Abstract:
Knowledge-based viIn this work, we investigate the knowledge learned in the embeddings of multimodal-BERT models. More specifically, we probe their capabilities of storing the grammatical structure of linguistic data and the structure learned over objects in visual data. To reach that goal, we first make the inherent structure of language and visuals explicit by a dependency parse of the sentences that describe the image and by the dependencies between the object regions in the image, respectively. We call this explicit visual structure the \textit{scene tree}, that is based on the dependency tree of the language description. Extensive probing experiments show that the multimodal-BERT models do not encode these scene trees.Code available at [this https URL](https://github.com/VSJMilewski/multimodal-probes).

[Full paper](https://arxiv.org/abs/2203.09306)

