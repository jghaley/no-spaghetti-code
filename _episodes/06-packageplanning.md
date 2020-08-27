---
title: "Design Your Package"
teaching: 5
exercises: 0
questions:
- "When and how to design a package efficiently."
objectives:
- "Understand when designing a program can be useful."
- "Learn that UML exists"

keypoints:
- "Modeling is the designing of software applications before coding."
- "Layout the diagrams on paper."
- "Think about the expected users."
- "Consolidating standalone scripts."
---

> ## Before you start writing code
>
> take a deep breath... and get a blank sheet of paper
>
{: .callout}


## Software design
> ## Modeling
>
> Modeling is the designing of software applications before coding
>
{: .callout}

The software we create is complex and involves lots of abstract ideas that need to work together. The classes and functions you write can quickly grow to more than you can keep in your head all at once. Large or small projects can all benefit from a careful consideration of how your software should work. If you want to build a house, your best first tool is a pencil, not a hammer.

<img src="{{ page.root }}/fig/software_paradigm.png" alt="Sidebar" width="250px" style="float:center" />

An excellent way to begin writing software is to draw a diagram. These can be diagrams that describe the inheritance of classes and interfaces, the ownership of objects, the logical flow of one or more functions, etc. All of these are useful thoughts to put on paper. Of course software is not a house; code is free. Your design can change as you learn new things about your data or your requirements.



## Unified Modelling Language

A powerful standard for producing these designs is called Unified Modelling Language, or [UML](https://www.uml.org/what-is-uml.htm). UML consists of many specifications that are widely adopted for creating designs for your software. These diagrams can be grouped into two broad categories:
* Structural Diagrams
* Behavioral Diagrams

You may find some of these diagrams more useful than others. [Here is a very nice UML tutorial](https://www.tutorialspoint.com/uml/) that gives a concise description of how to use the most common diagrams.

Here are a few specific examples of diagrams that you may want to try drawing for your code:

#### Class diagram 

The class diagram is a structural diagram. The purpose of class diagram is to model the static view of an application. Class diagrams are the only diagrams which __can be directly mapped with object-oriented languages__ and thus widely used at the time of construction.[^1]

<img src="{{ page.root }}/fig/uml_class_diagram.jpg" alt="Sidebar" height="350px" style="float:center" />



[^1]: Taken from [tutorialspoint.com/uml](https://www.tutorialspoint.com/uml/)

{% include links.md %}

