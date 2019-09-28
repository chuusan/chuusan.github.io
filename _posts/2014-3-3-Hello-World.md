---
layout: post
title: A Brief Introduction to Variance
---

To help you learn better about the `variance`. I find you a job at an Apple battery supplier (btw you are welcome!), Your job is to test the battery lifespan. 

On your first day of work, you are asked to submit a report regarding the batteries' lifespan for their newest iPad. Your manager told you that the average lifespan of these batteries is 1000 days $ E(X)=1000 $. One of your colleague thinks that the mean value is sufficient for your report. But actually:

- _It is possible that the majority of the batteries have a lifespan between 950 days and 1050 days._

- _It is also possible that about half of these batteries have a good performance of about 1300 days, however, the half left only have a lifespan of approximately 700 days._

To better learn the performance of these batteries, you need to mention the difference between the lifespan of each battery L and the average lifespan of these batteries E(X)=1000 in your report. But here comes the question. "How can you measure the difference?"

Apparently, we can use the following formula to measure the difference?

 E{|X-E(X)|}

But this equation contains absolute value computation, it is inconvenient for our calculation. So we transform it:
    
 Var(X) = E{ [X-E(X)]}


This is what we called `Variance`. Informally, it measures **how far** a set of (random) numbers are spread out from their **average value**. ([wikipedia](https://en.wikipedia.org/wiki/Variance))

### Definition 

The `variance` of a discrete random variable X measures the spread, or variability, of the distribution, and is defined by

Var(X)= Σ(X_i - \bar X) ^2 P_i

### Example:

Suppose an individual plays a gambling game where it is possible to lose \$1.00, break even, win \$3.00, or win \$10.00 each time she plays. The probability distribution for each outcome is provided by the following table:


| Outcome     | -  1|   0|   3|   5|
|-------------|:----|:--:|:--:|---:|
| Probability | 0.3 |0.4 | 0.2| 0.1|

_[Source](http://www.stat.yale.edu/Courses/1997-98/101/rvmnvar.htm)_

$E(X)= -1*0.3 + 0* 0.4 + 3+0.2 +5*0.1$

$Var(X)= (-1-0.8)^2*0.3 + (0-0.8)^2*0.4 +(3-0.8)^2*0.2 +(5-0.8)^2*0.1 =3.960$

Since there is not a very large range of possible values, the variance is small.
