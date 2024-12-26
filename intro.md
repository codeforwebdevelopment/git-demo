Git commands demo

test branchgit add -i


Q.
You've checked out some code from a Git repository. You started coding on your own local branch called my-new-changes. You finish coding and run git add to stage all your changes.
$ git branch
* my-new-changes
master
$ git status
On branch my-new-changes
Your branch is up to date with 'origin/my-new-changes'.
Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: src/HelloWorld.py
$ git add -u
What should you do next to deliver your work?
Select the best option:
A. Upload changes to the remote git server using git commit
B.
Submit the staged changes to your local branch using git commit
C. Upload changes to the remote git server using git push
D.
Submit the staged changes to your local branch using git push
