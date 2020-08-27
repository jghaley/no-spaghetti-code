---
title: "Design Your Package"
teaching: 10
exercises: 0
questions:
- "When and how to design a package efficiently."
objectives:
- "Understand when designing a program can be useful."
- "Learn that UML exists"
keypoints:
- "Layout the diagrams on paper."
- "Think about the expected users."
- "Consolidating standalone scripts."
- "Modeling is the designing of software applications before coding."
---

## Fast solutions vs sustainable solutions

This is a very unique challenge for us. Usually our performance is evaluated by the results we've produced, not the codes behind the scenes. As a result fast solutions are naturally appealing. There are many fast solutions to lure us. For instance, we can open a TBrowser in ROOT and make the plots beautiful by hands. Also there are many unexpected studies when doing an analysis. We often have to perform a very specific study that goes beyond the current scope of your software. In this case, having something simple and fast to tackle down this one or two issues is indeed the most sufficient way. 

However, we also have frequent updates from various groups (combined performance groups, data preparation groups, physics groups, etc) and some of them can involve substantial changes. It is not surprising to find out that a script we wrote before does not work any more. 

A sustainable solution would take those possible changes into account and become flexible enough to incorporate them. They are better integrated into the whole workflow and can save us a lot of time in the long run. Giving the facts mentioned above, it is also challenging.  

## Plan and organize the package

Blueprints are important. It is hard to make sure all small pieces fit together nicely if we do not think ahead. Draw some diagrams on paper and think about what the upstream/downstream softwares are and who the expected users are. Try to figure out which parts of the package need to be rigid (or OK to be rigid) and which parts are definitely necessary to be flexible

Let's have a quick brain storming section: 

~~~
"What are the most common requests or comments one would receive during meetings that may require software change?"
~~~


Change the binning? Extend the binning? Add a histogram? Update CP recommendations? Add a ratio panel? Submitting grid jobs? Babysitting grid jobs?.....

Well if you have a list let's try to make our software able to do those things easily.
  

## Live with it or change it

Unless we start a project from scratch, we will probably be given some existing packages. If everything is up-to-date, nicely written and well organized. CONGRATULATIONS! But often this is not the case. In this situation, we can either live with it and try to get the work done or try to change it. When we have such a dilemma, we should think about how long we are gonna use them and how many more new things we are supposed to do. Often the time it is better to revamp. Do not let the argument "Please do not re-invent the wheels" stop you, you are crafting better wheels. 

<img src="{{ page.root }}/fig/michelin.png" alt="Good wheel!" width="60%" />

> ## Before you start writing code
>
> Take a deep breath... and get a blank sheet of paper
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


#### Interaction diagram 

The purpose of interaction diagrams is to visualize the interactive behavior of the system. Visualizing the interaction is a difficult task. Hence, the solution is to use different types of models to capture the different aspects of the interaction.[^1]

One of these models, shown below, is called the sequence diagram which captures the time sequence of the message flow from one object to another.

<img src="{{ page.root }}/fig/uml_sequence_diagram.jpg" alt="Sidebar" height="350px" style="float:center" />

<br>

You don't have to learn how these diagrams work right now, but it's good to know that they exist. When you're staring at a blank piece of paper trying to figure out how to design your code, take a look at the [UML tutorial](https://www.tutorialspoint.com/uml/) because chances are, theres a useful model to follow.

[^1]: Taken from [tutorialspoint.com/uml](https://www.tutorialspoint.com/uml/)

{% include links.md %}

