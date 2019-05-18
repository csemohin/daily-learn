# Git Daily-Learn
## Git Configuration
```bash
$ git config --global user.name <your-name>
$ git config --global user.email <your-email>
```
## Generate SSH Key
```bash
$ ssh-keygen -t rsa -C <your_email@example.com>
$ cat ~/.ssh/id_rsa.pub             # copy id_rsa.pub
```
## Basic Git Command
```bash
$ git init                          # initialize git
$ git status                        # check git status
$ git add <file-name>               # add a single file
$ git add . <add all file>          # add all file
$ git commit -am "comment"          # git commit all file
$ git commit -m "comment"           # commit all file
$ git commit --amend                # same commit but different log id
```

## Git Log
```bash
$ git log                           # check all the-history 
$ git show <log-id>                 # show log
$ git log <fileName.txt>            # show single file log
$ git reflog                        # show all file log
```

## Git Checkout
```bash
$ git checkout <log-id>             # go to <log-id> file
$ git checkout master               # go to last/master commit
$ git checkout <log-id> <file.txt>  # go to single log
$ git checkout master -f            # go to single file master/head
```
## Git Reset
```bash
$ git reset --soft <log-id>         # reset accidental commit softly
$ git reset --hard <log-id>         # reset accidental commit hardly
$ git reset HEAD@{<reflog-offset>}  # hard reset file backup
$ git reset hard                    # after reset HEAD@{8}
```
## Git Stash & Git Clean
```bash
$ git stash                         # temporary data delete
$ git stash pop/apply               # temporary date back
$ git stash list                    # show how many stash available
$ git stash pop stash@{<stash-list-offset>} # back any offset stash
$ git stash clear                   # clear all stash
$ git clean -f                      # delete all untraced file
$ git clean -f -n                   # check whose file I want to delete
```
## Git Push & Git Pull
```bash
$ git clone <url>                   # download repository from url
$ git remote add <origin> <url>     # add local repository in remotely
$ git remote show                   # show how many git remote
$ git remote show <origin>          # show how many git remote url
$ git pull origin <branch>          # latest file from server <branch>
```
## Git Ignore
> git ignore file automatically remove all file and and folder. Ex- *.zip

## After Git Marge
```bash
$ git checkout master; git fetch; git reset --hard origin/master; git branch -D <branch-name>; git checkout -b <branch-name>
```