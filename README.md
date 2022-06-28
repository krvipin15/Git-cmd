# Git-cmd

**Cheatsheet for Git**

## Configuring you Git
git config --global user.name "Username"	Sets the name you want attached to your commit transactions
git config --global user.email "Email"	        Sets the email you want attached to your commit transactions
git config --global color.ui auto	        Colorization of command line output
git config --global credential.helper cache     Sets the git for auto login without credentias for 15 mins 

## Creating Repository
git init	    Turn an existing directory into a git repository
git status          Return current state of repository / working directory
git clone [url]	    Clone a repository that already exists on GitHub

## Operations on Files
git add <file>	            Adds a file to Staging area
git add *	            Adds all files to Staging area
git apply                   Apply patch to the file
git add -p <file>           To look at changes and add them
git commit -a <file>	    Stages files automatically
git commit -m "message"     Add short description about the commit
git log                     show commit logs / history
git log -p	            Produces patch text
git show	            Shows various objects
git diff  	            Show the differences in various commits
git diff --staged	    Show all staged files compared to the named commit
git add -p	            Allows a user to interactively review patches to add to the current commit
git mv	                    Moves a file
git rm	                    Removes a file

## Reverting Changes
git reset	        Resets the repo, throwing away some changes (After Staging)
git commit --amend	Make changes to commits
git revert	        New commit which effectively rolls back a previous commit
git rebase              Reapply commits onn top of another base tip
git rebase -i           Make list of commit which are about to be rebassed

## Branches
git branch	                Used to manage branches
git branch <name>       	Creates the branch
git branch -d <name>            Deletes the local branch
git branch -D <name>	        Forcibly deletes the branch
git checkout <branch>	        Switches to a branch
git checkout -b <branch>	Creates a new branch and switches to it
git merge <branch>	        Merge joins branches together
git merge --abort	        Abort the merge action (In case of merge conflict)
git log --graph --oneline	Shows a summarized view of the commit history for a repo

## Interaction with Remote Repository
git push	     Push commits from your local repo to a remote repo
git push -u          create trackinbg reference for every local branch pushed onto remote repo
git push -f          Force git to push 
git push --delete    To Remove the remote branch
git pull	     Fetch the newest updates from a remote repository

## Remotes
git remote	           Lists remote repos
git remote -v	           List remote repos verbosely
git remote show <name>	   Describes a single remote repo
git remote update	   Fetches the most up-to-date objects
git fetch	           Downloads specific objects
git branch -r	           Lists remote branches; can be combined with other branch arguments to manage remote branches
