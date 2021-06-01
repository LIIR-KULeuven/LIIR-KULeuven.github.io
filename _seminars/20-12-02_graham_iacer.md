---
title: "December 2, 2020: By Graham Spinks and dr. Iacer Calixto"
excerpt: "Convolutional Generation of Textured 3D Meshes by Graham Spinks, and a guest talk by dr Iacer Calixto"
header:
#  image: https://cvssp.org/faceweb/3dmm/MorphDemoW0.png
  teaser: https://cvssp.org/faceweb/3dmm/MorphDemoW0.png
#sidebar:
#  - nav: "jc-nav"
date: 2020-11-05
---


## Convolutional Generation of Textured 3D Meshes

### Dario Pavllo, **Graham Spinks**, Thomas Hofmann, Marie-Francine Moens, Aurelien Lucchi

This paper by Graham Spinks made in collaboration with ETH Zurich was accepted as an oral presentation at NeurIPS. 

[arxiv]({{ "https://arxiv.org/abs/2006.07660" | url }})<br />
[NeurIPS]({{ "https://nips.cc/Conferences/2020/ScheduleMultitrack?event=18727" | url }})

#### Abstract:
While recent generative models for 2D images achieve impressive visual results, 
they clearly lack the ability to perform 3D reasoning. 
This heavily restricts the degree of control over generated objects as well as the possible applications of such models. 
In this work, we bridge this gap by leveraging recent advances in differentiable rendering. 
We design a framework that can generate triangle meshes and associated high-resolution texture maps, 
using only 2D supervision from single-view natural images. 
A key contribution of our work is the encoding of the mesh and texture as 2D representations, 
which are semantically aligned and can be easily modeled by a 2D convolutional GAN. 
We demonstrate the efficacy of our method on Pascal3D+ Cars and CUB, both in an unconditional setting and in settings 
where the model is conditioned on class labels, attributes, and text. Finally, we propose an evaluation methodology 
that assesses the mesh and texture quality separately.

## Invited Talk

### Dr. Iacer Calixto

Iacer Calixto is a postdoctoral research fellow at the Center for Data Science at New York University where he works with Kyunghyun Cho. 
His scientific interests include natural language processing, understanding, and generation, 
how human languages interact with our visual perceptions and representations, and how these interact with and are grounded by the external world.

He has experience in and many publications regarding the use of visual information for natural language models, and how to combine these different modalities.
Currently, he is working on the IMAGINE project (Improving Multi-modal lAnguage Generation wIth world kNowledgE) funded by the Marie Skwodówska-Curie Global Fellowship.

[Personal page: https://iacercalixto.github.io/]({{ "https://iacercalixto.github.io/" | url }})<br />
