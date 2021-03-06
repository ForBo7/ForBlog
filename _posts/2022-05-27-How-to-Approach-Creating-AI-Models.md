---
title: "How to Approach Creating AI Models"
description: "Putting the drive into the train."
layout: post
sticky_rank:
toc: true
comments: true
categories: [model deployment, drivetrain approach]
image: images/2022-05-27/thumbnail.jpg
hide: false
search_exclude: false
---

<img src="{{ site.baseurl }}/images/2022-05-27/thumbnail.jpg"
width=250>

## Introduction

How you approach making your model is crucial. Articial Intelligence is not 
about creating models; it is only a tiny part of it. It is 80% problem 
solving and 20% implementing (I would not be suprised if it actually 
followed the 80-20 rule[^1]).

It is like the scientific method in a sense. Sure, you can create a really 
accurate, well functioning experiment. But what use is it if you do not 
approach conducting the experiment and analyzing the results in a well 
defined manner?

One highly successful approach is the _Drivetrain Approach_, created by 
fast.ai course creater Jeremy Howard along with his collegues Margit Zwemer and 
Mike Loukides. Their official blogpost on this approach goes into much 
detail and can be read in full [here](https://www.oreilly.com/radar/drivetrain-approach-data-products/).
The goal of this approach is to not use data just to generate more data 
(that is in the form of predictions), but to use data to also generate 
actionable outcomes.

Over here, I'll be providing a short overview of my understanding of this 
approach (from the fast.ai course) and will be applying it to the final 
project I did in the 
University of Helsinki's and Reaktor's [Elements of AI](https://www.elementsofai.com) 
course (I highly highly recommend this course; it gives a really good primer 
into AI).

## Overview of the Drivetrain Approach

There are four main steps to this process:

- Define the objective
- Consider your possible actions
- Consider your data
- Create the models

### Define the objective

Write out what you are really trying to achieve. What is your goal?

### Consider your actions

Think about what actions you can take to achieve your objective. 

Also think about what would happen if you did those actions. What would 
happen if did _x_? Would _y_ really be a good idea? What if _z_ worked 
really well? What if _z_ worked really bad?

### Consider your data

Think about the data you already have and how it can be used. Think about 
any further data that is needed and how it could be collected.

### Create the model

Created models that produce the best actions that in turn produce the best 
results in terms of your objective.

## Endangered Language Chatbot

The final project of the Elements of AI course asked me to come up with my 
own AI method that would solve a problem, and how it would. I ended up 
creating an overview for how a chatbot could be created to preserve 
endangered languages.

Now that I think of it, what the project asked me to do is one sort of 
approach to creating AI methods, though more on the why side. You can view my 
project overview 
[here](https://github.com/ForBo7/Endangered-Language-Chatbot).

### Define the objective

The objective of creating such a chatbot is to preserve languages that are 
endangered or extinct. This would help preserve different histories and 
cultures, as well as humanity's diversity.

### Consider your actions

Probably, a new sort of NLP architecture would have to be created primarily 
due to the lack of data there would be for these languages.

Alternatively, existing methods could be applied, but there would be varying 
degrees of success depending on how much data is available for a language.

### Consider your data

The main source of data for training such models would corpuses of text. 
However, this itself is a problem since many endangered or extinct languages 
do not have enough written text that would achieve the level of performance 
required to have somewhat of a good conversation with the bot. Further 
troubles arise for those languages that are speech only; you would need to 
have audio recordings, which would be extremely difficult for a language 
that is endangered or nigh impossible for those that are extinct.

The main solution to these problems that comes to mind is literal manpower 
and brute force. That is, humans would have to manually create masses of 
text or speech that the model can then be trained on to "learn" the langauge.

### Create the model

Create a model that speaks as accurately as a native of the endangered 
language so that any person interacting with the chatbot gets a vivid idea 
of the language, its culture, and its people.

## Conclusion

This concludes my understanding and explanation of one such approach to 
creating models, along with an attempted example. Approaches are crucial: 
you can have all the best tools and the most accurate models in the world, 
but they are worthless if not correctly approached, used, and applied.

If you have any comments, suggestions, or corrections, please do post them down 
in the comment section below!

**Footnotes**

[^1]: [The 80/20 Rule, also known as the Pareto Principle](https://en.wikipedia.org/wiki/Pareto_principle)