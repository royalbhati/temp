---
layout: post
title: "What is L1 and L2 regularization?!"
date: 2018-09-29 16:32:20 +0300
description: L1 and L2 Norms . # Add post description (optional)
img:  # Add image post (optional)
---

First of all **What is Regularization?**

Regularization has a different meanings in different contexts but in machine learning this term is is used to prevent the model from overfitting.

## How does model overfits?

There are various reasons which can lead to overfitting like
  * Small dataset
  * Large number of features
  * Complex Model (High degree polynomial in Regression)
  
 So Regularization helps in overcoming the over-fitting and there are various techniques of regularization but we'll talk about the two of the famous ones.
 
 # L1 Regularization
 
It places constraints on the vector W of “weights”.
When you hear about L1 regularization it means that the L1-norm [1] of the vector  is being constrained.
The L1-norm of the vector is defined in the following way:
  W<sub>r= \sum

\begin{equation}

$\text{S}_1(N) = \sum_{p=1}^N \text{E}(p)$
$ \sum_{\forall i}{x_i^{2}} $

\end{equation}

$ \sum_{\forall i}{x_i^{2}} $

