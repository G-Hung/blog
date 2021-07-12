---
title: "Revisit some basic theorems in probability"
toc: true
image: images/post/statistics_theorem.png
comments: true
layout: post
hide: false
search_exclude: false
description: "Central Limit Theorem; Law of large number; Chebyshev's inequality"
categories: [statistics]
---

### For a long time, I confused their relationship

When I had my statistics class, I always confused these three in my mind:

Chebyshev's inequality [I don't know how to pronounce :-\, usually just call it CS inequality]: met it few times in my life but didn't leave me a big impression.

Law of large number & Central Limit Theorem: always use them interchangeably, but deep in my heart I remember they are different

Recently in a conversation with my friend, we talked about some hypothesis testing things [t-test], we discussed the assumptions of t-test like this:

```
A: yeah, you see, even the distribution shapes of these two population are different
By central limit theorem, the means will follow normal distribution regardless of the shape
We can still use it even the distributions are not normal

B: Sure, law of large number right? As we have more samples
they will converage and hence t-test is valid even the distributions are not normal

A: oooo seemingly right.....
```

Obviously I am A, but I was hestiate for few seconds because I forgot what is law of large number and how is it related to CLT! I remember they have some subtle differences. Therefore, I revisit the materials in probability course recently to answer the difference myself, and what the hell is Chebyshev's inequality


### Chebyshev's inequality
Recall the basic numbers for distribution, expected value and variance, one describes the central tendency, another describes the spreadness of the distribution

If the variance is small, the distribution is not that widely spread, it is less likely to get the outcome far away from the mean

In mathematical terms, it is less likely to see abs(X - u) >= certain number, hence Pr[ abs(X - u) >= certain number ] should be small.

When that certain number becomes even bigger, that probability should become even smaller [less likely]. 

Chebyshev's inequality basically states this relationship using expected value and variance:

- Pr[ abs(X - E(X)) >= a ] <= Var(X) / a^2 for a > 0

The importance of this equation is that we can calculate the sample size after we specify what level of confidence and bound we want

It is also beautiful! Link expected value and variance together in one inequality regardless of distributions

### Law of large number
Recall the fact that variance will decrease when n increases and take a look on Chebyshev's inequality again!

- Pr( abs(X - u) >= a) <= Var(X) / a^2 for a > 0
- Var(X) -> 0 as n increases

Therefore, Pr[ abs(X - E(X)) >= a ] -> 0 for a > 0
Therefore, Pr[ abs(mean(X) - E(X) >= a ] -> 0

Law of large number basically tells us the sample average will converge to expected value when n increase, basis of statistics and simulation

### Central Limit Theorem
CLT tells us average of n observations of ANY r.v will follow normal, ALL distributions, no matter how complex it is as long as mean and variance are finite

### Conclusion
Now rethink what each of them is doing

CS inequality tells us that the difference b/w sample and expected value is bounded

LLN tells us the difference b/w sample mean and expected value is not only bounded, but converages to zero when n increases

CLT tells us the sample mean not only converages, but the distribution of sample mean converages to normal distribution when n increases regardless of underlying distributions

CLT makes the biggest claim and hence is also the most famous, valuable and backbone of statistics

Recall the t-test conversation
```
A: yeah, you see, even the distribution shapes of these two population are different
By central limit theorem, the means will follow normal distribution regardless of the shape
We can still use it even the distributions are not normal

B: Sure, law of large number right? As we have more samples
they will converage and hence t-test is valid even the distributions are not normal

^^^This statement is not correct^^^
# sample mean does converge to expected value
# but nothing to do with converging to normal distribution, that's the magic of CLT

A: oooo seemingly right.....
```

### Disclaimer
Some of them are not precise & complete description, eg you may rmb weak/strong law of large number, reading a mathematical statistics book maybe more useful.
