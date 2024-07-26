---
author: jfcouture
comments: true
date: 2007-12-16 21:38:01+00:00
layout: post
link: http://jfcouture.com/2007/12/16/installing-git-on-mac-os-x/
slug: installing-git-on-mac-os-x
title: Installing Git on Mac OS X
wordpress_id: 99
categories:
- git
---

**Note:** These instructions are for Mac OS 10.4. I don't know if they'll work with Leopard.





Installing git is easy, just compile from the source. Git svn is harder to install because it is a bunch of perl scripts that needs the svn perl bindings (it comes with git btw). Here are the steps I recommend to make sure everything works.





First, we'll install git using [Macports](http://www.macports.org/). This will take care of installing all the required perl libraries:




    
    
    $ sudo port install git-core +svn
    





However, macports installs a slightly old version of git. So I suggest [downloading](http://git.or.cz/) the latest and compiling from source.




    
    
    $ sudo make install
     # Note: watch out for the way your PATH is setup 
     # to make sure you are using this new git version
     # instead of the macports version
    $ git --version
    





Now if you try to run git svn, you might get an error about it not finding SVN/Core.pm. That means your version of subversion does not include the perl bindings (which is the standard if you installed svn with macports). I suggest you install subversion from this [package](http://downloads.open.collab.net/binaries.html) that includes the language bindings. Now you need to add this to your ~/.profile:




    
    export PERL5LIB=/usr/local/lib/svn-perl





Everything should work. Now it's time to import your svn repositories and enjoy git.
