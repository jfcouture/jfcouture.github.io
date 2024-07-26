---
author: jfcouture
comments: true
date: 2007-08-18 18:29:08+00:00
layout: post
link: http://jfcouture.com/2007/08/18/installing-ruby-on-rails-on-a-brand-new-mac/
slug: installing-ruby-on-rails-on-a-brand-new-mac
title: Installing Ruby on Rails on a Brand New Mac
wordpress_id: 70
categories:
- mac
- Rails
---

I just changed my iMac G5 to a MacBook. There are lot of instructions on installing Ruby and Rails on a Mac on the net, some of them not quite up to date. Here is what I find to be the easiest way to do it.





  * Pop your Mac OS X install disc 1 and install the xcode tools. (this installs an old version of ruby)



  * Download and install [MacPorts](http://www.macports.org/)


  * open terminal:

    
    sudo nano /etc/profile


Prepend /opt/local/bin: to PATH, so it reads:

    
    PATH="/opt/local/bin:/bin:/sbin:/usr/bin:/usr/sbin"


This is to make sure the new version we are about to install will get used instead of the old one.



  * Make sure MacPorts is up to date:

    
    sudo port selfupdate





  * Install ruby and rubygems:

    
    
    sudo port install ruby
    sudo port install rb-rubygems
    ruby -v


This last command should give 1.8.6. If you see 1.8.2, this means it is still using the version installed from the OS X cd. Make you correctly updated your PATH.



  * Install Rails:

    
    sudo gem install rails -y






You might also want to install subversion right now using ports:

    
    sudo port install subversion



		
(Note: at the time of writing, Rails is at version 1.2.3 and Ruby at 1.8.6. )
