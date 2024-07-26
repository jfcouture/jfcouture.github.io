---
author: jfcouture
comments: true
date: 2007-07-06 19:24:53+00:00
layout: post
link: http://jfcouture.com/2007/07/06/rethinking-design-patterns/
slug: rethinking-design-patterns
title: Rethinking Design Patterns
wordpress_id: 53
categories:
- Software Engineering
---

[Jeff Atwood](http://www.codinghorror.com/) has a good post entitled [Rethinking Design Patterns](http://www.codinghorror.com/blog/archives/000899.html).


<blockquote>It's certainly worthwhile for every programmer to read Design Patterns at least once, if only to learn the shared vocabulary of common patterns.</blockquote>


No matter what you think of design patterns, you have to read the book at least one time. I remember a talk with a fellow programmer, explaining a part of his design: "so you this object inheriting from that one, and implementing that one interface, and blabla blabla object object blabla more objects etc...". After a couple of minutes, I said "so basically, you have a composite". "Yes". As a design gets bigger and bigger, it's important to have a bigger vocabulary than just class this, object this.

But there are problems with patterns as Jeff continues:


<blockquote>If you find yourself frequently writing a bunch of boilerplate design pattern code to deal with a "recurring design problem", that's not good engineering-- it's a sign that your language is fundamentally broken.

In his presentation "Design Patterns" Aren't, Mark Dominus says the "Design Patterns" solution is to turn the programmer into a fancy macro processor.</blockquote>


Don't Repeat Yourself. If the same pattern happens again and again, maybe you should find a way to automate it? A good language can help here. I hear a lot more about patterns in the java world than in the ruby world. Why? You have no choice but to code the pattern and it's boilerplate every time in java. In ruby, you do it one time with a bit of metaprogramming. The ruby standard library provides a library for the singleton. "Include singleton" in your class and you're done. Other design patterns are there to cover a flaw in the language. For example, you don't need visitors if you use lisp because of multiple dispatch.


<blockquote>How can you distribute responsibility for design through all levels of a large hierarchy, while still maintaining consistency and harmony of overall design? This is the architectural design problem Alexander is trying to solve, but it's also a fundamental problem of computer systems development.</blockquote>


I will have to read the Alexander book. That's a much more interesting problem than something you can abstract in a good language.
