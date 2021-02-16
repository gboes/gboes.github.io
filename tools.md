---
title: Digital Tools
layout: default
permalink: /tools/
description: A collection of digital tools that I found (at least at some point) useful for my academic work. If time permits, I provide a more detailed article.
---

> Here I collect digital tools that I found (at least at some point) useful for my academic work. If time permits, or somebody lures me into [structured procrastination](http://www.structuredprocrastination.com/), I provide a more detailed article.

## Why?
While there were good support classes offered for physics students, I did not find much material on digital tools for philosophers. While studying in Tokyo, I took a class in digital humanities, but that resulted only in using a proprietary XML editor to tag a document by hand. This produced little insight and solved no problem I ever had, although I understand it might be relevant for scholars preparing digital editions of manuscripts. A digital humanities class I took in London was a little better, but had no great payoff either. 
In Cambridge there was at least a mention of the open-source bibliography manager Zotero, and eventually some academics recommended Scrivener as a writing environment. But nobody could help for example with adapting a Zotero citation style to support shorthands, which were quite common in my field at least. It still seems that for learning about digital tools, there is little on offer, and I suspect the situation in disciplines other than philosophy is similar. I almost certainly spent more time on methodological considerations than I should have, but I think of myself as slowly reaping a dividend for this time investment. Maybe I can help others to get there more quickly. 

## Reference Management
The tools I have adopted differ enormously in terms of complexity and payoff. 
The lowest hanging fruit is to use **Zotero** as a reference and file manager. If you don't do that yet, stop reading and set it up right now, I cannot see how you could regret it. (tutorials for setting up zotero and zotfile have been around for a while, like [this one](https://gettingthingstech.com/zotero-workflow-zotfile/))


## eReading / Digital Paper
The next most useful thing I established is probably my **e-reading and note taking setup**. This is also a tool on which I did not find much information (and even a little disinformation) on. It's a new market, so there's also a lot of videos around that in my view oversell what eReaders can currently do. But after a lot of research and trial and error, I have found a setup that I am happy with. I found it especially helpful for regaining some longer-attention span, slow-thinking time that is so crucial for philosophy. 

Here is the [full article](/tools/ereader "Article on my ereader setup").

## Emacs and org-roam for a digital slip box (Zettelkasten)
**Emacs** is an extensible Open Source text editor that has been around since the Seventies (which is a biblical age for software, I guess). What distinguishes it from more modern editors is its radical extensibility: almost any part of the program can be changed by the user. Using emacs is more like building something you like out of a bag of mixed lego pieces, and any two users usually end up with quite different programs.

Adopting emacs as my text-editor is by a great margin the most complex tool that I have adopted, it is probably overkill for most people working in the humanities. I have so far only met one colleague who also uses it for philosophy (shoutout to Dan). 
I still think has real potential, especially if you occasionally have to edit code as well. With the introduction of Windows WSL, the performance under Windows improved drastically, and doom emacs makes the configuration much simpler. This makes emacs a cross-platform tool.

If you do not need to program, emacs might still be worthwhile if you are interested in adopting a powerful way to take notes. [org-roam](https://github.com/org-roam/org-roam/) is great and has immensely cleaned my desk. Especially those who have heard of [Luhmann's Zettelkasten](https://en.wikipedia.org/wiki/Zettelkasten) (that's almost always sociologists) might be interested. Org-roam allows to quickly take notes without having to think of an eternal hierarchy. This is very useful when somebody says something interesting in a talk, or you come across an idea in an unexpected place, you just read an interesting paper or found a nice poem to quote etc.  These notes can be linked, and following their interconnections at a later time can reveal unexpected connections.  But even without the creative benefit, adopting this note taking system helped me to increase focus (because I can write any ideas down and return to what I was meant to do) and reduced my anxiety about forgetting ideas and losing  temporary notes. Maybe I will describe this process at some point in more depth.

## LaTeX
I mostly use LaTeX for my academic work, because it gives me fine-grained control and modularity. Emacs' org-mode and LaTeX work well together, which is why I am still using it to write my PhD thesis and normal papers. I have not planned to add a detailed description of this setup, but who knows.
The original selling point of TeX is that you can completely separate writing and formatting, but with a little discipline this is possible in Word as well. In short, I totally understand why most people in the humanities avoid TeX.

Be that as it may, I ended up cobbling together a XeLaTeX Beamer style with KCL's corporate design, to create my academic presentations (see the slides in [downloads](/dl/), but let me know if you are at KCL and interested in adopting it). 

## Semi-automatic absence reports
I have semi-automated a KCL-specific procedure for reporting consecutive student absences. This saves writing time and allows me to include more information and better formatting into the emails I send to personal tutors. The code is quite trivial and runs via Python3 on a command line. A running outlook instance opens a draft window, nothing sends automatically. The [repository is on github](https://github.com/gboes/absence_reporter/), in case you are interested in solving a similar problem.



<!-- ## Open Source -->
<!-- One of the many things that distinguished my studies in physics from those of philosophy was the presence and awareness of digital tools for research.  -->
<!-- It might be a particularity of German academia, and maybe the physics community, that a lot of emphasis was placed on the use of open source tools.  -->
<!-- All departmental workstations, as well as those used in the Max-Planck Institute for Physics were as a matter of course running Ubuntu (and a KDE desktop) -->

<!-- It might have even been something more local about Munich. It is the only city whose administration ran in a tailor-made open source environment (with its own distribution, LiMux). So it is probably a fertile ground for Open Source enthusiasts. But the different fields seem to play their part: When I started a new research assistant job at the Max-Planck Institute for Innovation and Competition -- populated mostly by economists and legal researchers -- the computing environment was built on Windows 7 again. -->

<!-- In this article, I list all open source tools hat I regularly use (and this is not because they're free - I do not mind paying for a tool if it does a job better). Maybe there are some that are not well enough known - like the lovely little *briss* that lets you crop pdfs and split pages in a very smart way - for anyone scanning books, a godsend. -->

<!-- [Here](/tools/floss/) is a  simple list of open source software that I am using. -->





<!-- ## Hosting a personal website on github pages / jekyll -->
<!-- There are simpler solutions. But having version control built in is nice, and it was quite educational to set this up. But I don't think I have very strong opinions about this; just that it feels much nicer to know _mostly_ what is happening on your website, and not having to deal with all the hidden stuff that comes with wordpress. And of course already using emacs makes writing markdown comparatively nice. -->
