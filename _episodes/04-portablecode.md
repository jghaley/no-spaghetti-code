---
title: "We Like Portable Code"
teaching: 10
exercises: 0
questions:
- "Why should we make our code portable?"
objectives:
- ""
keypoints:
- "Use relative path and environment variables."
- "Test it often."
- "Use CI."
---
Usually we do our work on certain machines. People based at CERN would prefer lxplus while people based outside may prefer their local clusters or personal machines. Each individual may also have a different shell setup. It is very rare that the person who writes the code is the sole user. As a result, it is important to make sure the code can be used by others on a different machine/setup easily. It is really worth the time thinking about this as in the end if your code does not work for someone, you will likely receive an email or message asking for help:)  

## Avoid user/machine specific setups

It can be prevented by using relative paths or environment variables. It also makes our softwares easier to run on the grid as the grid can not access your local machines. 

## Test it often

The infrastructures/softwares keep evolving (slc5 -> slc6 -> centos7, Athena Rel 20.7 -> Rel 21). The packages involved can change very often as well. We should test our code often. 

Having it compiled is not the end goal as we want the results to be meaningful ultimately. So it is better to test the whole work flow. 

CI saves the day!

It feels really great when everything just works out of the box after following the recipes in the README.  

{% include links.md %}

