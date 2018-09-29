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
  
     ![poisson-distribution](/assets/img/poisson-distribution.png)

* Counts cannot be negative. The method will fail outright if you attempt to use it with negative labels.

* A Poisson distribution is a discrete distribution; therefore, it is not meaningful to use this method with non-whole    numbers.



## Why Poisson Regression works better over linear or logistic regression

**Linear regression** make wrong kinds of assumptions about what count outcomes look like.It assumes that target values are normally distributed around the expected value and can take any real value, positive or negative, integer or fractional, whatever.If you throw some data for predicting number of people affected by Dengue outbreak then its a possibilty that it might predict some absurd values like 0.5 people or -5 people.

*Logistic regression* only works for data that is 0-1-valued (TRUE-FALSE-valued), like "has a disease" versus "doesn't have the disease".

The **Poisson distribution** is discrete and positive. At a very minimum, this will make your model to give you answers that could actually happen in real life. They may or may not be good answers, but they will at least be drawn from the possible set of "people affected by disease".

### So Is Poisson Regression the perfect solution?

# Sadly NO! 

The Poisson has its own problems 

It assumes that the mean of the vote count variable will also be the same as its variance. There are hardly any non-contrived examples where this was true. 

Fortunately, bright people have come up with other distributions that are also positive and discrete, but that add parameters to allow the variance to vary.

So one of that distribution is **Negative Binomial Distribution**

## Now What is Negative Binomial Distribution?

Negative binomial regression is a type of generalized linear model in which the dependent variable  is a count of the number of times an event occurs.

Isn't this why we used Poisson Regression?

*Well Yeah!*

The negative binomial regression simply lifts the assumption that the population mean and variance are equal, allowing for a larger class of possible models.In fact, from this perspective, the Poisson distribution is but a special case of the negative binomial distribution.



##TL;DR

If your target variable is a non-negative integer and you are looking to make some count predictions. 
Then you have two Standard regression techniques for this type :

* Poisson regression
  if mean = Variance

* Negative binomial regression
  if mean != Variance



### Use cases

This model could be used to predict :

* retweets of Twitter data 

* failures of nuclear plants under various operating conditions

* predict exam success rates among identifiable groups of students

* predict number of medical cases which occur due to some reasons



