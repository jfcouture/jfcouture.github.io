---
author: jfcouture
comments: true
date: 2007-11-08 02:02:06+00:00
layout: post
link: http://jfcouture.com/2007/11/07/montreal-on-rails-4th-edition-report/
slug: montreal-on-rails-4th-edition-report
title: Montreal On Rails, 4th Edition Report
wordpress_id: 93
categories:
- montreal
- Rails
- social
---

Yet another great [Montreal On Rails](http://www.montrealonrails.com/) last night, again at the Standout Jobs office.





### JRuby on and off Rails, by Mathieu Martin





[JRuby](http://jruby.codehaus.org/) is an interesting project in many regards. Whether you already have a huge investments in Java, need one of its many libraries, want a faster VM (not for long), prefer to write a performance sensitive part of your app in Java over C, JRuby has something for you.





It can be tough to follow the development of JRuby and [Mathieu](http://webmat.wordpress.com/) did a great job of bringing everyone up to speed on the current state of JRuby and where it's going. I learned that even C libraries will soon be usable (they just need a small wrapper.)





There remains some small compatibility issues between JRuby and the official ruby, so you need to test your app to see if everything is working for you.





The only thing that bugs me is when I hear that deployment is easier. I don't think copying a war file is easier than running cap deploy. Yes you have to make your cap recipe and configure your server, but I hear that this is still easier than installing something like Tomcat.





### acts_as_state_machine, Alain Pilon





[acts_as_state_machine](http://elitists.textdriven.com/svn/plugins/acts_as_state_machine/) is a great little plugin that more people should know about. [Finite state machines](http://en.wikipedia.org/wiki/Finite_state_machine) are very useful to model lots of thing. The plugin provides a way to define states, events that change the state and actions when that happens. FSM are simple to understand and simple to verify their correctness.





### Comatose, Sylvain Carle





[Comatose](http://comatose.rubyforge.org/) is another nifty plugin that gives you basic Content Management System(CMS) functionality (create, edit pages and history of modifications). [Sylvain Carle](http://www.afroginthevalley.com/) explained how to use it and how easily they integrated it for the [Praized Media](http://praizedmedia.com/) website and in another of their projects in two days.
