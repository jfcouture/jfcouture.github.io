---
author: jfcouture
comments: true
date: 2007-07-26 20:06:47+00:00
layout: post
link: http://jfcouture.com/2007/07/26/a-three-days-experiment-using-delicious-for-my-bookmarks/
slug: a-three-days-experiment-using-delicious-for-my-bookmarks
title: A Three Days Experiment Using Del.icio.us For My Bookmarks
wordpress_id: 63
categories:
- api
- bookmarks
- delicious
- productivity tips
---

I have 880 bookmarked pages in Firefox. 200 of them are in a folder named rails. I can't find anything anymore. It is usually faster to google for what I want.  It's time for summer cleaning. It's also time to move to [delicious](http://del.icio.us/): I want my bookmarks available anywhere and I want to use tags.

I signup and install the [firefox plugin](http://del.icio.us/help/firefox/extensionnew). It can import your bookmarks. Better, there's an option to automatically add the most popular tag. Talk about a great way to harness the wisdom of crowds! One problem: it only adds the most popular tag when I want all of them. Tags are useful only when you can put more than one (otherwise you are back to using folders)! I wrote a small ruby script to add all popular tags to my bookmarks using the [api](http://del.icio.us/help/api/) (and [this](http://del.icio.us/help/json/url) to get the most popular tags).

**The good**



	
  1. My bookmarks are now online and a bit better organized thanks to tags (ex: I can see all rails plugins related to databases).

	
  2. When adding new bookmarks, the firefox plugin suggests the most popular tags. That's very nice as it is not always easy to find good tags.

	
  3. I can delete all my bookmarks in firefox. I now only keep the bookmark toolbar with links to sites I visit daily and links to online tools such as gmail, google reader, dictionary, etc. It is a breath of fresh air to have it so clean.


**The bad**



	
  1. The Firefox plugin is sloooooooooow. It is almost unusable. It is better to search on the delicious site.

	
  2. A big problem with bookmarks is actually a problem related to the way a lot of websites are built: the title isn't correctly set. Or if it is set, the title is not very good at telling you what the page is all about. Even with tags, I have to actually open the page to know what it is about.


I'm not entirely sold yet, but I will continue the experiment for a couple of weeks.
