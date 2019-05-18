# Git Daily-Learn
## Git Configuration
```bash
$ git config --global user.name <your-name>
$ git config --global user.email <your-email>
```
## Generate SSH Key
```bash
$ ssh-keygen -t rsa -C <your_email@example.com>
$ cat ~/.ssh/id_rsa.pub     // copy id_rsa.pub
```
## Basic Git Command
```bash
$ git init                  // initialize git
$ git status                // check git status
$ git add <file-name>       // add a single file
$ git add . <add all file>  // add all file
$ git commit -am "comment"  // git commit all file
$ git commit -m "comment"   // commit all file
```

## Git Log
```bash
$ git log                   // check all the-history 
$ git show <log-id>         // show log
```

## Git Checkout
```bash
$ git checkout <log-id>     // go to <log-id> file
$ git checkout master       // go to last/master commit
```





