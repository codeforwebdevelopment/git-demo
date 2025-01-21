index-
GitHub
Git
Git Advantages
git vs github
Basics terms to understand to work on GitHub
Some tips to search smartly
git setup
common commands git

https://essence-ai.com/chatbot/   // learn about git repo

Here I will talk about basic git commands that give you more control on your project code management and the difference between git and GitHub.

GitHub:

Create repos, start a branch, write comments, and open pull requests.

Projects on GitHub can be accessed and managed using the standard Git CLI and all of the standard Git commands work with it. It also allows all users to browse public repositories on the site whether they are signed up or not. It is a web-based Git or version control repository and Internet hosting service.

Git:

Git keeps a track of every change ever made. It is a version control system (VCS) for tracking differences in computer files and organising work on those files among multiple people. It is fundamentally used for software development, but it can be used to keep track of changes in any files. Thank famed software developer Linus Torvalds for Git, the software that runs at the heart of GitHub, the same person who created Linux.

Git Advantages-

Git lets you save your code online.

Git will allow all the developers of a project to see what modifications the other one has made.

It allows you to discuss issues in your code with other developers.

Git is Focused on version control, code sharing and GitHub is Focused on centralized source code hosting.

git vs github-

In Git we use the command-line tool while GitHub is used through the web.

We use git to make changes in code and on GitHub we can check those changes.

Git is a revision control system, a tool to manage your source code history and GitHub is a hosting service for Git repositories.

Git is the tool, GitHub is the service for projects that use Git.

Basics terms to understand to work on GitHub-

A Main Working Directory:

It has all the work that we do such as creating, editing, deleting and organizing files on your local computer. We can say that Git overflow.

working directory>staging area>repository  

> git config --global --add safe.directory *  // add it

A Staging Area:

It is an area where you'll put changes you make to the working directory.

Repository:

A repository is a folder inside which you are going to store all your code files. Git permanently saves those changes as different versions of the project.

Fork:

Copying others repository into your account is called forking. It is like making a bookmark.

Upstream:

The person or organisation which owns the code that you forked.

2 commits in GitHub means you made 2 changes.

To work on this you have to download the git bash and GitHub software from https://desktop.github.com/

If you are getting the below error:

error: failed to push some refs to 'https://github.com/username/repo.git'

hint: Updates were rejected because the tip of your current branch is behind

hint: its remote counterpart. Integrate the remote changes (e.g.

hint: 'git pull ...') before pushing again.

hint: See the 'Note about fast-forwards' in 'git push --help' for details.

Then run the below command

PS E:\pro\gameApp> git push -f origin master

if you get this error Unlink of file 'debug.log' failed. Should I try again? (y/n)

Then close your IDE then pull the code

Some tips to search smartly-

file finder

open any repo

Press t

you can search any file in your repository easily.

If you want to search for interesting projects on GitHub just add the topic name and search it

https://github.com/topics/{topicName}

https://github.com/topics/angular

If you want to search the two words then use the question mark

https://github.com/topics/{keyword1}?q={keyword2}

https://github.com/topics/python?q=packages

Link to code snippets

open any file 

Click on any number

right-click and select copy permalink or press y 

It generates the canonical URL means if the content is removed it will always show the code.

Then it will bookmark that line.

Github project holds this information- 

raw

blame

history

watch-(follow this)--notification

star-bookmark

wiki-any material you have

To integrate git in your project follow these steps-

create a new repository on the command line

git init

git add README.md

git commit -m "first commit"

git remote add origin https://github.com/githubusername/demo.git

git push -u origin master

common commands git-

help: To read about a specific subcommand or concept use help. Suppose you need help with the commit command then type this command and it opens a description of this command in the HTML file. 

>'git help -a' and 'git help -g'  'git help <command or concept> // It shows the list of available commands and concept guides.

>git help commit

To exit git log or terminal, type “q” or “z”.

version 

git --version or git version // To check the details of the version type this command

mv

git mv seond.txt second.txt // To rename the file 

