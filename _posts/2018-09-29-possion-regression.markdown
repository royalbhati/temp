---
layout: post
title: "What is Poisson and Negative Binomial Regression!"
date: 2018-09-29 16:32:20 +0300
description: These are generalized linear model forms of regression . # Add post description (optional)
img:  # Add image post (optional)
---

When I was working on a problem where target value was counts, I came across these two terms.

## What is Poisson Regression

**Poisson regression** is a generalized linear model form of regression analysis introduced by Siméon Denis Poisson in 1837 to support his work exploring the causes of wrongful criminal convictions. Poisson Regression, also referred to a log-linear model when working with categorical data, is now common in most analytical packages and is recommended wherever you need to model count data or construct contingency tables.

## When to use?

Poisson regression is intended for use in regression models that are used to predict numeric values, typically counts. Therefore, you should use this module to create your regression model only if the values you are trying to predict fit the following conditions:

* The response variable has a [Poisson distribution](https://en.wikipedia.org/wiki/Poisson_distribution).

  A Poisson distribution is a tool that helps to predict the probability of certain events from happening when you know         how often the event has occurred. It gives us the probability of a given number of events happening in a fixed interval of   time.
  
     ![poisson](/assets/img/poisson-distribution.png)

* Counts cannot be negative. The method will fail outright if you attempt to use it with negative labels.

* A Poisson distribution is a discrete distribution; therefore, it is not meaningful to use this method with non-whole    numbers.

### Use cases

This model could be used to predict :

* retweets of Twitter data 

* failures of nuclear plants under various operating conditions

* predict exam success rates among identifiable groups of students

* predict number of medical cases which occur due to some reasons



