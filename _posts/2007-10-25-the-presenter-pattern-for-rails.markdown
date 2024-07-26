---
author: jfcouture
comments: true
date: 2007-10-25 01:37:57+00:00
layout: post
link: http://jfcouture.com/2007/10/24/the-presenter-pattern-for-rails/
slug: the-presenter-pattern-for-rails
title: The Presenter Pattern For Rails
wordpress_id: 92
categories:
- Rails
- Software Engineering
---

### The problem:





Having logic in your view is bad. Putting some in the helpers can help. Some methods can be put on the model. Sometimes, your view involves a couple of models, the helpers get bigger, you're not sure on which model to put a method as it needs data on a few of the associations. The view is getting ugly, you have to go through pages of helper methods to find things. You're feeling dirty. 





### The solution:





Move all the methods related to one of the view to a class (the presenter). Create it in the controller by passing it all the objects it needs to manipulate. Change your view to only call methods on your @presenter.





### Implementation:





You will probably want to have access to the ActionView::Helpers::* in your presenter so it can useful to declare a base presenter class you will inherit from like this:




    
    <code><span style="color:#CC7833">class </span><span class="class">Presenter</span>
      <span class="ident">include</span> <span style="color:#DA4939">ActionView</span><span class="punct">::</span><span style="color:#DA4939">Helpers</span><span class="punct">::</span><span style="color:#DA4939">TagHelper</span>
      <span class="ident">include</span> <span style="color:#DA4939">ActionView</span><span class="punct">::</span><span style="color:#DA4939">Helpers</span><span class="punct">::</span><span style="color:#DA4939">FormHelper</span>
      <span class="ident">include</span> <span style="color:#DA4939">ActionView</span><span class="punct">::</span><span style="color:#DA4939">Helpers</span><span class="punct">::</span><span style="color:#DA4939">FormTagHelper</span>
      <span class="ident">include</span> <span style="color:#DA4939">ActionView</span><span class="punct">::</span><span style="color:#DA4939">Helpers</span><span class="punct">::</span><span style="color:#DA4939">FormOptionsHelper</span>
      <span class="ident">include</span> <span style="color:#DA4939">ActionView</span><span class="punct">::</span><span style="color:#DA4939">Helpers</span><span class="punct">::</span><span style="color:#DA4939">DateHelper</span>
      <span class="ident">include</span> <span style="color:#DA4939">ActionView</span><span class="punct">::</span><span style="color:#DA4939">Helpers</span><span class="punct">::</span><span style="color:#DA4939">JavascriptHelper</span>
      <span class="ident">include</span> <span style="color:#DA4939">ActionView</span><span class="punct">::</span><span style="color:#DA4939">Helpers</span><span class="punct">::</span><span style="color:#DA4939">AssetTagHelper</span>
      
      <span style="color:#CC7833">def </span><span class="method">intialize</span><span class="punct">(</span><span class="ident">controller</span><span class="punct">)</span>
        <span style="color:#D0D0FF">@controller</span> <span class="punct">=</span> <span class="ident">controller</span>
      <span style="color:#CC7833">end</span>
    <span style="color:#CC7833">end</span></code>







Some helpers need the @controller to do their magic.





### Success stories:





I've used this approach two times now. Last time, I had a view that showed deeply nested data (parent => children => children => children). There were a bunch a checkboxes that needed to be all checked/unchecked at the same time depending on which element was clicked. Putting all the methods required to generate the checkboxes with ids and class and restoring that from the params in case of an error was ugly. However, that ugliness was nicely sealed in a class that prevented infection of the rest of the code.





### Further links:





  
  * [Jay Fields Thoughts: RailsConf Europe 07: Presenter Links](http://blog.jayfields.com/2007/09/railsconf-europe-07-presenter-links.html)

  
  * [Simple Presenters](http://blog.caboo.se/articles/2007/8/23/simple-presenters)

  
  * [Model View Presenter Pattern](http://www.martinfowler.com/eaaDev/ModelViewPresenter.html)

  
  * [Jay Fields Thoughts: Rails: Rise, Fall, and Potential Rebirth of the Presenter Pattern](http://blog.jayfields.com/2007/10/rails-rise-fall-and-potential-rebirth.html)

  
  * [Giles Bowkett: My Version Of Rails Presenters](http://gilesbowkett.blogspot.com/2007/10/my-version-of-rails-presenters.html)

  




### Warning:





The approach I described here may not fit the original presenter pattern as described in those other links. What's important here is, if your view is getting ugly, hard to test, you have too many helpers, or the code is starting to smell, you can move stuff to a new class. This may seem evident, but I sometimes feel people using rails forget that you can do stuff "outside" of the way rails normally structure a project. Also note that the presenter pattern is definitely not something you need for every project. 
