---
author: jfcouture
comments: true
date: 2005-03-15 01:09:23+00:00
layout: post
link: http://jfcouture.com/2005/03/14/mf-bliki-dynamictyping/
slug: mf-bliki-dynamictyping
title: Tests and rails
wordpress_id: 12
categories:
- Agile
- Rails
- Ruby
- Software Engineering
---

[MF Bliki: DynamicTyping](http://martinfowler.com/bliki/DynamicTyping.html)


<blockquote>I discovered that in the presence of SelfTestingCode, most bugs that static types would have were found just as easily by the tests.</blockquote>



Last night I was playing with rails trying to understand some of the features. Old habits kicked in. I did not write some tests and got bitten once again. Lost almost an hour on a few stupid typos. As Martin Fowler explains, tests are more important in a dynamic typed language as the compiler won't catch some errors for you. Fortunately, rails supports testing [right out of the box](http://manuals.rubyonrails.com/read/book/5).
