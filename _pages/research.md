---
title: "IMMD Lab - Research"
layout: textlay
excerpt: "IMMD Lab -- Research"
sitemap: false
permalink: /research/
---

# Research

Our overall research goal is to construct robust and comprehensive **process-structure-property relationships** to conduct systematic process and materials design for advanced manufacturing processes. To do so, we develop and integrate novel multiscale multiphysics simulation models and physics-informed machine learning models at different time- and length-scales.

## Multiscale Multiphysics Modeling and Simulation
Simulation becomes an important tool to enable us to understand rapid solidification in metal additive manufacturing given the limitations of experimental techniques for in-situ measurement. A mesoscale multiphysics simulation model, called **phase-field and thermal lattice Boltzmann method (PF-TLBM)** was developed with simultaneous considerations of heterogeneous nucleation, solute transport, heat transfer, fluid dynamics, and phase transition. The simulation can reveal the complex dynamics of rapid solidification in the melt pool, such as the effects of latent heat and cooling rate on dendritic morphology and solute distribution. 

<table><tr>
<!-- <td style="width:50%">
<iframe width="250" height="250"
src="{{ site.url }}{{ site.baseurl }}/images/research/Flow.mp4" 
frameborder="0" 
allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" 
allowfullscreen></iframe></td> -->
<td style="width:50%">
<img src="{{ site.url }}{{ site.baseurl }}/images/research/Ti64.jpg" height="250" />
</td>
<td style="width:50%">
<img src="{{ site.url }}{{ site.baseurl }}/images/research/AlSi10Mg.jpg" height="250" />
</td>
</tr></table>

## Physics-Informed Machine Learning
Physics-informed machine learning has been considered to alleviate the issue of data sparsity in training machine learning models to solve engineering problems. In this approach, prior knowledge of physics is incorporated as constraints to guide the training of machine learning models. For instance, in the training of **physics-constrained neural networks (PCNNs)**, physical knowledge embodied as partial differential equations serves as the constraints and regularizes the training loss. The training is based on the weighted average of all losses from both data and physical constraint aspects. It has been shown that the required amount of training data can be significantly reduced by adding physical constraints if weights associated with the different losses for data and physical constraints are properly tuned. To systematically search the optimal weights of different losses, a **PCNN with minimax architecture (PCNN-MM)** was developed, where the training of the PCNN is formulated as solving a minimax problem instead of the traditional minimization.

![]({{ site.url }}{{ site.baseurl }}/images/research/PCNN.png){: style="height: 250px; margin: 0px  10px"}

## Optimization and Generative Design
To conduct systematic metal additive manufacturing process optimization, a hybrid physics-based data-driven process design framework was developed to establish reliable surrogates of process-structure relationships. The process design framework includes a mesoscale multiphysics simulation model to predict microstructure evolution, a physics-constrained neural network to construct the surrogate of the process-structure relationship, and Bayesian optimization for process design. The proposed framework is demonstrated by optimizing the initial temperature and cooling rate for the single dendritic growth of Ti-6Al-4V alloy during rapid solidification in metal AM so that the desired dendritic area and microsegregation level can be achieved. The Pareto front for dendritic growth was constructed with the **multi-objective Bayesian optimization** method. The proposed process design framework is generic and can be potentially applied in materials design and digital twins of metal AM.

<table><tr>
<td style="width:50%">
<img src="{{ site.url }}{{ site.baseurl }}/images/research/Research_Framework.png" height="250" />
</td>
<td style="width:50%">
<img src="{{ site.url }}{{ site.baseurl }}/images/research/Dendrites.png" height="250" />
</td>
<td style="width:50%">
<img src="{{ site.url }}{{ site.baseurl }}/images/research/BO.png" height="250" />
</td>
</tr></table>

