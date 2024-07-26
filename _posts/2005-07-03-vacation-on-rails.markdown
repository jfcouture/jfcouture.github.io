---
author: jfcouture
comments: true
date: 2005-07-03 23:32:18+00:00
layout: post
link: http://jfcouture.com/2005/07/03/vacation-on-rails/
slug: vacation-on-rails
title: Vacation on Rails
wordpress_id: 23
categories:
- Rails
---

I just got back from a 3 days fishing trip. It ended my week of vacation, and once again, I barely did anything that I wanted to do. It happens every time. I dress a list of things to occupy the week and can only finish a third of them.

Of the things I did do though is find some time to play with Rails. I bought the beta book [Agile Software Development With Rails](http://www.pragmaticprogrammer.com/titles/rails/index.html). I went through the tutorial (about 100 pages) and I remembered so clearly why I fell in love with Rails. The framework keeps the boring stuff out of the way and allows you to concentrate on the functionality of your application. It's just fun seeing the application rapidly come to life.

There are a few things that bug me right now, but they probably come from my lack of experience with Ruby and the lack of a good IDE. Debugging can be hard, and typos are hard to find. For debugging I recommend you use Webrick as the console leaves a trace of call made and shows a stack trace when an exeption is thrown. However, on my computer, Webrick is just too slow to allow to rapidly see the changes just made so I prefer to use Apache with FastCGI. In fact, I think it's a must if you want to keep your sanity.

I had some problem with the tutorial at some point as the book documents a version of Rails that isn't out yet. A quick gems install --source gems.rubyonrails.org fixed that. I was lucky with that part, as I bought the book on monday and a new update was released on tuesday night. The email that I got to inform me of the update mentioned it.
