---
title: "We Like Short Code"
teaching: 10
exercises: 0
questions:
- "How to make our code easier for others to use?"
objectives:
- ""
keypoints:
- "Use existing libraries if we can."
- "Create common functions if we need them very often."
- "Split if certain blocks become monstrous."
---

We work in a large collaboration and very likely when we need some functions in our code someone has already done it before and it may even exist in many well maintained packages. 

## ROOT has a lot of stuffs

Question:

~~~
"Have you created some functions and later on realized that ROOT already has them?"
~~~


Nowadays there are more well maintained packages to use so look around!

But be careful of the pitfalls:

<img src="{{ page.root }}/fig/Recursion.jpg" alt="Elegance!" width="50%" />

## Functions are better than copy/paste 

Prrof of concept:

<img src="{{ page.root }}/fig/function.jpg" alt="Loop!" width="50%" />

## We can use multiple files.

~~~
"Would you rather fight 100 500-line C++ scripts or 10 5000-line C++ scripts?"
~~~

{% include links.md %}

