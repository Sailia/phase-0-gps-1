# phase-0-gps-1

The purpose of this page is to describe my process when creating a file and pushing that file into the Github repo.
The following in bold are my commands towards git.

##cd DBC
I needed to change directories to create a file in that directory
##touch awesome_page.md
Created the file awesome_page.md
##ls
list the files in the directory to make sure I created the file
##rm awesome_page.md
removed the file after checking that I was supposed to create the file on the master branch in git.
##git co master
So I got on to the master branch
##touch awesome_page.md
Created the file
##git status
Made sure the file was created
##git add awesome_page.md
Therefore added the file to git to commit
##git commit -m "upload awesomepage"
committed the file to prepare for lift off.(upload into github)
##git push origin awesome_page.md
Oh noes! This printed:
####error: src refspec awesome_page.md does not match any.
####error: failed to push some refs to 'https://github.com/Sailia/phase-0-gps-1.git'
##git status
So I wanted to check what happened. See this yo.
####On branch master
####Your branch is ahead of 'origin/master' by 1 commit.
####  (use "git push" to publish your local commits)
####nothing to commit, working directory clean
##ls
Checked if the file wasn't injured
##git commit
I thought I might as well just try to commit the entire folder as the files are the same on the repo so I wouldn't be adding unrelated files.
####On branch master
####Your branch is ahead of 'origin/master' by 1 commit.
####  (use "git push" to publish your local commits)
####nothing to commit, working directory clean
##git push
So I thought to push the entire folder
####warning: push.default is unset; its implicit value has changed in
####Git 2.0 from 'matching' to 'simple'. To squelch this message
####and maintain the traditional behavior, use:

####  git config --global push.default matching

####To squelch this message and adopt the new behavior now, use:

####  git config --global push.default simple

####When push.default is set to 'matching', git will push local branches
####to the remote branches that already exist with the same name.

####Since Git 2.0, Git defaults to the more conservative 'simple'
####behavior, which only pushes the current branch to the corresponding
####remote branch that 'git pull' uses to update the current branch.

####See 'git help config' and search for 'push.default' for further information.
####(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
####'current' instead of 'simple' if you sometimes use older versions of Git)

####Username for 'https://github.com': Sailia
####Password for 'https://Sailia@github.com':
####Counting objects: 3, done.
####Delta compression using up to 4 threads.
####Compressing objects: 100% (2/2), done.
####Writing objects: 100% (3/3), 313 bytes | 0 bytes/s, done.
####Total 3 (delta 0), reused 0 (delta 0)
####To https://github.com/Sailia/phase-0-gps-1.git
####   1efef03..0c6d5c2  master -> master

Done!!!