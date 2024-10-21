---
layout: default
title: research themes
permalink: /oresearch_themes
order: 1
---

## **Research themes** 

I am broadly interested in understanding deep learning from both an empirical and scientific perspective, with a focus on deriving actionable insights. Specifically, I am interested in the following themes:

<br>

### :mag: &nbsp; **model interpretability via representation analysis**
Deep learning works by transforming inputs to latent representations. Can we understand and describe the information stored in these latent representations?
- In [Bhalla\*, Oesterling\*, **Srinivas**, Calmon & Lakkaraju (2024)](https://arxiv.org/abs/2402.10376), we find that representations of vision-language models can be written in terms of a sparse linear combination of "concept" vectors that denote individual high-level semantic concepts; which we can use for dataset analysis and model editing

<br>

### :heavy_dollar_sign: &nbsp; **data attribution & valuation**
Behaviour of machine learning models depend critically on the datasets used to train them. Can we identify critical datapoints / data subsets that influence key model properties? 
- In [Ley, **Srinivas**, Zhang, Rusak & Lakkaraju (2024)](https://arxiv.org/abs/2410.09940) (caution: early pre-print!) we propose "generalized group data attribution", a framework to extend arbitrary data attribution algrorithms to efficiently attribute to groups of training data points, yielding upto ~50x attribution speedups

<br>

### :bar_chart: &nbsp;  **model interpretability via feature attribution**  
Feature attributions are a popular means to interpret model behaviour in terms of the most important input features a model "pays attention to". However, these methods have been found to be inaccurate, and sometimes conceptually ill-defined. How can we ensure that feature attributions accurately reflects model behavior in a meaningful, well-defined way?

- In [**Srinivas** & Fleuret (2021)](https://openreview.net/forum?id=dYeAHXnpWJ4), we show that popular computer vision-based feature attribution approaches are unfaithful to models, in that they produce attributions completely independent of model behaviour
- In [Han, **Srinivas** & Lakkaraju (2022)](https://arxiv.org/abs/2206.01254), we unify 8 popular feature attribution methods via local linear approximations of non-linear models
- In [**Srinivas\***, Bordt* & Lakkaraju (2023)](https://arxiv.org/abs/2305.19101) and [Bhalla*, **Srinivas\*** & Lakkaraju (2023)](https://arxiv.org/abs/2307.15007), we identify model robustness as a key factor in producing faithful feature attributions. To quantify faithfulness, we define a notion of ground-truth feature attributions in terms of the signal a feature carries about the predicted label, formalized via a "signal-distractor" decomposition

<br>

### :muscle: &nbsp; **alternate notions of model robustness** 
Training adversarially robust models is hard. Are there alternate definitions of robustness that are both practically meaningful, and easier to train for? 
- In [**Srinivas\***, Matoba*, Lakkaraju & Fleuret (2022)](https://arxiv.org/abs/2206.07144), we propose an efficient algorithm to train deep models that are smooth, in the sense that they have a small Hessian everywhere. The resulting smooth models are competitive with adversarially robust models, have stable gradients, and maintain predictive accuracy
- In [Han*, **Srinivas\*** & Lakkaraju (2024)](https://arxiv.org/abs/2307.13885), we propose average-case robustness as an alternative to the worst-case adversarial robustness, and develop methods to efficient estimate this quantity
- In [**Srinivas\***, Bordt* & Lakkaraju (2023)](https://arxiv.org/abs/2305.19101), we introduce the concept of off-manifold robustness, where models are robust only to perturbations of irrelevant "distractor" features -- an aspect characteristic of Bayes Optimal predictors

<br>

### :recycle: &nbsp; **computational efficiency of deep models** 
Given a pre-trained deep model, how can we effectively identify and eliminate redundant neurons or weights while maintaining the model's performance?
- In [**Srinivas**, Kuzmin, Nagel, van Baalen, Skliar, Blankevoort (2022)](https://openaccess.thecvf.com/content/CVPR2022W/ECV/html/Srinivas_Cyclical_Pruning_for_Sparse_Neural_Networks_CVPRW_2022_paper.html), we propose a state-of-the-art approach to train sparse neural networks, via incorporating a cyclical sparsity schedule which alternates between pruning and "unpruning" weights
- In [**Srinivas** & Babu (2015)](http://arxiv.org/abs/1507.06149), we propose a simple algorithm to identify redundant duplicate neurons and remove them from pre-trained models, without incurring accuracy loss, via a "surgery" step
- In [**Srinivas** & Babu (2016)](http://www.bmva.org/bmvc/2016/papers/paper104/index.html) and [**Srinivas**, Subramanya & Babu (2017)](https://arxiv.org/abs/1611.06694), we propose an algorithm to automatically prune neurons / weights during training, but incorporating trainable multiplicative binary gates to neurons / weights

<br>

Apart from these broad themes, here are some cool miscellaneous projects I have worked on:
- **gradient-based knowledge distillation**: In [**Srinivas** & Fleuret, 2018](http://proceedings.mlr.press/v80/srinivas18a.html), we propose to distill knowledge from a "teacher" to a "student" model by matching their gradients, which helps improve the sample efficiency of distillation
- **gradient-based model representations**: In [**Srinivas** & Fleuret, 2019](https://papers.nips.cc/paper/2019/hash/80537a945c7aaa788ccfcdf1b99b5d8f-Abstract.html), we observe that the outputs of ReLU NNs can be written exactly as the sum of layerwise gradients. We use this fact to define gradient-based saliency maps for such models

<br>


