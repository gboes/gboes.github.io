---
title: digital paper - eInk for focused reading and writing
layout: default
permalink: /tools/ereader
description: This little article describes how I use a Boox Max 3 in conjunction with Zotero for reading, annotating, and synchronizing a digital library (mostly pdfs). The setup also has great potential for writing and note taking, both by longhand and typing.
---

# Like paper, but digital &ndash; an eInk solution for focused reading and writing

> This little article describes how I use a Boox Max 3 in conjunction with Zotero for reading, annotating, and synchronizing a digital library (mostly pdfs). 
> TL;DR: For some years, I could not achieve an entirely digital workflow for reading and writing. Now I have moved to a setup centred around the Boox Max 3, and I am for the first time very happy with my solution. Things I like: less eyestrain, consistent digital annotations, fewer distractions, great mobility, being able to work outside, with much of the haptics of working on paper. The setup also has great potential for writing and note taking, both by longhand and typing.

![Boox Max 3 lying flat](/graphics/max3_horizontal_web.jpg)
<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
**Table of Contents**

- [The problem](#the-problem)
- [Basics: eInk](#basics-eink)
- [The Boox Max 3 - and its price drop](#the-boox-max-3---and-its-price-drop)
- [Demonstration: pdf reading and annotation](#demonstration-pdf-reading-and-annotation)
- [The setup](#the-setup)
- [Alternative ereaders](#alternative-ereaders)
- [Anticipating disappointments](#anticipating-disappointments)
- [Bonus: emacs via Termux](#bonus-emacs-via-termux)
- [Further resources](#further-resources)

<!-- markdown-toc end -->


I vividly remember the first time I entered the Knightsbridge professor's office. It was an enviable place to work in. But despite the room's impressive size, it was filled to the brim: spines of books covered every bit of wall. I was hoping that one day, I'd amass a similar collection.

But frequently moving as a student, usually living only in a small room, and knowing the financial prospects of an academic career for those who are not "independently wealthy", I could not really see how. Besides the cost of acquisition, already the _physical challenge_ of taking care and keeping track of such a physical library seemed unachievable. When I moved from Munich to London (let alone from Munich to Japan), I had to make heartbreaking choices between which books I would bring and which I would sorely miss a month later. On top of that, Hermes lost one of the two boxes I sent, so the greater part of my painfully selected titles never arrived. <sup id="a1">[1](#f1)</sup> Meanwhile, my parents had long lost track of the books with strange titles that kept filling up every little corner. 

Although the physical library has a great romantic appeal and makes for an impressive Zoom background, I had long hoped that there was a better way. The technology had been a long time coming and I saw no reason why it should not be possible to find a satisfying digital workflow for - in my case - academic philosophy. But my previous attempts, with Kindles and an expensive and niche devices, like the Boox M96, all failed. My last attempt, however, is finally satisfying. Maybe you are also dissatisfied with reading on your laptop and the problems with physical books sound familiar. If on top of that you are not afraid of shrinking the physical representation of your intellect, you might want to read on.

## The problem
Philosophy obviously involves a lot of reading. Physical reading material presents a number of problems:
- hunching over books for hours is not ergonomic
- lack of mobility (also requires e.g. choosing which books to bring into a library)
- no backups
- not integrated into a digital writing process
- expensive
- limited to one user at a time
- indices provide only limited keyword navigation, no direct following of references
- not everyone is fast at or enjoys handwriting

Digitizing the reading aspect of academic work seems like a good way to address these problems. But it raises at least five new problems:

- eye strain or insomnia from extended screen use
- abundance of distractions when reading on a laptop or tablet
- unspontaneous annotation capacities, lack of physical interaction
- mobility limited by battery
- working in sunlight is impractical

There might be other digital setups that work well. If you do not encounter any of these problems, I am not sure you will benefit much from what follows, other than satisfying curiosity. To me anyways, a combination of these issues was a reason for a recurrent dissatisfaction. Seeing a fair number of colleagues printing out what they plan to read had me thinking that I am not alone in this. 

I thought about this for a long time -- the reason that I am writing now is that I think I cracked it. My current solution to these problems centres around a device by a Chinese company called Onyx, the Boox Max 3. It is a 13" (ca. A4) eInk tablet that runs Android 9.0, exactly the same operating system that runs a lot of phones and some conventional tablets. I bought my first eReader in 2010, and tried to build this setup since at least 2014, when I invested a scholarship into a Boox M96. That ultimately failed, and likewise did later attempts to achieve this with a Kindle. But in late 2020, I wanted to give it another shot (because what do you do in a pandemic?) and I got my hands on a reMarkable 2 eInk tablet. That didn't work either, but I realized that Onyx had considerably improved their devices. Begrudgingly I decided to give them another shot (it was Christmas after all), and to my amazement, it finally works. 

As you can probably tell, this is not an advertisement for Onyx, and I am not sponsored them nor anyone else. My experience with the M96 made me reluctant to ever buy from them again, and I don't think they are a particular nice company &ndash; more on that below. But in the end I am just glad I can finally do what I wanted all along. If this article is useful to somebody who wants to rethink the way they consume or create text, that is all I want to achieve. More incidentally, that the [Max 3 supports Termux](#bonus-emacs-via-termux) might also be interesting to coders or people who could use an eInk screen in a DIY project.

## Basics: eInk
If you already know what eInk is, just [skip this section](#the-boox-max-3---and-its-price-drop). eInk screens have been around for a while, mainly popularized through Amazon's Kindle. What I am describing here is centred around a device that uses the same technology, but unlike the Kindle, is not part of a book retail ecosystem.

The most common computer screens are backlit: that means they have an approximately uniform light source that is then manipulated to yield what you see on a screen. By digitally controlling how much of the uniform backlight is filtered out (e.g. using liquid crystals), the image on a screen can change. These changes can happen extremely fast &ndash; images can be redrawn hundreds of times per second. But without the backlight, the screen remains black.

An eInk display, on the other hand, does not use a backlight. It rearranges "digital ink particles" that just reflect whatever light hits the screen, like toner or ink paper would. At least for my reading experience, this makes a significant difference. You are not looking into a light source. A situation where this difference becomes obvious is when you take the screen outside, for example to read on a park bench. On a sunny day, it will be hard to read on most laptop screens, but no issue at all with an ereader, where the reflected sunlight is not competing with a backlight. Not having a backlight also means that you do not need power to keep your images alive: the screen only draws power to change what it displays. 

But eInk screens also come with drawbacks: the refresh rate is generally either very slow, or in a fast refresh mode, new images show traces of what has been displayed before ("ghosting", like seeing through thin paper). The current lack of colour can also be a deal breaker, if you want to study colourful plots or anatomical drawings for example. The underlying screen technology also appears to be restrictively protected by patents and new developments are happening at a moderate pace. In short, eInk devices have remained a niche product.

## The Boox Max 3 - and its price drop
I ended up buying the Max 3 after a detour. In 2020, the reMarkable 2 was launched - a note taking device with an A5 eInk screen. Apparently I had not opted out of all ad personalizations: Some colleagues and I were inundated with advertisements for it, until I actually wanted to give it a try. It looked like suddenly eInk would break out of its niche, and the device was so hyped that I had to wait more than 2 months until my order arrived.

In the end, I returned the device, because of a disappointing reading experience and the limitations in controlling the software. But I had been impressed by the nice writing experience, and started a much too long research into which new devices had come up recently.

It turned out, Onyx had just released the Boox Max Lumi, the first A4 eInk device with an integrated light (not a backlight, but shining diffusely from the side, but I agree that it can be confusing). The Lumi was impossible to get hold of, and if it were, it would cost more than €1200. After my bad experience with the company before, I did not want to trust their software or their warranty, and I did not find anything about a trial period. But I realized that its predecessor, the Boox Max 3, was essentially the same device, just missing the light and running Android 9 instead of 10. It used to be just as expensive, but without the novel light it got a lot less interest, so I could find the Max 3 for €580 on German eBay, refurbished by Onyx. I follow with a short demonstration, and then explain my file synchronization and Zotero integration which work really well. After that, I mention a number of caveats, because they might be sources of frustration (like the lack of a proper manual, in a European language at least).

## Demonstration: pdf reading and annotation
Here are two short demonstration videos to give you an idea of what reading with the Max 3 looks like. I have placed the Max 3 in a tablet holder and, for the second video, added a clip-on light. In a well-lit office or outside, a clip-on light is not necessary at all.

<p align="center">
<iframe width="360" height="640" src="https://www.youtube.com/embed/2jPOH7KFSh0" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></p>

Here I demonstrate several ways of adding annotations to a pdf article: you can draw directly onto the pdf. <sup id="a2">[2](#f2)</sup> You can also select text, which is automatically saved as highlighted. Such highlights can also carry notes. For text input, you can either type on the touch keyboard, tap the keys with your pen, or if you install a keyboard software that supports it, swipe over the keys with your pen. Not demonstrated in the video is the probably most convenient option: to simply connect a bluetooth keyboard. But even  when you are reading on your favourite park bench, writing comments is fast enough. The very best feature: all these comments are natively embedded in the pdf. If you later look at the same document on a laptop, using a very different software, you can just edit the annotations, delete them, add typos, etc. This was not possible in the relatively popular reMarkable 2.

Another area where the reading software in the Max3 beats this competitor, are the text navigation options. You can search for text, use bookmarks, and a very useful fast-scroll bar. To get an idea, see the second video. Although not demonstrated here, this is particularly useful if you are working with longer books, like the Husserliana, that often approach a thousand pages. 

<p align="center">
<iframe width="360" height="640" src="https://www.youtube.com/embed/Shns6KRnTPI" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

## The setup
Much of the setup relies on the freedom to install arbitrary applications from the Play store to this device - it is just a tablet running Android 9.0. This allows for example the integration of newspapers or reading apps (like Pocket). And it gives you access to a full digital library. I briefly describe how to achieve this.

### File synchronization
File synchronization works via AutoSync for Google Drive. I use this to synchronize my pdf library, which I organize with Zotero and its zotfile plugin: it is a simple folder with a good number of files named "AuthorYear_Title.pdf". I am very happy with this setup and it I could move it to a different device or operating system in a flash. 

I always found it helpful to print and read an in progress draft. The physical change in interaction really helps me to get fresh eyes on what I have written, and it stops getting distracted by small formatting changes. I guess I will keep printing my drafts now and then, but using the reader to the same end seemed to work as well. This is why, besides the Zotero folder, I also synchronize a temporary folder. 
I have defined a tiny bash function (I am using WSL1), that copies an arbitrary file into that location &nbsp; maybe useful for somebody:
```
# define environment variable:
export BOOXTEMP="/mnt/d/your/path/to/cloud/boox/temp/"

function push_to_boox {
    # copy to boox temporary folder
    echo -n "copying to $BOOXTEMP"
    echo -n ""
    cp -t ${BOOXTEMP} ${1}
    echo -n ""
}
```

### Zoo for zotero
Zoo for Zotero is an android app that allows you to access your zotero collection on an Android device. If you have set up Zotero's zotfile plugin correctly, you can just navigate your collection from this app and find any text on your device (even if you only remember the title, for example). 

### External reading light
As mentioned above, a main reason that the Boox Max 3 dropped ca. 50% in price has to do with the release of its successor, the Boox Max Lumi. The Lumi is essentially the same device, but it the first A4 reader with an integrated light. Since this is not the kind of device you'd use for reading under a blanket, I don't think it is strictly necessary.

Of course sometimes light conditions might not be ideal. If you have the money, why not just go with the Boox Max Lumi - it also comes with Android 10 instead. But besides being expensive, the Lumi seemed also very hard to get hold of.

In the spirit of getting 80% there for 2.5% of the cost, I just bought a clip-on light. It's ugly, but the whole device is not particularly beautiful either. If you're trying to look stylish while working, either the iPad or a collection of hardcover books will get you further anyway.

### Screen protector
One of the annoyances with Onyx is that they do not apply the screen protector in factory - for a device that they (used to) sell upwards of €1000! At least, a basic screen protector ships with the device. But it is so notoriously difficult to apply. Forums are full of people confessing that they just write directly on their screens, or that they ended up getting alternative protectors.

I was tempted to just skip the protector altogether, but I have to emphasize how glad I am about applying it. Besides protecting the screen from scratches, it changes the writing feel. But most importantly, it makes for a more diffuse reflection - the blank eInk display is decidedly more shiny than paper, and this was the main thing that initially curbed my enthusiasm.

Here is my unsolicited advice on applying the protector:
- find a dust free environment. Forum advice has it that the steamy air in a bathroom works well, and that's what I followed. But I don't know if my relative success was due o this.
- Really clean the tablet surface - with alcohol - before applying the screen protector. Don't wipe it dry with a paper towel, that will leave dust on the surface.
- trim the edges before applying. The protector has exactly the same size as the screen plus bezel, but it is hard to fit exactly. If the protector stands off from the bezel, it will easily peel off. With a slightly trimmed protector, application becomes more forgiving, at the price of leaving some of the bezel unprotected, which really does not matter.

### Pens and nibs
Another annoyance, which really makes the Max 3 a device that has to grow on you after unboxing, is the quality of the included pen. It is incredibly light and thin, made from a cheap plastic, and has a very hard tip.

I bought a Staedler Noris digital Jumbo, which has a good ergonomic shape and a slightly goofy (but at least in Germany, well-known) design. This improves the writing feel _a lot_, to the extent that it can compete with the reMarkable 2. To my surprise, however, this difference seemed to depend mostly on the screen protector and the nib. Putting one of the Staedler nibs into the original pen also improved the writing feel that dramatically. While writing, the original pen even seemed slightly more accurate than the Staedler pen. Since I mostly annotate PDFs and don't write much long hand, I prefer the ergonomics of the bigger pen. But it might be feasible to build something better and cheaper from the original pen by swapping the nib, adding weight, and a grip tape.


## Alternative ereaders
### Bigger is better
Many people (within a very small group) debate whether the A4 reader isn't too large. I was almost impressed enough to get an A5 device instead. But at least I am very glad I did not, because it has the following advantages:
- Sharper image. The pixel density of the A4 and A5 devices is the same. But the reading distance from an A4 device is higher, so there are more pixels in view (each pixel covers a smaller solid angle).
- No need for perfect cropping. Your image is still large enough if there is some breathing room (and that makes for more pleasant reading, as LaTeX default layout users will confirm)
- Margin space for notes
- More space for writing/drawing
- Split-screen makes sense, if you prefer to take handwritten notes in a separate document, or need to read two documents side by side.
- It is still mobile. It is not bigger than my ultrabook, fits in any bag or sleeve that you would need to carry for an A5 device anyway. It is also not heavier than a hardback

### Why not a Kindle
The kindle ecosystem determines most of what you can or cannot do. It is great for some tasks. And together with Calibre, it is possible to convert arbitrary HTML content - such as the web view of oxfordscholarship.com to ebooks for your kindle. But sometimes, things are not perfectly smooth. Reading a pdf without having to reflow a document still seems preferable. Also annotations with .epub or .mobi files are more complicated to integrate wiht other devices.

### Why not the reMarkable 2
I have tried the reMarkable 2 and returned it before getting the Max 3. My main reasons:
- smaller screen
- no Bluetooth Keyboard
- synchronization only via reMarkable cloud and Desktop application
- very tedious pdf navigation
- pdf annotations are in a bitmap layer

I think it is a nicely designed device with good hardware, and much better marketing than Onyx. The return was fine as well, I don't know if that would be more complicated for Onyx &nbsp; so if you are on the fence whether eInk is for you at all, and might be more interested in writing than reading, the reMarkable 2 might be worth a shot.

## Anticipating disappointments
I am writing a lot of negative things here, so I should maybe reiterate: you can take _all_ your books with you, into the park, and read in the sun while nothing disturbs your peaceful philosophical thinking! It is a dream and I love it. But there are a already a number of youtube channels that already give their best to create a hype for eReaders. Let me focus on some warnings instead.

- The Boox Max 3 looks much cheaper than it is.
- You will have to do a little reseach and put some effort into setting up your device, because the official documentation is quite useless. It probably helps if you enjoy figuring out technology, rather than expect everything to work out of the box.
- The case is not very good and seems even cheaper than the device - definitely not like the €40 it costs when bought individually. 
- There are reports that [Onyx violates Open Source Licences](https://www.reddit.com/r/Onyx_Boox/comments/hsn7kx/onyx_using_recent_antichina_movement_as_excuse_to/), and has done so [for years](https://www.mobileread.com/forums/showthread.php?t=277431). I really disagree with this, but I know of no alternative device that would make this setup possible.
- The Max 3 comes with an HDMI mini input, but sharing a screen in this way or via the DeskSpace Android app is too blurry to be usable. The feature is not really developed.
- The Play store gives you access to an insane number of applications, but the interface of many apps will not work well on an eInk screen. You should not assume that you can just use e.g. Adobe Reader. However, non-interactive background services, for syncing a folder or calendars, accessing zotero, or just reading on the web, work well.
- My previous experience with the Boox M96 also eroded my faith in Onyx' firmware updates. Sometimes they would introduce new bugs - so I would not install them immediately, and only after searching some forums about whether they introduce new problems.
- Onyx releases a lot of new devices in quick succession, probably at the expense of long-term support for their devices. I would not bet on the Max 3 receiving software updates in 3 years. That said, it runs fine with the latest firmware I installed in January 2021 and I don't expect to need to make any changes really.

## Bonus: emacs via Termux
The Max 3 also supports termux, which gives access to a command line with a lot of open source tools.  I managed to installed doom emacs (my writing and notetaking environment), so I could do distraction free, battery unconstrained writing on the eReader. So far, I am not using this - for small snippets, like the draft of a paragraph, synchronization is much simpler if you just write it in Google Keep for example. But in principle, the writing process could be moved to the eInk screen as well. And for somebody who is planning a DIY eInk project, termux with the whole battery of terminal tools (like git, rsync, ...) could be interesting.
<p align="center">
<iframe width="360" height="640" src="https://www.youtube.com/embed/45dnxoKx8F4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

Let me know if this was helpful, if there are omissions or errors, or if you have recommendations to add. Enjoy reading.


## Further resources
A good channel with feature demonstrations of eReaders is _My Deep Guide_. The name is apt, considering this 1h:17 [review of the Max 3](https://www.youtube.com/watch?v=SEHFkqHtu_g).
There are more eReader specific channels on youtube, but I find them often a bit too enthusiastic.


___
<b id="f1">1</b> The shipping was insured. But because I did not have individual receipts for the dozens of books, my reimbursement followed a bulk freight calculation - estimating the value of my shipment by weight, where it turns out a kilo of book is worth about €10.  [↩](#a1)

<b id="f2">2</b> Looking at Huw Price's paper "Metaphysics after Carnap: The Ghost who walks?" for this video, for the first time I noticed Price's typographic pun: a smaller-than-standard space in the middle of Carnap's name, before setting up the scenario, of a famous logical empiricist falling asleep in a traffic jam.[↩](#a2)

![Boox Max 3 in a tablet stand](/graphics/max3_portrait_web.jpg)
