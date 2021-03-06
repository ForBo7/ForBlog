---
title: "📌 Data Quality is Important | Car Classifier"
description: "Classy Cars"
layout: post
sticky_rank: 1
toc: false
comments: true
categories: [data, data cleaning, analyzing models]
image: images/2022-06-04/thumbnail.jpg
hide: false
search_exclude: false
---
![A parking lot filled with rows of cars.]({{ site.baseurl }}/images/2022-06-04/thumbnail.jpg)

I recently created a car classifier that classified cars into their brand.

Despite having almost 5000 images in training set, I ended up having to use 
over a hundred layers (I ended up using ResNet101) in my model and twenty 
epochs. Even then, I still had an error rate of 17.4%.

The culprit? My dataset.

I scraped 5000 images of cars (500 for each company) from DuckDuckGo. 
Naturally, as expected, the data quality is not so good.

Why? Below are some potential reasons:
- Noncar images present in dataset
- Cars of incorrect company present in dataset
- F1 cars present in dataset
- A large variety of cars from different time periods present in dataset
- Different companys' cars look similar
- Modded cars present in dataset
- Concept cars present in dataset
- Multiple cars present in a single image
- Certain angles of cars appear more than others
- Cars appear in certain backgrounds more than others
- The search term `{car_brand} car` could be skewing results

I could have absolutely achieved better results with fewer layers and fewer 
epochs if I trained the model on better quality data — or manually combed 
through the 5000 images 💀. However, I did use fastai's GUI for data cleaning.
This GUI sorts images by their loss which helps to determine if certain 
images should be relabeled or deleted.

Below is the confusion matrix for this model.

![Car Classifier Confusion Matrix]({{ site.baseurl }}/images/2022-06-04/confusion_matrix.png)

It can be seen that this model "confuses" between quite a few different 
brands: Ford and Chevrolet, Chevrolet and Ford, Jaguar and Aston Martin, 
Renault and Ford.

But **why** is data quality important? Because without good data, the model 
will not be able to "see" things the way they actually are and in turn, end 
up making worse predictions and not be able to generalize to other data.

Let's say you did not know how a toaster looked like. So I taught you by 
showing you pictures of a kettle. Then to test you, I showed you a set of 
pictures depicting various kitchen appliances and told you find the toaster. 
You would not be able to. 

Similarly, if instead I showed you toasters only 
from two brands and toasters from only the last two years, you would not be 
able to idenfity toasters from other brands or from other years.

Obviously, humans are smarter and can infer. AI methods can only infer to a 
certain degree, mainly based on what is in their dataset. This talk does 
start to become more philosophical.

The point of this post is to emphasize the importance of quality data and 
different aspects to consider as to why data quality may not be good. You 
can have the best architecture in the world but it is pretty useless if you 
don't have good data.

If you have any comments, questions, suggestions, or corrections, please do 
post them down in the comment section below!