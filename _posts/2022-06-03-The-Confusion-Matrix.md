---
title: "A No Nonsense Guide to Reading a Confusion Matrix"
description: "Are you confused yet?"
layout: post
sticky_rank:
toc: true
comments: true
categories: [how to, guide, confusion matrix, analyzing models]
image: images/2022-06-03/thumbnail.jpg
hide: false
search_exclude: false
---

<img src="{{ site.baseurl }}/images/2022-06-03/thumbnail.jpg" 
alt="What matrix were you thinking of?" width=400>

Confusion matrices help us model designers view what mistakes our model has 
made.

I'll be approaching this with logical examples.

Jump to [Case 2](http://forbo7.github.io/ForBlog/how%20to/confusion%20matrix/analyzing%20models/2022/06/03/The -Confusion-Matrix.html#case-2) for an ultra concise rundown.

Ready? Here we go.

## Case 1: Introduction

<img src="{{ site.baseurl }}/images/2022-06-03/confusion_matrix_1.png">

Ignore the "Actual" and "Predicted" labels for now.

Let's compare grizzly bears to black bears.

All comparisons begin at the bottom, and with the columns.

First, highlight the grizzly bear column.

<img src="{{ site.baseurl }}/images/2022-06-03/confusion_matrix_1_1.png">

Next, highlight the black bear row.

<img src="{{ site.baseurl }}/images/2022-06-03/confusion_matrix_1_2.png">

Now find the common entry in the highlighted column and row.

<img src="{{ site.baseurl }}/images/2022-06-03/confusion_matrix_1_3.png">

This common entry is our required information.

All entries in the main diagonal are correct 
classifications. All other entries are incorrect classifications.

Our common entry does not lay in the main diagonal. Therefore we are looking 
at incorrect classifications.

We have compared grizzly bears to black bears. Therefore, from this 
deduction, **three grizzly bears have been incorrectly classified as black 
bears**.

{% include info.html text="There is a difference between comparing grizzly 
bears to black bears and black bears to grizzly bears.
<br><br>
Comparing grizzly bears to black bears means, 'How many grizzly bears were 
misclassified as black bears?'
<br><br>
Comparing black bears to grizzly bears means, 'How many black bears were 
misclassified as grizzly bears?'" %}

## Case 2: Ultra Concise

Let's compare black bears to grizzly bears.

Highlight the black bear column.

<img src="{{ site.baseurl }}/images/2022-06-03/confusion_matrix_1_4.png">

Highlight the grizzly bear row.

<img src="{{ site.baseurl }}/images/2022-06-03/confusion_matrix_1_5.png">

Highlight the common entry.

<img src="{{ site.baseurl }}/images/2022-06-03/confusion_matrix_1_6.png">

Zero grizzly bears were misclassified as black bears.

## Case 3: Correct Classifications

Let's see how many teddy bears were correctly classified. We are essentially 
comparing teddy bears to teddy bears.

Highlight the teddy bear column.

<img src="{{ site.baseurl }}/images/2022-06-03/confusion_matrix_1_7.png">

Highlight the teddy bear row.

<img src="{{ site.baseurl }}/images/2022-06-03/confusion_matrix_1_8.png">

Highlight the common entry.

<img src="{{ site.baseurl }}/images/2022-06-03/confusion_matrix_1_9.png">

Fifty three teddy bears were correctly classified as teddy bears.

## Exercise: Do It Yourself

Below is a confusion matrix of a car classifier that classifies cars into 
their brand.

<img src="{{ site.baseurl}}/images/2022-06-03/confusion_matrix_2.png">

You learn by doing!

- How many Lamborghinis were correctly classified?
- How many Jaguars were incorrectly classified?
- How many Chevrolets were misclassified as Fords?
- How many Fords were misclassified as Chevrolets?
- Which two car brands did the model have the most trouble differentiating 
  between?



If you have any questions, comments, suggestions, or corrections, please do 
post them down in the comment section below!