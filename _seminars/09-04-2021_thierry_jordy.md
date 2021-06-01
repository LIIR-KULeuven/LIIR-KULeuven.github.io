---
title: "April 9, 2021: By Thierry Deruyterre and Jordy Van Landeghem"
excerpt: "Problems and solutions for talking to self-driving cars by Thierry, and progress regarding Intelligent Automation for AI-driven Document Understanding by Jordy."
header:
  teaser: "assets/images/seminar_thierry_jordy.png"
#sidebar:
#  - nav: "jc-nav"
date: 2021-04-09
---


## Giving commands to self-driving cars

### **Thierry Deruteyrre**

In this presentation, Thierry will give an complete overview of the progress of his PhD regarding talking to self-driving cars. 
He will discuss several of the encountered tasks and issues in his work. This includes dataset creation, object location, uncertainty resolution and the upcoming tasks regarding path planning.  

## Intelligent Automation for AI-driven Document Understanding

### Jordy Van Landeghem

In the first part of the presentation, I will shortly introduce the global scope of my Ph.D. project "Intelligent Automation for AI-driven Document Understanding" and summarize the progress I have made in the first year of my Ph.D. The second part will focus on presenting work in progress: "Approximating Strong Calibration for Structured Prediction".

#### Short summary:
While machine learning models are continually improving, for most tasks they fail to achieve perfect predictive performance. Probabilistic predictive models address this concern by modeling probability distributions over possible targets.
In order to be a valuable tool in decision-making under uncertainty, it stands to reason that we want some statistical guarantees on the quality of probability distribution outputs.
Whereas research in statistics and machine learning has contributed different measures and tests for evaluating calibration, it has focused mainly on (i) classifiers predicting single [scalar] discrete or real outputs, and (ii) miscalibration of only the most confident prediction.
Many prototypical tasks in Natural Language Processing (NLP) involve sequential, structured output spaces (POS tagging, named entity recognition, machine translation, image captioning).
In this work, we present a calibration framework for structured prediction, which properly accounts for structure and interdependencies in potentially high-dimensional output spaces. We propose a theoretical quantity of strong, structured calibration from first principles, which we make tractable through approximations for real-life applications. We formulate hypothesis tests based on kernel two-sample measures and motivate empirical estimators for different Natural Language Processing tasks with increasingly complex structured output spaces.
Finally, I will reflect on the theoretical research process, share some best practices, and engage in a blueprinting session.
