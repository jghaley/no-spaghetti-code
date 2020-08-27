---
title: "Use GitLab Wisely"
teaching: 10
exercises: 0
questions:
- "What usually causes trouble when using git?"
- "How could we avoid them?"
objectives:
- "Highlight non-optimal practice that occurs very often."
keypoints:
- "Commit often."
- "Write informative commit messages."
---

As illustrated by the previous instructors, Git (GitLab) provides very convenient functions maintain our repositories. We should make the most of it. 

## It is not Dropbox

The first recipe I got after joining ATLAS was:

~~~
"Copy my folder on lxplus to your directory and follow the README there. Do not use the version on GitLab, it does not work"
~~~
{: .source}

We hope this will not be the recipe you will share with your colleagues:).

## Pull often, commit often

Have you done this before:

~~~
mv project project_backup
git clone ssh://git@gitlab.cern.ch:7999/project.git
~~~
{: .source}

Because of merge conflicts? The time spent on fixing individual files again can be saved by many git commit/push/pull commands while developping your code.

## Informative commit messages

I browsed the commit messages I made six year ago:

<img src="{{ page.root }}/fig/ShameOne.jpg" alt="Why was I so apologetic?" width="50%" />

I'd hope the younger me could have just written down what the mistake was rather than being apologetic.

<img src="{{ page.root }}/fig/ShameTwo.jpg" alt="Nothing really?" width="50%" />
   
This is rather ambiguous as it could really have been literally nothing or a reflection of my state of mind. It turned out that I fixed a dump bug introduced by me.  

{% include links.md %}

