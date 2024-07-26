---
author: jfcouture
comments: true
date: 2007-07-21 17:12:40+00:00
layout: post
link: http://jfcouture.com/2007/07/21/capistrano-rules/
slug: capistrano-rules
title: Capistrano Rules
wordpress_id: 60
categories:
- capistrano
- dreamhost
- Rails
- Ruby
---

[Capistrano](http://www.capify.org/) is a framework for deploying Rails application (you can do more with it, but it comes with built-in tasks for rails). How does it work? It connects to the server through SSH, checks out the last version of your app from your subversion repository in a new directory (releases/{date}), runs migration (optional), symlinks the directory to /current. You're up and running after simply running "cap deploy".

It supports rollback when something goes wrong. Setup is really simple (for dreamhost, you can find info in the [wiki](http://wiki.dreamhost.com/Capistrano)). It supports more complex deployment scenarios to multiple machines (multiple app servers with one db server for example). It's easily extensible if you need to add custom steps to your deployment procedure. Let's say you have a directory for uploads, you can create a task to properly link to the new version.

It was my first time with [Capistrano](http://www.capify.org/) because I was working on Windows before. It is such a time-saver to have a great and powerful tool like this for deployment (compared to writing your own scripts). I think I'm in love.
