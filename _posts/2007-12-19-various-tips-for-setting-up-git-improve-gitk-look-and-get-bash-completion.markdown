---
author: jfcouture
comments: true
date: 2007-12-19 01:40:04+00:00
layout: post
link: http://jfcouture.com/2007/12/18/various-tips-for-setting-up-git-improve-gitk-look-and-get-bash-completion/
slug: various-tips-for-setting-up-git-improve-gitk-look-and-get-bash-completion
title: 'Various Tips For Setting Up Git: Improve Gitk Look And Get Bash Completion'
wordpress_id: 100
categories:
- git
---

You just installed [git](http://git.or.cz/). Now it's time to set it up. First, you want to set up your name and email, which will be added to your commits:




    
    
    $ git config --global user.name "Your Name"
    $ git config --global user.email name@email.com
    





Another useful option is alias. We can also use the command line to set it or we can edit  ~/.gitconfig:



    
    
    [alias]
    	st = status
    




This means we can just type git st instead of git status. As you get more familiar with git, you'll want to add your own aliases.





Check the [manual](http://www.kernel.org/pub/software/scm/git/docs/git-config.html) for the complete list of options.





### Change gitk fonts





Gitk looks bad. Really bad. We can improve it by changing the default font. You need to edit ~/.gitk:




    
    
    set mainfont {Monaco 10}
    set textfont {Monaco 10}
    set uifont {Monaco 10}
    





Much better.





### Bash completion





Lookup contrib/completion in the git source directory. Git-completion.bash includes the instruction to set it up. You need to copy that file somewhere and source it in your ~/.profile. Once this is done, you can press tab to complete git commands, options and the name of branches in bash. The script also adds __git_ps1 which you can use in your PS1 to include the name of the current branch in your bash prompt. Because you will use branches with git, it can help you remember that you switched branch just before leaving work the day before.
