---
author: jfcouture
comments: true
date: 2007-09-09 17:47:15+00:00
layout: post
link: http://jfcouture.com/2007/09/09/metaprogramming-dsl-considered-harmful/
slug: metaprogramming-dsl-considered-harmful
title: Metaprogramming + DSL Considered Harmful
wordpress_id: 80
categories:
- Agile
- Rails
- Ruby
- Software Engineering
---

[The Rails Edge: Quotes and Notes](http://blogs.pathf.com/agileajax/2007/08/the-rails-edge-.html) is a very interesting collection of quotes from the rails edge conference. Two in particular caught my attention:





<blockquote>“Metaprogramming + DSLs is the Ruby equivalent of Design Patterns in the Java world”
  — Chad Fowler. Fowler’s point here was more about the buzz and hype, just like there was a time in the early 2000s when every Java programmer wanted Design Patterns whether or not they were needed, Fowler sees a similar rush to add DSLs to Ruby programs.</blockquote>





<blockquote>“If programmers, on average, were able to write parsers and compilers, Ruby on Rails would not have taken off”
  — Stuart Halloway</blockquote>





This is something I've noticed a lot recently: every plugin that gets released is a DSL! or it uses a cool metaprogramming trick! That's nice, but was it really needed? And can we really talk about a 'language' when your plugin adds two simple commands to a controller?





I guess it's a rite passage when learning ruby to write something using metaprogramming. The problem is when you start using it for everything, just like when you add patterns after patterns to your code, just because.






Again, this is a case of using the **right tool for the right job**. Metaprogramming is a power tool that is useful some time.






Here are other quotes that I like, as they echo the discussion I had with Fred Brunel at the last [book club](http://jfcouture.com/2007/08/29/montreal-web-development-book-club-august-edition/) about process:






<blockquote>“The right process is always ‘not quite enough process’”
  — Stuart Halloway
</blockquote>





<blockquote>“Do the dumbest, simplest thing that almost works”
  — Stuart Halloway, on process
</blockquote>





<blockquote>   “The traditional view, with sixteen pounds of documentation, introduces a single point of failure in the process, understanding the problem domain”
      — Dave Thomas
</blockquote>





<blockquote>“Getting a specification involves bullying the customer”
      — Dave Thomas
</blockquote>
