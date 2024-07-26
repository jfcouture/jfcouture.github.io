---
author: jfcouture
comments: true
date: 2008-04-03 02:15:25+00:00
layout: post
link: http://jfcouture.com/2008/04/02/rails-moving-to-git-how-to-really-understand-and-master-git/
slug: rails-moving-to-git-how-to-really-understand-and-master-git
title: 'Rails Moving To Git: How To Really Understand And Master Git'
wordpress_id: 104
categories:
- git
- Rails
---

It appears that [Rails will switch to git](http://weblog.rubyonrails.com/2008/4/2/rails-is-moving-from-svn-to-git) real soon. Nice! However, it means confusion for developers used to svn. You might find a few tips on this blog to help you get started, but right now I want to give you the secret to git mastery:





You need to think in terms of how you want to modify your graph. My what you say?!? A git repository is a [directed acyclic graph](http://en.wikipedia.org/wiki/Directed_acyclic_graph) of commits (the nodes). Huh?? Read this article: [Git for Computer Scientists](http://eagain.net/articles/git-for-computer-scientists/). Do not continue reading before you understand that article. Everything falls into place when you understand that all git commands manipulate these four basic structures: blobs, trees, commits and tags.





From now on, before typing a git command in the shell, try to picture in your head how you want your repository to look after the command. Your best friend is gitk for visualization (use the --all option to see all branches). Run it before and after each command you do with git. Here is what you should be thinking when using these commands:





  
  * git commit: I am creating a new node in my graph, linked to the current node. 

  
  * git branch branch_name: I am tagging a node with a name.

  
  * git merge: I am creating a new node that will link two parents nodes, one for each branch I am merging (could be more than two).

  
  * git fetch remote_repos: I am adding all the nodes from a distant repository to my graph.

  
  * git push: I am sending all the nodes I created to a distant repository.

  
  * git pull: I want to fetch all remote nodes AND merge.





Once you think like this, "advanced" git stuff becomes trivial. For example, this morning one coworker realized that his last three commits actually belonged to a branch. Try to visualize the solution. When you think about it, nothing has to change about the actual graph, just which nodes the tag (the branch name) needs to point at. So you just create a branch where you are, on the last commit, and then you can use the reset command to move back the other branch to the correct commit.





That's the core of git. There are maybe two other things to worry about when using git. The first is the [index](http://www.kernel.org/pub/software/scm/git/docs/tutorial-2.html), which is sort of a staging area where you prepare your commits. The other thing is the way git configuration works and the way it names and references branches (and the special reference HEAD) and remote repositories. Check out the [git user manual](http://www.kernel.org/pub/software/scm/git/docs/user-manual.html#understanding-commits).
