---
title: "November 5, 2020: By Nathan Cornille and Victor Milewski"
excerpt: "Feedback and tips on using brain-inspired anticipation in Transformers, by Nathan 
and Are scene graphs good enough for image captioning, by Victor"
header:
#  image: https://bethpascoe.com/wp-content/uploads/2018/01/anticipation-08-1080x675.jpg
  teaser: https://bethpascoe.com/wp-content/uploads/2018/01/anticipation-08-1080x675.jpg
#sidebar:
#  - nav: "jc-nav"
date: 2020-11-05
---


## Distributed Internal Regression Transformer (DIRT)

### Nathan Cornille

Context: this poster presentation was originally going to take place in March, but got moved to November due to Covid.
It's about a project that in March was in it's beginning stage, but by now has been stopped, 
as I didn't get the results I wanted and didn't see a clear path forward.
My intentions with the presentation are
 - Teach the audience "lessons learned" that are hopefully useful 
 - Possible get input from a knowledgeable audience on a new way forward
 - Earn the right to be there (as the KUL is still paying a fee for it, even though it's virtual :P)

Impressive scores on general-purpose Natural Language Understanding (NLU) benchmarks such as GLUE and SuperGLUE show how NLU has improved remarkably in recent years.
However, there is still a gap between machine and human performance.
This work is designed to decrease that gap by extending Transformers, the current state-of-the-art models, with "anticipation": a brain-inspired inner-self-prediction objective. In addition to current self-supervised objectives, the proposed model predicts masked-out internal activations, using other activations that are respectively adjacent and top-down.
To prevent the model from cheating by making internal activations trivial to predict, we employ contrastive learning.

Besides addressing the issue of cheating, contrastive learning has been shown to induce desirable 'slow features', providing a further intuition for how the extended objective can improve representation quality.
We compare a number of variations of our model, and evaluate extensively on SuperGLUE.
Unfortunately, our added anticipation objective does not improve performance.
Reflection suggests two paths forward:
 1. Develop a clear view of how anticipation can benefit current ML models. Induction of slow features is not the answer, as they are a consequence of contrasting, not of anticipation. If anticipation's main utility in the brain is to do credit assignment for example, it would not complement the current tools of machine learning, as backprop achieves that goal already.
 2. If we have reason to believe anticipation does complement current machine learning tools: investigate replacing contrasting by a more biologically plausible technique to prevent cheating, for example a minmax-type objective.

Extra reading: [On Intelligence](https://papers.harvie.cz/unsorted/Jeff%20Hawkins%20-%20On%20Intelligence.pdf) (boek van Jeff Hawkins)
## Are scene graphs good enough to improve Image Captioning?

### Victor Milewski

Many top-performing image captioning models rely solely on object features computed with an object detection model 
to generate image descriptions. However, recent studies propose to directly use scene graphs to introduce information 
about object relations into captioning, hoping to better describe interactions between objects. 
In this work, we thoroughly investigate the use of scene graphs in image captioning. We empirically study whether 
using additional scene graph encoders can lead to better image descriptions and propose a conditional graph attention network (C-GAT), 
where the image captioning decoder state is used to condition the graph updates. 
Finally, we determine to what extent noise in the predicted scene graphs influence caption quality. 
Overall, we find no significant difference between models that use scene graph features and models that only use 
object detection features across different captioning metrics, which suggests that existing scene graph generation models 
are still too noisy to be useful in image captioning. Moreover, although the quality of predicted scene graphs is very low in general, 
when using high quality scene graphs we obtain gains of up to 3.3 CIDEr compared to a strong Bottom-Up Top-Down baseline.
