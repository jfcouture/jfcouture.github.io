---
author: jfcouture
comments: true
date: 2005-04-24 21:11:39+00:00
layout: post
link: http://jfcouture.com/2005/04/24/2-weeks-with-aspnet/
slug: 2-weeks-with-aspnet
title: 2 weeks with ASP.Net
wordpress_id: 20
---

I inherited some of the worst code I have ever seen. Part of the problem, according to the original coder, is ASP.Net strange ways of doing things. The real problem is that he didn't really try to understand how the framework actually works. This led to him creating a method called EnsureStart() that is the first thing called inside every method for example.

Anyway, in two weeks, I refactored most of his code to make it understandable, have the intialization happen only in one place. I think the biggest problem with ASP.Net right now is the magic is does automatically when you create your controls in the web form with the Visual Studio designer. Once you start to add dynamic controls, things start to get messy, as the magic is not done for you, and you have to make sure you recreate them every time. Also, on your page_load event, your dynamic controls might not all be loaded. This generally means that you do not have access to the new values entered by the user yet.

After two weeks, I cannot say that I'm impressed, but it is definitely less bad than what most people told me.
