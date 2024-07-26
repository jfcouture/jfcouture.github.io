---
author: jfcouture
comments: true
date: 2008-01-20 21:44:45+00:00
layout: post
link: http://jfcouture.com/2008/01/20/how-to-set-up-a-git-server/
slug: how-to-set-up-a-git-server
title: How To Set Up A Git Server
wordpress_id: 102
categories:
- git
---

Git does not require a special "server" to run. For example, if you are on a local network, you can just put the repository on a shared network drive. Git does not handle the security. You configure the read/write access on the folder. I'm not an expert in system administration so I'm going to suggest some options and provide links that I found helpful:







  * [Ssh](http://www.openssh.com/) is you friend for security. If you do not want to provide shell access to everyone, you can setup [one git user and use ssh keys](http://eagain.net/blog/2007/03/22/howto-host-git.html) to provide access. If you go that route, take a look at [gitosis](http://scie.nti.st/2007/11/14/hosting-git-repositories-the-easy-and-secure-way), which is a bunch of python scripts that automates part of administering that kind of setup. Gitosis gives you a git repository to configure access and projects. It's very nice.



  * Another option is [through http](http://www.kernel.org/pub/software/scm/git/docs/howto/setup-git-server-over-http.txt). You need webdav for that.



  * [Git daemon](http://www.kernel.org/pub/software/scm/git/docs/git-daemon.html) comes with git and is perfect if you only need to quickly give public read access.



  * There are couple of git hosting site that are popping up. Check out [repo.or.cz](http://repo.or.cz/) and [Github](http://github.com/) (invitation only for now but has a sexy look).


