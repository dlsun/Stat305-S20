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
    - $\hat\mu_{\text{MLE}} = $ ??? (The algebra for deriving the MLE is messy, but 
    the answer ends up being quite simple in the end. If you use Wolfram Alpha, it might 
    help to first simplify the expressions by hand, letting $a = \sum X_i$ and $b = \sum X_i^2$. 
    You should end up having to solve $\mu^2 + \mu + c = 0$, where $c$ is some expression 
    that depends on $X_1, ..., X_n$, which you can do using the quadratic formula.)
    
For each scenario:

1. Derive the maximum likelihood estimator (MLE) for the parameter.
2. Calculate the bias, variance, and mean-squared error of each estimator (as a function of the unknown parameter). Graph these functions. 
Which estimator is best? (For some estimators, you will be able to calculate the bias, variance, and MSE exactly. For others, 
you have to use simulation.)
3. Explain how you would construct a 95% confidence interval for each parameter. Evaluate the coverage probability of this interval 
using a simulation study.
    
## Deliverables

1. A lesson, which can take many forms (e.g., Colab notebook, slides, video, website). You may assume that the 
audience has taken STAT 305, but they may not have studied these particular scenarios. So you don't need to spend 
time defining "maximum likelihood" or "bias". However, it is still helpful if you connect your calculations to the 
definitions and interpret your calculations in context. In other words, it may be a good idea to remind the 
listener about definitions, but there is no need to teach the concept from scratch.
2. Your presentation of the lesson, which you can do in the presentation session or record as a video. (Note: If your lesson 
itself is a video, you may skip this step.)

## Grading

Grading will be based on the following rubric:

- Correctness (100 points): 50 points for each scenario, based on...
    - Calculation of MLE
    - Graph of the bias, variance and MSE of the three estimators, either by calculation or by simulation
    - Construct a reasonable confidence interval and evaluate its coverage probability in a simulation
    - It is possible to go above and beyond and earn extra credit, if you do additional work related to these scenarios.
- Clarity (100 points)
    - Are topics ordered in a logical way?
    - Are the verbal explanations clear and concise?
    - Does the lesson strike the right balance of equations, text, and graphics? 
    (All three are necessary. But too much of one is not desirable.)
- Aesthetics and Presentation (100 points)
    - Does the lesson capture the listener's interest?
    - Is the lesson visually appealing?
    - Is technical content (e.g., equations) formatted in a way that is easy for readers to read?
    - For group projects, both partners should talk equally in the presentation. 
    (It is not okay to have one person present one scenario and the other person present the other.) 
    One suggestion is to frame the presentation as a dialogue or conversation.
