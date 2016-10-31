# git-notes
Git notes and commands.

## Installing git 
Go [here](https://git-scm.com/downloads).

## Setting email
    git config --global user.email "<youremail@example.com>"

## Setting name
    git config --global user.name "<Your Name>"

## To create a new Git instance for a project:
    git init

## View the difference between the file now and how it was at your last commit
    git diff

## Add your GitHub username to your configuration:
    git config --global user.username <username>

## Set remote locally
    git remote add origin <URLFROMGITHUB>

If you have GitHub for Windows on your computer, a remote named 'origin' is automatically created. In that case, you'll just need to tell it what URL to associate with origin. Use this command instead of the 'add' one above:

    git remote set-url origin <URLFROMGITHUB>

## Show all the remotes
    git remote show
    
## Pushing work 
Git has a branching system so that you can work on different parts of a project at different times. By default the first branch is named 'master'. When you push (and later pull) from a project, you tell Git the branch name you want and the name of the remote that it lives on.

In this case, we'll send our branch named 'master' to our remote on GitHub named 'origin'.

    git push origin master
    
    
## Add remote connections
    git remote add <REMOTENAME> <URL>

## Set a URL to a remote
    git remote set-url <REMOTENAME> <URL>

## Pull in changes
    git pull <REMOTENAME> <BRANCHNAME>

## View remote connections
    git remote -v

## Push changes
    git push <REMOTENAME> <BRANCH>
    
## Cloning repos
    git clone <URLFROMGITHUB>
    
## Set local remote for forked library 
    git remote add upstream <ORIGINALLIBRARYURL>
    
## To see current branch and staged files
    git status
    
## Creating branch

Branches are case-sensitive so name your branch exactly the way your GitHub name appears.

    git branch <BRANCHNAME>

To go into that branch and work on it, similar to using cd to change directory in terminal, you checkout a branch. Go onto your new branch:

    git checkout <BRANCHNAME>
    
##  To change your branch name

    git branch -M <NEWBRANCHNAME>
    
## You can create and switch to a branch in one line
    git checkout -b <BRANCHNAME>
    
## Create a new branch
    git branch <BRANCHNAME>

## Move onto a branch
    git checkout <BRANCHNAME>

## List the branches
    git branch

## Rename a branch you're currently on
    git branch -m <NEWBRANCHNAME>

## Verify what branch you're working on
    git status   

## Pull in changes from a remote branch
    git pull <REMOTENAME> <REMOTEBRANCH>

## See changes to the remote before you pull in
    git fetch --dry-run

## Merge a branch into current branch
    git merge <BRANCHNAME>

## Change the branch you're working on
    git checkout <BRANCHNAME>

## Delete a local branch
    git branch -d <BRANCHNAME>

## Delete a remote branch
    git push <REMOTENAME> --delete <BRANCHNAME>

## Pull from a remote branch
    git pull <REMOTENAME> <BRANCHNAME>




























