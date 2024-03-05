---
title: Git Commands CLI Cheat Sheet
date: 2024-03-03 10:00:00 -600
categories: [git,CLI,tools]
tags: [git,packages,CLI,tools,utilities]
---

# Basic Git Commands Cheat Sheet

## 1. git help

> Take help from github help section for different commands and other errors.  

## 2. git config

> To set the basic configurations on github like your name and email. 

## 3. git config –-global user.name “username”

> Sets configuration values for your user name on git. 

## 4. git config –-global user.email 'email'

> Sets configuration values for your user email on git.  

## 5. git config –-global color.ui true

> To see different colours on command line for different outputs.  

## 6. mkdir store

> Create a directory if not created initially. 

## 7. cd store

> To go inside the directory and work upon its contents.  

## 8. git init

> To create a local git repository for us in our store folder.This will help to manage the git commands for that particular repository.  

## 9. git status

> To see whats changed since last commit.It shows all the files that have been added and modified and ready to be committed and files which are untracked.  

## 10. git add Readme.txt

> To add a file Readme.txt to the staging area to track its changes.  

## 11. git commit -m “Created a Readme.txt”

> To commit our changes(taking a snapshot) and providing a message to remember for future reference. 

## 12. git log

> To check the history of commits for our reference. 

> **Different ways to use add command:**  

## 13. git add

> To add a specific list of files to staging area.  

## 14. git add --all || git add -A

> To add all files of current directory to staging area. 

## 15. git add *.txt

> To add all text files of the current directory to staging area.  

## 16. git add docs/*.txt

> To add all text files of a particular directory(docs) to staging area. 

## 17. git add docs/

> To add all files in a particular directory(docs) to staging area.  

## 18. git add “*.txt”

> To add text files of entire project to staging area. 

# **More Commands:**  

## 19. git diff

> To figure out what changes you made since last commit.  

## 20. git reset head license

> To undo staging of the file that was added in the staging area.  

## 21. git checkout –license

> To Blow away all changes since the last commit of the file.  

## 22. git commit -a -m “Readme.md”

> To add any of our tracked files to staging area and commit them by providing a message to remember.  

## 23. git reset –soft HEAD^

> To undo last commit and bring file to staging area.  

## 24. git reset –hard HEAD^

> To undo last commit and remove file from the staging area as well(In case we went horribly wrong). 

## 25. git reset –hard HEAD^^

> To undo last 2 commits and all changes.  

## 26. git remote add origin 'url-origin'

> This commands make a bookmark which signifies that this particular remote refers to this URL. This remote will be used to pull any content from the directory and push our local content to the global server.  

## 27. git remote add 'address' 

> To add new remotes to our local repository for a particular git address.  

## 28. git remove rm

> To remove a remote from our local repository.  

## 29. git push -u origin master

> To push all the contents of our local repository that belong to master branch to the server(Global repository). 

## 30. git clone 'url'

> To clone or make a local copy of the global repository in your system   
	(git clone command downloads the repository and creates a remote named as origin which can be checked by command – git remote -v).  

## 31. git branch 'name-of-branch'

> To create a new branch named as 'name-of-branch'.  

## 32. git branch

> To see all the branches present and current branch that we are working on.  

## 33. git checkout Testing

> To switch to branch Testing from master branch. 

## 34. ls

> To see directories and files in the current directory.  

## 35. ls -la

> To see hidden directories and files with in the current directory. 

## 36. git merge Testing

> To merge Testing branch with master branch (or branch that you have checked out).  

## 37. git branch -d Testing

> To delete Testing branch.  

## 38. git checkout -b admin

> To create a new branch admin and set it as current branch.  

## 39. git branch -r

> To look at all the remote branches.  

## 40. git branch -D Testing

> To forcefully delete a branch without making commits.  

## 41. git tag

> To see the list of available tags. 

## 42. git checkout v0.0.1

> To set the current tag to v0.0.1.   
 
## 43. git tag -a v0.0.3 -m “version 0.0.3”

> To create a new tag. 

## 44. git push –tags

> To push the tags to remote repository. 

## 45. git fetch

> To fetch down any changes from global repository to current repository .

## 46. git stash 

> To move staged files to stash area which are present in staging area.

## 47. git stash pop

> To get back the files which are present in stash area.

## 48. git stash clear

> To clear the stash folder.

## 49. git rebase

> Three tasks are performed by git rebase 

>>1.  Move all changes to master which are not in origin/master to a temporary area.
>>2.  Run all origin master commits.
>>3.  Run all commits in the temporary area on top of our master one at a time, so it avoids merge commits.

## 50. Return to previous HEAD
> git switch - || git checkout 'branch-name'

## 51. Create a new branch which retains commits, following change of head
> git switch -c "new-branch-name"

## 52. Pull down ALL contents of remote repository

> git pull --all


## 53. Adding a remote repository to local code repo, and adjusting naming of primary branch
> `git remote add origin <remote-url>`
> `git remote -v` to check status of remote repositories and verify connection exists
> `git push -u origin <name-of-branch, typically will generate as master>`
### To then re-name branch from master to main, or any other combination should it arise:
> 1. Rename the branch locally by running `git branch -m <current-branch-name> <new-branch-name>`
> 2. Push re-named branch to remote with `git push -u origin <new-branch-name>`
> 3. Confirm default branch has been changed/updated through GitHub GUI or Web interface:
>>> Select repository on GitHub
>>> Settings --> Branches
>>> Next to default branch select pencil icon to edit
>>> select the newly named branch as default and save changes
> 4. Delete the old branch from remote by running `git push origin --delete <old-branch-name>`
> 5. Update local clones, run the following:
>>> `git fetch origin`
>>> `git branch -u origin/main main`
>>> `git remote set-head origin -a`