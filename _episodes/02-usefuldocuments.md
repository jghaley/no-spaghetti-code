---
title: "Useful Documents"
teaching: 5
exercises: 0
questions:
- "Where could I get guidance?"
objectives:
- "Knowing where to seek for help within the collaboration."
keypoints:
- "Start paying attention to good coding practice."
- "There are experts willing to help!"
---

## Materials from the ATLAS software team

The ATLAS computing team has many useful documenations (twiki pages, slides, notes, etc). Here is a list of them recommended by software experts:

1. [A nice twiki page on software quality](https://twiki.cern.ch/twiki/bin/viewauth/AtlasComputing/SoftwareQuality)
2. [A note on ATLAS C++ guidelines](http://atlas-computing.web.cern.ch/atlas-computing/projects/qa/draft_guidelines.pdf)
3. [A set of slides summarizing best C++ practice](https://indico.cern.ch/event/829411/contributions/3564510/attachments/1913272/3163600/2019-09-24-cxx.pdf)

Of course there are more available. If you have any questions you can also ask via the mailing lists: [hn-atlas-PATHelp@cern.ch](mailto:hn-atlas-PATHelp@cern.ch) (Physics Analysis Tools) and [hn-atlas-offlineSWHelp@cern.ch](mailto:hn-atlas-offlineSWHelp@cern.ch) (mainly Athena).

<img src="{{ page.root }}/fig/code_quality.png" alt="Sidebar" width="700px" style="float:center" />

### When is following this guide required?

If you do find yourself doing any [Athena](https://gitlab.cern.ch/atlas/athena) development (e.g. simulation, reconstruction, derivation) you are required to adhere to the style guide. Merge request shifters will hopefully enforce these rules.

Combined Performance and Analysis software packages are typically less restrictive with their requirements, but a few still maintain contribution guidelines that encourage high-quality code. For example, [EGamma CP](https://gitlab.cern.ch/ATLAS-EGamma/Software/ElectronID/TagAndProbe/-/blob/master/CONTRIBUTING.md) closely follows the Google __[C++](https://google.github.io/styleguide/cppguide.html)__ and __[Python](https://google.github.io/styleguide/pyguide.html)__ style guides. 

Let's be honest though. We don't expect that everyone is going to open those links and read the full style guides. The best way to learn these things is incrementally. 
* Keep an eye out for code that you find to be particularly readable and try to emulate that style. 
* When your code gets modified in a code review, investigate why the reviewer made the change they did.
* Use an IDE. Most modern IDEs have automated style checking and autoformatting. Learn from its suggestions.

## Internet

There are always answers to any coding problems on the Internet. We hope this bootcamp has expanded your ATLAS related coding vocabulary so that you can acquire your answers easier and faster. 

{% include links.md %}

