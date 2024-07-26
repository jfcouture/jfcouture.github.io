---
author: jfcouture
comments: true
date: 2005-03-15 00:58:22+00:00
layout: post
link: http://jfcouture.com/2005/03/14/good-design/
slug: good-design
title: Good design
wordpress_id: 11
categories:
- Agile
- Software Engineering
---

[The Bar is Higher Now](http://www.artima.com/weblogs/viewpost.jsp?thread=42486)


<blockquote>I don't care how good you think your design is. If I can't walk in and write a test for an arbitrary method of yours in five minutes its not as good as you think it is, and whether you know it or not, you're paying a price for it.</blockquote>



In the last few months I've had the chance to code a couple of projects using test driven development, that is writing unit test before the actual code. Whenever I have to go back to code not written that way, I'm entering a world of pain. The peace of mind it provides when writing and most importantly changing code is unbelievable.

Because you want the test to be easy to write, you have to make sure the class is easy to instantiate. This generally leads to very low coupling, which is a sign of a good design.
