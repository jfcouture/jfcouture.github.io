---
author: jfcouture
comments: true
date: 2007-12-12 23:50:07+00:00
layout: post
link: http://jfcouture.com/2007/12/12/the-guerilla-guide-to-git-how-to-start-using-git-even-if-your-team-is-on-svn/
slug: the-guerilla-guide-to-git-how-to-start-using-git-even-if-your-team-is-on-svn
title: 'The Guerilla Guide To Git: How To Start Using Git, Even If Your Team Is On
  Svn'
wordpress_id: 98
categories:
- git
---

I've been using [git](http://git.or.cz/) for three months now and it has had zero impact on my team. They weren't even aware I was using it for the first few weeks. That means, **you** can start using it now, for your personal development, without having to convince anybody.





Git comes with a svn wrapper. You can import your svn repository to a local git repository. You then get all the advantages of git: easy branching/merging, offline operation(very useful if you work with a laptop), etc.




    
    
    $ git svn clone http://path/to/svn -T trunk -t tags -b branches
    




This command will import all the revisions from svn and create branches in your git repository (one for trunk, and one for all your branches). You will be on a branch master (linked to trunk) and can start working. You commit normally to your repository.





When you are ready to send your changes back to svn:



    
    
    $ git svn rebase # (equivalent to svn update)
    $ git svn dcommit # (equivalent to svn commit)
    




Rebase works by reverting your changes, getting the latest revisions from svn, and then reapplying your changes. You resolve any conflicts (if there any). The last command then pushes your changes to svn for your team to enjoy.





Those are the three commands you need to know to use git with svn.





### Caveats




Svn:externals are not supported. I suggest you use [piston](http://piston.rubyforge.org/) to handle them.




Check out the [git svn docs](http://www.kernel.org/pub/software/scm/git/docs/git-svn.html) for a few more things to watch out for.





### Conclusion




Now that your team has seen you using git successfully for weeks, it will be much easier to get them to switch!
