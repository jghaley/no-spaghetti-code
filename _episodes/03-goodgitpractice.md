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

```
"Copy my folder on lxplus to your directory and follow the README there. 
Do not use the version on GitLab, it does not work"
```

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

There are many articles defining how and why to write a good commit message ([here's one](https://chris.beams.io/posts/git-commit/)) but the basics are:

* Short one-line __subject__ describing what is done
* Longer multiline explanation of __why__ it was done
* Tell more than what files were changed. That's already obvious in the commit.

## Merge requests and code reviews

#### Merge requests

Merge requests in GitLab (and pull requests in GitHub) are some of the most powerful tools for collaboration and ensuring good practices are followed. You should _always_ make a merge request when submitting a significant change to a code base used by multiple people. 
Merge requests give other developers the opportunity to
* comment on your code, 
* make suggestions, and 
* review your work.

#### Code reviews

__[Code reviews](https://www.atlassian.com/agile/software-development/code-reviews)__ are one of the most effective techniques for any software project. Not only do they keep bugs from making it into the code base, but they are great for sharing knowledge. "When a developer is finished working on an issue, another developer looks over the code and considers questions like:
* Are there any obvious logic errors in the code?
* Looking at the requirements, are all cases fully implemented?
* Are the new automated tests sufficient for the new code? Do existing automated tests need to be rewritten to account for changes in the code?
* Does the new code conform to existing style guidelines?"
(- [Code reviews](https://www.atlassian.com/agile/software-development/code-reviews))

They are one of the best tools for mentoring new developers. Merge requests are the core structures for code reviews. They enable comments on individual lines of code, and keep a record of discussion about how a decision was reached. You are encouraged to a) review any code that someone writes to your repository and b) request than any code you push to a repository is looked over by a colleague.

<a href="https://oroinc.com/orocrm/blog/performing-efficient-code-review-part-i-best-practices/">
  <img src="{{ page.root }}/fig/code-review-best-practices.png" alt="Formatting Rules" height=300px/>
</a>


An excellent way to learn about the ATLAS codebase is to sign up for a [merge review shift](https://atlassoftwaredocs.web.cern.ch/guides/MR_reviewers/)! As a level-1 shifter you mostly follow a checklist and can raise any confusing changes to the level-2 shifters. Try it out!

{% include links.md %}

