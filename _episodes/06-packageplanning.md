---
title: "Design Your Package"
teaching: 5
exercises: 0
questions:
- "When and how to design a package efficiently."
objectives:
- ""
keypoints:
- "Layout the diagrams on paper."
- "Think about the expected users."
- "Consolidating standalone scripts."
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

{% include links.md %}