git mv first.txt tuna/pp.txt // To move the file to tuna folder use

config 

To set the author name and email address each to be used with your commits use this cmd

git config –global user.name “[name]”

git config --global user.name "Your Name"

git config –global user.email “[email address]”

git config --global user.email "you@example.com"

git config user.email //find user email address

git config --list //get settings detail

git config --global user.name "Your Name" git config --global user.email you@example.com git commit --amend --reset-author

git config user.name "Full Name"

init

To start a git repository so that you can track changes and properly work on the project using this cmd.

>git init [repository name] 

clone 

To Clone/copy everything from some repository to your local machine.

git clone [url]

git clone <add the repository address here>

git clone --branch branchname --single-branch .giturl // to checkout particular branch

git add

add

This command adds the file to the staging area. This adds the file you want to change on the server.  adds all modified and new (untracked) files in the current directory and all subdirectories to the staging area

git add [file]

git add filename.extension

git add .

commit 

This command commits your changes to the repository with an explanation message. Record changes to the repository.

git commit -m “Type message what functionality you have added”

git commit -a -m "Type commit message" // This command submit many files directly without using git add the command

>git commit -am "this submit many files" // Editing and modifying files in git-

diff

This command shows the differences between the files in the staging area and the latest version present. This command gives the file differences which are not yet staged. Show changes between commits, commit and working tree, etc

red colour-your original content

green colour -you change about to make

git diff // for unstaged changes

git diff --staged // for staged changes if the file is present in the staging area(means you use this command git add first.txt) then git diff command will not work for this,

git diff branch1..branch2

shortlog 

Analyze all users commit history to get the full stats of all developers

git shortlog -sn

git shortlog -sn --no-merges.

reset

Remove the file from the staging area. Also, It can undo all the commits after the particularised commit and preserves the changes locally.

git reset [file/commit]

git reset <commit-sha>

git reset HEAD profile.html

git reset

profile.html

git reset –hard [commit] // This command cancels all history and goes back to the specific commit.

status

This command shows all the files that have to be committed. Show the working tree status. It shows the current state and any merge conflicts.

>git status

rm

This command deletes the repository files. Remove files from the working tree and from the index.

git rm [file]

git rm third.txt

log

This command is used to show the version history for the current branch. Basically, it Shows commit logs.

git log

git log --author="sam"

git log --oneline # more succinct output

git log --graph # with a visual graph of branches

git log -S'<search-string>' // Search for a specific text in the commit message

git reflog // View your "undo" history

git log -p //to check last commit changes

show

This command shows the content changes of the specified commit. show various types of objects.

git show [commit]

branch  

This command shows all the local branches in the current repository. List, create or delete branches.

git branch [branch name]

git branch dev

> git branch -d [branch name] // This command creates a new branch.

 git branch -a // fetch all branch names

command to delete feature branch?

fetch

To fetch all branches Download objects and refs from another repository.

git fetch     

checkout

To change from one branch to another. Switch branches or restore working tree files. To back in the condition which it is.

git checkout -b "student-code" // To create new branch use this command-

Remember one thing space is not allowed while creating a new branch.

Example-

git checkout -b "student code" // Incorrect way

git checkout -b "student-code" //  correct way

git checkout [branch name]

git checkout dev

> git checkout -- index.html // back it to that text.

> git checkout - // Go to the last branch name if you don't remember the name of a branch

remote

This command is used to connect your local repository or folder to the remote server.

git remote add "variable name" "Remote Server Link"

git remote add githubrepo https://github.com/Username123/AndroidAppDemo.git 

git remote //gives repository name

git remote show origin // Get current repository origin name

git remote -v // To get origin

git remote set-url origin https://github.com/username/reponame.git // To update the origin 

push

This command sends the committed changes of the branch to your remote repository. It uploads files of the folder to Github. Update remote refs along with associated objects.

git push [variable name] master

git push origin dev

git push origin master

git push -u githubrepo master

git push -f origin master // forcefully push the changes

pull

This command fetches and merges revisions on the remote server to your working directory. Fetch from and integrate with another repository or a local branch.

