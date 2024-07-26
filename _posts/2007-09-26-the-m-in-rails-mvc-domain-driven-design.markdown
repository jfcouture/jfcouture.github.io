---
author: jfcouture
comments: true
date: 2007-09-26 01:23:53+00:00
layout: post
link: http://jfcouture.com/2007/09/25/the-m-in-rails-mvc-domain-driven-design/
slug: the-m-in-rails-mvc-domain-driven-design
title: 'The M in Rails'' MVC: Domain Driven Design'
wordpress_id: 90
categories:
- Agile
- Book
- Rails
- Ruby
- Software Engineering
---

One of the best books I've read about design is [Domain Driven Design: Tackling Complexity in the Heart of Software](http://amazon.ca/dp/0321125215), by [Eric Evans](http://domainlanguage.com/about/ericevans.html). [InfoQ](http://www.infoq.com/) has a small ebook called [Domain Driven Design Quickly](http://www.infoq.com/minibooks/domain-driven-design-quickly) that provides a nice summary of the book. It was a good refresher for me as I read DDD about three years ago.





So [What is Domain Driven Design?](http://domainlanguage.com/ddd/index.html) Read the link to have a good overview. Here are the two most important points:






  * Focus on modeling the **domain** and domain logic of your application.


  * Build a "**Ubiquitous Language**" that is used by all the team (from domain experts to analysts to developpers).





The most interesting part of the book for me was the patterns presented as the basic building blocks of a model-driven design: Layered Architecture, Entities, Value Objects, Services, Modules, Aggregates, Factories, Repositories. These are all very simple but fundamental patterns in software development. These are types of objects that are present in all designs. Understanding the difference between a value object and an entity is crucial and can help simplify a design.





The book also discusses the importance of iterative design, the importance of incorporating back what you learned about the domain in the model as you iterate and how to preserve the integrity of the model. There is a good discussion of ways of separating the model as the team gets bigger.





### The value of this book for a Rails developer





Ever heard about [skinny controller, fat model](http://weblog.jamisbuck.org/2006/10/18/skinny-controller-fat-model)? This is THE book about building a rich model.





However, it really depends on the type of application you're building. Most Rails application are mostly concerned about CRUD operations without too much logic behind. You won't get out much from this book.





But if you're working on a business app with a lot of business logic, then this is a must-read.





The ebook also has a small interview with the author. He highlights the expressiveness of ruby and mentions that DSLs are probably the next big step in Domain Driven Design.
