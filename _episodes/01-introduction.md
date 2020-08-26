---
title: "Introduction"
teaching: 5
exercises: 0
questions:
- "What kind of code should we (not) write?"
objectives:
- "How to make the software packages written by us more accessible by our colleagues."
keypoints:
- "We are not professional software engineers but software is important."
- "Our code is very likely to be shared with our colleagues."
---

> ## What is a programming language?
>
> __"Programs must be written for people to read, and only incidentally for machines to execute."__
> 
> _-Abelson & Sussman, Structure and Interpretation of Computer Programs_[^1]
>
{: .callout}

[^1]: [Structure and Interpretation of Computer Programs](https://en.wikipedia.org/wiki/Structure_and_Interpretation_of_Computer_Programs)

<br>

We work in a large collaboration so that we read/use each other's codes very often. Sadly but truly discussing coding is part of our lives (at least mine). No matter what is going on in this world, we talk (complain) about software often. Again at least for me:

<img src="{{ page.root }}/fig/Sadness.jpg" alt="My lunch conversation compositions:" width="90%" /> 

Ok that is a bit exaggerated but software is indeed important for us. In this mini section we are not gonna tell you everything you need to know about writing elegant codes but rather share our experience working with software in ATLAS. Hopefully in the end we could convince you that it is worth thinking about this. 

## Why care about good code?[^2]

We are busy people with dozens of things to pay attention to in our work.
Why should we put in additional effort to produce quality code? Why not just settle with code that works?

Focusing on quality code is actually one of the best ways to save you and your team tremendous amounts of time in the future. Clean and elegant code is much easier to understand, maintain, and extend.

[^2]: Borrowed heavily from [Cleverti](https://medium.com/@cleverti/why-is-code-quality-such-a-big-deal-for-developers-91bdace85d44)

## Code quality goals[^2]

* __Readability, consistency__ — how easy it is to read and understand sections of the code; this includes code clarity, simplicity, and documentation.

* __Predictability, reliability, and robustness__ — software behavior should be predictable, and not prone to hidden bugs.

* __Maintainability and extensibility__ — fixing, updating and improving software should be as simple as possible, not inherently complex.

This lesson will introduce practices and habits that will help you achieve these goals. Some techniques are good for software development in general, and some are specific to the coding we do in ATLAS.

<br>

{% include links.md %}

