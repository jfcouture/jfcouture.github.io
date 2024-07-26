---
author: jfcouture
comments: true
date: 2007-09-20 03:59:08+00:00
layout: post
link: http://jfcouture.com/2007/09/19/web-architecture-rest-rails-the-universe-and-everything/
slug: web-architecture-rest-rails-the-universe-and-everything
title: Web Architecture, REST, Rails, the Universe and Everything
wordpress_id: 84
categories:
- Rails
- REST
- Software Engineering
---

The last part is [easy](http://en.wikipedia.org/wiki/42_(number)). Now what is architecture as related to software development, that's a much harder problem (42 is still a good answer of course). I think I just read the best explanation of what it is.





[Roy Fielding](http://www.ics.uci.edu/~fielding/)(inventor of [REST](http://en.wikipedia.org/wiki/Representational_State_Transfer)) gave a talk at [RailsConf Europe](http://www.railsconfeurope.com/) entitled "[The Rest of REST](http://conferences.oreillynet.com/presentations/railsconfeurope07/re7_royfielding.pdf)". The last slide really sums it best:




<blockquote>use principled design:

> 
> 

>   * identify desired architectural properties 
> 

>   * constrain behavior to induce properties 
> 

>   * compensate for the inevitable design trade-offs
> 

</blockquote>





I think this is the best way to really understand why [constraints are liberating](http://gettingreal.37signals.com/ch03_Embrace_Constraints.php). When designing, you choose the properties important to your application (whether it be efficiency, scalability, maintainability or any other -ilities). The architecture will codify a set of constraints that should lead to your application having these properties. These constraints free you from having to constantly think about any of the properties, as long as you respect the architectural guidelines.





An example from the slides: Constrain interactions to be stateless. This simplifies the server, improves scalability and reliability. However, it degrades efficency. Checkout the slides as Roy gives very detailed info on the advantages and tradeoffs of using a REST architecture. Seriously, these [slides](http://conferences.oreillynet.com/presentations/railsconfeurope07/re7_royfielding.pdf) are gold. I will read them again and again over the next few weeks.
