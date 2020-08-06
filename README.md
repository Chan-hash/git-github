# git-github
This is for tutorial purpose.

You can work with project localy. When you want to push it to remote server, then it is necessary to add remote repo url.

git remote add origin <MY-URL>

Now you can push it:

git push -u origin master

When it works. Hooray. Sometimes you may find following error:

error: src refspec master does not match any.
error: failed to push some refs to '<MY-URL>'

The reason why this happens is not that obvious. :-)

Git creates master branch only after commit to your local repo. If you just initialize repo then there is no master. How to fix it?

Just add and commit at least one change to your repo and re-run push command. You can add e.g. .gitignore.

1. add dummy files, then add, then commit. then push using 
git remote add origin <MY-URL> git push -u origin master
2. add your real files, then add, then commit then only ------ git push -u origin master

