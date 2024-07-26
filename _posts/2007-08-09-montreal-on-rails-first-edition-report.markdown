---
author: jfcouture
comments: true
date: 2007-08-09 00:38:26+00:00
layout: post
link: http://jfcouture.com/2007/08/08/montreal-on-rails-first-edition-report/
slug: montreal-on-rails-first-edition-report
title: Montreal On Rails First Edition Report
wordpress_id: 68
categories:
- montreal
- Rails
- social
---

Tuesday night saw the birth of the [Montreal On Rails](http://www.montrealonrails.com/2007/08/07/debrief-first-meeting/) user group in a small room on the Mcgill campus. It was a lot of fun.

The first presentation was by [Marc-André Cournoyer](http://macournoyer.wordpress.com/2007/08/08/how-was-montreal-on-rails/), [Standout Jobs](http://standoutjobs.com/) Ruby Guru, entitled "How to make your tests faster".
Marc-André started with a very funny introduction. I don't know how to describe his intro. He should turn it in a video for all to see. First part was a demonstration of caching results from external apis (he used twitter as an example) to a file to make tests go really fast on your development machine. You then add a flag so the build machine uses the actual api. You get the best of both worlds: fast tests when developping, but you also validate that the api didn't change. I just started a project monday that is gonna connect to 3 apis, so the presentation was very timely. 

The second part was about a plugin he is developping called InactiveRecord to stub out the access to the database for your test. You can find the slides to his presentation along with the code [here](http://macournoyer.wordpress.com/2007/08/08/how-was-montreal-on-rails/).

Second presentation was from [Carl Mercier](http://blog.carlmercier.com/) of [Karabunga](http://karabunga.com/). It was a small tutorial on [HAML](http://haml.hamptoncatlin.com/), a templating engine for Rails. You can play online with HAML [here](http://lab.hamptoncatlin.com/play/with/haml). The latest version released a couple of weeks ago seems to have fixed a lot of performance problem (30% slower than rhtml instead of 1000% slower). I will have to give it another try soon, along with [sass](http://haml.hamptoncatlin.com/docs/sass), which is haml for css.

Suggestions for improvements:



	
  * Bigger room for more people, but also more open space to make it easier to socialize, and a room where donuts are allowed ;)

	
  * Wiki on [montrealonrails.com](http://www.montrealonrails.com) so people can post suggestions for topics that would interest them for presentations

	
  * Maybe we can have a round of quick presentation (2-5 mins) if let's say you want to present a small plugin or a ruby trick. This could help orient discussions after the main presentation. It would also allow more people to talk and present themselves, in a less intimidating way than a full blown presentation.

	
  * Maybe someone is crazy enough to want to videotape the presentations?



I can't wait for the next edition!
