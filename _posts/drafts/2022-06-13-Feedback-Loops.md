---
title: "The Double Edged Nature of Feedback Loops | A High Level View"
description: "Double Trouble"
layout: post
sticky_rank:
toc: false
comments: true
categories: []
image:
hide: false
search_exclude: false
---

Whenever I find the computer science concept of "feedback" being explained, 
I always find it strange and a bit awkward. The example provided doesn't 
help either.

I feel feedback in computer science is intuitive and a pretty self 
explanatory concept: it's simply how feedback works in real life. In fact, 
that's how the concept should really be explained.

A person A does an action. Person B tells person A how to improve that 
action. Person A takes that feedback and improves the action. Persen C says 
person A's action is really good! Person A takes that feedback and does 
nothing. Person D says that action is really good, but _x_ could be done. 
Person A can choose to implement _x_ or not in their action.

Feedback loops are a natural continuation of this. The feedback person A 
receives, impacts the feedback that person A will receive in the future. 
Person B tells person A how to improve their action. Percon C was also going 
to tell person A how to improve their action. However, person B caused 
person A to improve their action, negating the need for person C to tell 
person A to improve. Instead, person C tells person A to keep going as they are.

This is pretty much how feedback and feedback loops work in computer science.
In computer science, person A would, for example, be the computer system and 
persons B, C, and D could be users, sensors, monitors, or controllers.

It can be seen that this is a pretty useful approach to creating systems 
that "sustain" or "adapt" themselves. Such systems would be able to improve 
themselves over time. In fact, this is how machine learning methods 
generally work. When training a model, the output of the model is used as 
feedback for the optimizer which then outputs a new set of coefficients to 
use in the model if needed.

However, the double edged nature of this concept comes into play with 
_positive_ feedback loops. Don't be fooled by the name! The _positive_ term 
doesn't refer to whether such feedback loops are good or not. Instead, it 
refers to how such feedback loops run.

A positive feedback loop is loop where the feedback exacerbates the 
situation at hand.

Take the current global warming crisis as an example. Our planet's ice caps 
are partly responsible for keeping Earth cool. However, out current global 
warming crisis is heating Earth up, which is causing the ice caps to melt. 
Smaller ice caps mean a hotter Earth. A hotter Earth means smaller ice caps. 
Smaller ice caps mean a hotter Earth. A hotter Earth means smaller ice caps. 
Smaller ice caps mean a hotter Earth. A hotter Earth means smaller ice caps.

And so on. Think of _positive_ as addition. It's adding to the situation. 
Obviously, there are good positive feedback loops, and there are bad ones 
too, as shown in the example above. Bad ones can become pretty bad.

Now how does this play into artificial intelligence methods? You can perhaps 
see where this is going.

[//]: # (Choose an example different from policing.)
