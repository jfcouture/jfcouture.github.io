---
author: jfcouture
comments: true
date: 2008-04-08 02:14:48+00:00
layout: post
link: http://jfcouture.com/2008/04/07/its-time-to-revisit-your-assumptions-about-vcs/
slug: its-time-to-revisit-your-assumptions-about-vcs
title: It's Time To Revisit Your Assumptions About VCS
wordpress_id: 105
categories:
- git
---

You might have heard about distributed version control systems recently, for example [git](http://git.or.cz/). There are a lot of articles popping up left and right about DVCS. What I find interesting about this is that version control has again become something to talk about. This is very healthy as version control is such an important tool for software developers.





When I started using using subversion five years ago, version control faded to the background. Subversion greatest strength is its simplicity. After a while, you get used to its quirks and it just works. Sure, some operations are painful, like merging back a branch, but you learn how to do it (and try to minimize to number of times you have to do it).





But five years is a pretty long time in computing terms. Maybe something better has come along. Maybe the reasons you chose something five years ago don't hold anymore. This applies to everything. Sometimes you come across a company policy that looks stupid. At the time the decision was taken, it might actually have made sense. But things changed (as they tend to) and nobody took the time to check if the assumptions used to make the decision were still true today.





I suggest you use all the hype around git, and the discussions it generates, to revisit, to question all your assumptions about what is version control and what it can do for you. Is version control about sharing code with other developers and having some kind of history and backup? That's something that, yes, it provides, but it can do so much more.





Have you ever used a VCS that required you to lock a file before editing, to avoid conflicts if two developers edited the file at the same time? If you've used any system that doesn't require it, you just know that it's a not a real problem. However, how do you explain it to the developer that is convinced that it is a very real problem? That's the problem I have with git right now after using it for six months. I don't how to convince people to try it when they raise objections. I can only say that it's awesome and that going back to subversion from git would be more painful for me than going back to locking file from subversion.
