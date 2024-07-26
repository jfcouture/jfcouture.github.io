---
author: jfcouture
comments: true
date: 2007-12-07 02:52:51+00:00
layout: post
link: http://jfcouture.com/2007/12/06/montreal-on-rails-deployment-edition/
slug: montreal-on-rails-deployment-edition
title: Montreal On Rails, Deployment Edition
wordpress_id: 96
categories:
- montreal
- Rails
- social
---

Deployment, deployment, deployment. Ok not three, but just two awesome presentations on deployment.





### Carl Mercier, Rails Deployment Option





Carl compared the different hosting solutions available for Rails. You want to avoid shared hosting and start with a Virtual Private Server(VPS) so you get enough RAM to run a couple of mongrels. Carl has had good experiences with [Slicehost](http://www.slicehost.com/). A dedicated server is the next step if you need more power, but you might want to skip it and go directly to the next option.






[Amazon EC2](http://aws.amazon.com/ec2). The game changer. Take all the advantages of server virtualization and add on demand power when you need to scale. Check out [EC2 on Rails](http://ec2onrails.rubyforge.org/). It contains a complete image already setup for rails. Also check out [Rightscale](http://rightscale.com/). They have a nice dashboard to help you manage your instances.






### Mehdi Adda, Setting Up Your Server





Mehdi showed how to setup mongrel+nginx+seesaw+monit. [Mongrel](http://mongrel.rubyforge.org/) acts as the app server. [Nginx](http://nginx.net/) is a lightweight and fast web server. [Seesaw](http://en.wikipedia.org/wiki/Seesaw) allows you to restart your mongrel cluster with no down time and always only one version of your app running. [Monit](http://www.tildeslash.com/monit/) supervises your processes and can kill them if they have a problem, restart them if they crash or send you a warning email if you're running out of disk space.






Check out Mehdi's slides. They are very thorough on the steps to setup each part. You can get the slides on the [Montreal On Rails](http://www.montrealonrails.com/past-presentations/) website.






### Next edition





The next is scheduled for the middle of January. I'm wondering if people would be interested in a presentation on [git](http://git.or.cz/). It is not strictly rails related, but should be of interest to all rails developer. I've been using it for almost three months and it rocks. In fact, I'm going to make a prediction: 80% of all rails developer will switch to git before the end of 2008.
