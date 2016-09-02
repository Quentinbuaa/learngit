Git is a distribution version control system.
Git is a free software distribution under the GPL.
Git has a mutable index called stage.
Git tracks changes of files.
It's my first time to use github !


This is the third time of learing git.
I want to master the usage of git.

Noun: "untracked" means that this is a new file. To get the git start tracking the changing of this new file, we have to add it to the stage area by git add.

"changes to be commit:" this means that the files are in stage area, and they are not in repository yet. To store the staged changes we run commit with a message describing what we've changed. 

You can use wildcards if you want to add many files of the same type. Don't forget the quote.

Fotunately for us, there's git log. Think of Git's log as a journal that remembers all the changes we've committed so far.

To push our local repository to the git server, we have to add a remote repository. This can be done by git remote add with a name and URL.

The push command tell Git where to push out commits when we're done. The push have a -u option, which tell Git to remember the parameters so next time we run git push without ambiguous. The push have two parameters, the name of the remote repository and the local branch.

Let pretend some time has passed. We've invited some other people to our git repository and make some changes. We can use git pull origin master and use git diff HEAD to checkout the changes.

Another big use of git diff is to "git diff --staged" to see the changes between staged files.

If you want to remove a file, you can use "git rm". This command will not only delete the file on a disk, but will also stage the removal of the file for us. Then the only thing you need to is commit.

After you make some changes on clean_up branch, you can commit and go back to you master and merge that changes.

This time, I have learned that the concept of stage area. Also I know that the new added file will not be tracked if it have not be sent to stage area. And usage of git reset and git diff and git rm 
git reset: unstage the staged file
git diff: firstly, it can be used to check the difference between the master and the head of the current workspace. Secondly, it can be used to compare the file and staged file by using git diff --staged 
git checkout: git checkout -- "some file" can be used to rmove all the changement made on "some file"
git rm: Not only remove the file on disk, but also remove it from stage.

