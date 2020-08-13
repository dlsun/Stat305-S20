---
mathjax: true
title: STAT 305 Summer 2020
---

{% include mathjax.html %}

# Final Project Info

## Overview

Your task is to prepare two lectures exploring estimation in two scenarios. You can work with a partner on this project. 
The project is due on Friday, August 21. On that day, there will be optional final presentations. You may attend the 
final presentation session or submit a pre-recorded video.

## Task

Consider the following scenarios:

1. $X$ is $\text{Binomial}(n, p)$. Consider the following estimators of the parameter $p$:
    - $\hat p_1 = \frac{X}{n}$
    - $\hat p_2 = \frac{X + 2}{n+4}$
    - $\hat p_3 = \sqrt{\frac{X(X-1)}{n(n-1)}}$ (This estimator is motivated by [Lesson 24](https://dlsun.github.io/probability/lotus.html), 
    where we showed that $E[X(X-1)] = n(n-1)p^2$. Equating $X(X-1)$ to this expected value and solving for $p$ yields this estimator.)
    - The MLE is one of these estimators. Which one?
2. $X_1, X_2, \ldots, X_n$ are i.i.d. $\text{Normal}(\mu, \sigma=\sqrt{\mu})$. (That is, the variance equals the mean: $\sigma^2 = \mu$.) 
Consider the following estimators of the parameter $\mu$:
    - $\hat\mu_1 = \bar X = \frac{\sum_{i=1}^n X_i}{n}$
    - $\hat\mu_2 = S^2 = \frac{\sum_{i=1}^n (X_i - \bar X)^2}{n-1}$
    - $\hat\mu_{\text{MLE}} = $ ???
    
For each scenario:

1. Derive the maximum likelihood estimator (MLE) for the parameter.
2. Calculate the bias, variance, and mean-squared error of each estimator (as a function of the unknown parameter). Graph these functions. 
Which estimator is best? (For some estimators, you will be able to calculate the bias, variance, and MSE exactly. For others, 
you have to use simulation.)
3. If possible, form a 95% confidence interval for each parameter.
    
## Deliverables

1. A lesson, which can take many forms (e.g., Colab notebook, slides, video, website).
2. Your presentation of the lesson, which you can do in the presentation session or record as a video. (Note: If your lesson 
itself is a video, you may skip this step.)

## Grading

Grading will be based on correctness, clarity, and aesthetics.
