---
author: jfcouture
comments: true
date: 2007-07-05 00:08:14+00:00
layout: post
link: http://jfcouture.com/2007/07/04/making-the-mental-switch-to-rest/
slug: making-the-mental-switch-to-rest
title: Making the mental switch to REST
wordpress_id: 52
categories:
- Rails
---

I finally played a bit with the REST part of Rails. Over the weekend, I made my first RESTful web app. How did it go? I don't know. I don't think I've yet made the mental switch. There's a few things that bug me about REST, and I'm not sure I can put it in words yet.

I think there's "REST" and "Rails REST". The way Rails does REST seem to be a subset of REST, or at least it puts more constraints on how you should do it.

The one thing that bothers me the most is the respond_to and how you can handle different formats. Yes it is nice to be able to reuse the same action and send back XML or CSV or a basic html representation of the information. But when it comes to the actual UI of your application, the html, the forms, the navigation, I don't want my user to interact with the application the same way a machine would.

Maybe I should investigate a bit more the [RADAR architecture](http://pragdave.pragprog.com/pragdave/2007/03/the_radar_archi.html) as described by Dave Thomas. The idea is to have the html application be another layer on top of your resources.
