---
layout: default
title: research themes
permalink: /research_themes
order: 1
---

<style>
.theme-card {
  background: #ffffff;
  border-left: 4px solid #4a5568;
  border-radius: 0 8px 8px 0;
  box-shadow: 0 1px 6px rgba(0,0,0,0.07);
  padding: 0.8rem 1.4rem 1rem 1.2rem;
  margin-bottom: 1.4rem;
}
.theme-card h3 {
  margin-top: 0.4rem;
  margin-bottom: 0.3rem;
}
.theme-card.color-1 { border-left-color: #5b6fa8; }
.theme-card.color-2 { border-left-color: #3a8c6e; }
.theme-card.color-3 { border-left-color: #b07830; }
.theme-card.color-4 { border-left-color: #a04040; }
.theme-card.color-5 { border-left-color: #2e7d8a; }
.misc-section {
  background: #ffffff;
  border-left: 4px solid #ccc;
  border-radius: 0 8px 8px 0;
  box-shadow: 0 1px 6px rgba(0,0,0,0.07);
  padding: 0.8rem 1.4rem 1rem 1.2rem;
}
</style>

## Research themes

My research focuses on understanding deep learning from an empirical and scientific perspective, aiming to derive actionable insights that can improve its practical application. Major themes include:

<div class="theme-card color-1" markdown="1">
### :mag: &nbsp; model interpretability via representation analysis
Deep learning works by transforming inputs into latent representations. Can we understand the information encoded in these representations?
- [Bhalla\*, Oesterling\*, **Srinivas**, Calmon & Lakkaraju (2024)](https://arxiv.org/abs/2402.10376): Representations of vision-language models can be decomposed into sparse linear combinations of semantic concept vectors, enabling dataset analysis and model editing
- [Bhalla, **Srinivas**, Ghandeharioun, Lakkaraju (2024)](https://arxiv.org/abs/2411.04430): We unify 4 representation analysis methods as "encoder-decoder" methods and evaluate them via control-based metrics
- [Li, **Srinivas**, Bhalla & Lakkaraju (2026)](https://arxiv.org/abs/2505.16004): Concept representations in sparse autoencoders are fragile — minimal input perturbations can substantially distort SAE-based interpretations without affecting the underlying model
</div>

<div class="theme-card color-2" markdown="1">
### :heavy_dollar_sign: &nbsp; data-centric machine learning
Model behaviour depends critically on training data. Can we identify datapoints and subsets that influence key model properties?
- [Ley, **Srinivas**, Zhang, Rusak & Lakkaraju (2024)](https://arxiv.org/abs/2410.09940): Generalized group data attribution extends arbitrary attribution algorithms to groups of training points, yielding ~50x speedups
- [Bordt, **Srinivas**, Boreiko & von Luxburg (2024)](https://arxiv.org/abs/2410.03249): Benchmark contamination in LLM pre-training does not automatically inflate scores — data seen early is often simply *forgotten* by end of training
</div>

<div class="theme-card color-3" markdown="1">
### :bar_chart: &nbsp; model interpretability via feature attribution
How can we identify which input features a model relies on, and verify that attribution methods are faithful to model behaviour?
- [**Srinivas** & Fleuret (2019)](https://papers.nips.cc/paper/2019/hash/80537a945c7aaa788ccfcdf1b99b5d8f-Abstract.html): ReLU network outputs decompose exactly as a sum of layerwise gradients, yielding a principled saliency method
- [**Srinivas** & Fleuret (2021)](https://openreview.net/forum?id=dYeAHXnpWJ4): Popular saliency methods can be unfaithful — producing attributions independent of the model
- [Han, **Srinivas** & Lakkaraju (2022)](https://arxiv.org/abs/2206.01254): 8 popular attribution methods unify under local linear approximations of non-linear models
- [**Srinivas\***, Bordt* & Lakkaraju (2023)](https://arxiv.org/abs/2305.19101) and [Bhalla*, **Srinivas\*** & Lakkaraju (2023)](https://arxiv.org/abs/2307.15007): Model robustness is a key factor in producing faithful attributions; we formalize ground-truth attributions via a signal-distractor decomposition
</div>

<div class="theme-card color-4" markdown="1">
### :muscle: &nbsp; alternate notions of model robustness
Training adversarially robust models is expensive. Are there alternate robustness definitions that are both meaningful and easier to train for?
- [**Srinivas\***, Matoba*, Lakkaraju & Fleuret (2022)](https://arxiv.org/abs/2206.07144): Smoothness (small Hessian) as a robustness proxy — competitive with adversarial training while maintaining accuracy and stable gradients
- [Han*, **Srinivas\*** & Lakkaraju (2024)](https://arxiv.org/abs/2307.13885): Average-case robustness as an alternative to worst-case adversarial robustness, with efficient estimation methods
- [**Srinivas\***, Bordt* & Lakkaraju (2023)](https://arxiv.org/abs/2305.19101): Off-manifold robustness — robustness only to perturbations of irrelevant "distractor" features, characteristic of Bayes-optimal predictors
</div>

<div class="theme-card color-5" markdown="1">
### :recycle: &nbsp; computational efficiency of deep models
How can we eliminate redundant neurons or weights in a pre-trained model while preserving performance?
- [**Srinivas**, Kuzmin, Nagel, van Baalen, Skliar, Blankevoort (2022)](https://openaccess.thecvf.com/content/CVPR2022W/ECV/html/Srinivas_Cyclical_Pruning_for_Sparse_Neural_Networks_CVPRW_2022_paper.html): Cyclical sparsity schedules that alternate between pruning and unpruning yield state-of-the-art sparse networks
- [**Srinivas** & Babu (2015)](http://arxiv.org/abs/1507.06149): Duplicate neurons in pre-trained models can be identified and removed without accuracy loss via a simple "surgery" step
- [**Srinivas** & Babu (2016)](http://www.bmva.org/bmvc/2016/papers/paper104/index.html) and [**Srinivas**, Subramanya & Babu (2017)](https://arxiv.org/abs/1611.06694): Trainable binary gates on neurons/weights enable automatic pruning during training
</div>

<div class="misc-section" markdown="1">
Some other projects I have worked on:
- **gradient-based knowledge distillation**: [**Srinivas** & Fleuret (2018)](http://proceedings.mlr.press/v80/srinivas18a.html): Knowledge distilled from teacher to student by matching gradients, improving sample efficiency
- **certified robustness to LLM attacks**: [Kumar, Agarwal, **Srinivas**, Li, Feizi & Lakkaraju (2024)](https://arxiv.org/abs/2309.02705): Certified defense against a class of adversarial LLM attacks via an "erase-and-check" procedure
</div>

<br>


