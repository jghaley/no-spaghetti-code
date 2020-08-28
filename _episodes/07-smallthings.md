---
title: "Subtle Things That Make Our Lives Better"
teaching: 5
exercises: 0
questions:
- "What prevents others from understanding our codes?"
objectives:
- "Start apply some simple but very useful practice."
keypoints:
- "Add comments in your code."
- "Use variable/function/file names that are easy to interpret."
---



> ## ‎
> __Here are some suggestions from ATLAS colleagues about practices they think are particularly useful for our collaboration.__
>
{: .callout}

## We need comments

Quotes from a colleague:

~~~
"I did something quick and dirty in my code, wrote it down in my notebook (physical notebook). Now I have problems when using my code and I want to check what I did before. Guess what, I left my notebook at CERN and I could not go back!"
~~~


An Instagram post from a friend when she was on VACATION:

<img src="{{ page.root }}/fig/ArtOne.jpg" alt="Art is everywhere?" width="50%" />

A snapshot from a piece of code written by a paranoid programmer:

<img src="{{ page.root }}/fig/Paranoid.png" alt="Art is everywhere!" width="50%" />

We should add comments where we are not sure whether what we are doing is correct (FIXME) or at places to conclude a loop/block. Also if we think we might be the only person on this planet writing such a block of code, we should probably add some comments. 

## Use easy to understand variable/file names

It is quite desperate to look for a variable named as "m" and figure out what it is doing. Unless it is an index or a counter or something similar.

We physicists like acronyms, they can be funny but we should make sure they are understandable when using them in our code.

Follow a certain naming convention can help a lot.   

## Testing

Write automated tests for the libraries and tools you are developing. For example [pytest](https://docs.pytest.org/en/latest/) is a great library to help with testing. To take a somewhat strong position: any code that's not tested should be assumed to not work.

For more reading, [Atlassian has a nice post](https://www.atlassian.com/continuous-delivery/software-testing/types-of-software-testing) on the different kinds of testing in software.

## Documentation

The never ending battle of documenting your code... Documentation is very important not just for your future colleagues, but also for yourself. "The most likely person to read your code is you six months from now, and unfortunately, past you doesn't respond to emails" (no idea where I heard that).

Like the several levels of testing, there are several levels of documentation. Code can be seen as self-documenting if it's written with clear variable names. It also benefits from sensible inline comments. And it's always a good idea to leave [method docstrings in python](https://www.programiz.com/python-programming/docstrings) or [Doxygen-style comments in C++](https://www.doxygen.nl/index.html) to clarify what your functions are doing. These are also used for automated documentation parsing.

On top of these low-level pieces of documentation, each software package you write should have [a README file](https://www.makeareadme.com/) that explains what it does, how it's used, and who to ask for help.

{% include links.md %}