git pull [Repository Link]

git pull <remote> <branch>

git pull origin dev 

merge  

Join two or more development histories together

git merge

stash

git stash

git stash apply

To examine the history and state check these commands (see also: git help revisions)-

 bisect     Use binary search to find the commit that introduced a bug

 grep       Print lines matching a pattern

grow, mark and tweak your common history-

 rebase     Reapply commits on top of another base tip

 tag        Create, list, delete or verify a tag object signed with GPG

To protect git branch-

go to settings - branches-  Branch protection rules

To check conflict in your code-

do global search

<<<

can we modify the commit message?

search code in GitHub repo

https://github.com/angulardevelopment/{repositoryname}/search?q={search any text code that is in project}

to upload large files-

https://git-lfs.github.com./

To exit git terminal use 

shift +z 

To remove untracked changes-

git clean -f -d   // o make sure that directories are also removed

Don’t actually remove anything, just show what would be done.

git clean -n

To remove untracked changes- git commands git clean -f -d // make sure that directories are also removed 

git clean -n // Don’t actually remove anything, just show what would be done.

https://github.com/stars

development

https://github.com/trending

launch

earning

android app version

GitCoin

earn money by solving issues (repo)

open source work

stop code push in master branch?

branch creation and deletion?

how to rewrite the commit message if you mistakenly commit the msg

cherry picking 

branch merge code 

https://www.instagram.com/p/B1_108PAdqW/?utm_source=ig_embed&utm_campaign=loading

https://skills.github.com/

https://everythingdevops.dev/how-to-create-and-apply-a-git-patch-with-git-diff-and-git-apply-commands/

https://github.com/tiimgreen/github-cheat-sheet

https://dev.to/wesen/squash-commits-considered-harmful-ob1

https://gitexplorer.com/

https://dev.to/unseenwizzard/learn-git-concepts-not-commands-4gjc                                                

https://dev.to/lydiahallie/cs-visualized-useful-git-commands-37p1  

https://www.freecodecamp.org/news/git-diff-command/

medium.com/javascript-in-plain-english/very-useful-git-and-grep-command-for-searching-text-6698f03e8964

https://dev.to/chrisachard/confused-by-git-here-s-a-git-crash-course-to-fix-that-4cmi

medium.com/@tygertec/how-to-find-stuff-in-git-35d4cb8c1845 

how to comparre two projects git 

https://github.com/github-changelog-generator/github-changelog-generator

https://docs.github.com/en/actions/reference/events-that-trigger-workflows#pull_request

TFS-version control    -manage sprint -documentary repository  

medium.com/@rian_17805/git-merge-commit-message-becomes-release-note-3cf827933eae
https://dev.to/geromegrignon/github-actions-full-ci-cd-javascript-workflow-39om

To learn more about git check this site-

try.github.io/    

https://lab.github.com/githubtraining/introduction-to-github

https://education.github.com/discount_requests/student_application

If you take this you will also get a Pro tag-

https://github.com/pricing
https://githubsatellite.com/

https://www.toptal.com/developers/gitignore

https://git-scm.com/
https://git-scm.com/book/en/v2

Git - Downloading Package (git-scm.com)   github setup
https://git-scm.com/download/win

use source tree software

https://learngitbranching.js.org/

https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow

The last commit that has not been pushed yet can be undone by running 'git reset --soft HEAD~' on your terminal. This command undoes the latest commit, keeps the changes in place, and reverts the files back to the staging area.

Use semversion as reference to version naming strategy https://semver.org/spec/v2.0.0.html ​
semantic Versioning
​

Use gitflow as reference to branch naming strategy https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow ​

​

Visualizing Git (git-school.github.io)
https://git-school.github.io/visualizing-git/#rewritten-history

Collaborating workflows	https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow	
git config --list --show-origin
dont add comma, inveted commas to the git new branch

Publicizing or hiding organization membership
Under your organization name, click  People.
To publicize your membership, choose Public.
To hide your membership, choose Private.