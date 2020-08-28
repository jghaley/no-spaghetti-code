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

	


> ## ‎
> __"Measuring programming progress by lines of code is like measuring aircraft building progress by weight."__
> 
> _- Bill Gates_
>
{: .discussion}

We work in a large collaboration and very likely when we need some functions in our code someone has already done it before and it may even exist in many well maintained packages. 

## ROOT has a lot of stuffs

Question:

~~~
"Have you created some functions and later on realized that ROOT already has them?"
~~~


Nowadays there are more well maintained packages to use so look around!
Start with a look at the [ROOT Tutorials](https://root.cern/doc/master/group__Tutorials.html) to get a sense of what is possible.

But be careful of the pitfalls:

<img src="{{ page.root }}/fig/Recursion.png" alt="Elegance!" width="50%" />

## Functions are better than copy/paste 

Prrof of concept:

<img src="{{ page.root }}/fig/function.jpg" alt="Loop!" width="50%" />

## We can use multiple files.

~~~
"Would you rather fight 100 500-line C++ scripts or 10 5000-line C++ scripts?"
~~~

## Refactoring

Another habit that's good to form is _refactoring_ your code. Refactoring is the process of restructuring existing computer code without changing its external behavior. It is intended to improve is non-functional attributes while preserving its functional behavior.

This can include:
* Simplifying logical expressions
* Removing duplicated code
* Replacing unclear variable names with clearer ones
* Improving C++ functions for more efficient compiling/running (virtual, static, constant, etc.)
* Re-writing a loop to be more efficient
* Including checks for undesired inputs (e.g. null pointers, edge cases)

Do you think that the first time you write some code it is going to be the most correct or the most readable? Me neither. Refactoring is an important process of making sure the code is high-quality. It also is often how you catch unnoticed bugs!

Testing is a very important part of refactoring! The more automated tests you have, the more confident you can be that your changes didn't unexpectedly break anything.


> ## Want to know more?
>
> [Refactoring Guru](https://refactoring.guru/refactoring) has some excellent lessons on how to refactor your code and why it's useful.
>
{: .callout}

{% include links.md %}

