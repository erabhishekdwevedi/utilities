# Git Commands

### Start
* Git initiate a repository.

```
git init
```
* Clone existing repository to your local machine.

```
git clone <repo url>
```

### Add & Deploy
* Add files for adding for commit index or stage.
_Typical Workflow is like  : Make Changes in files > Add > Commit > Push_
```
git add .
git add <filename>
```
* Remove files from commit index or stage 
```
git rm .
git rm <filename>
```
* Commit added changes to local repository
```
git commit -m " Commit message"
```
* Add and commit changes together to local repository . This only includes files which were previously added.
```
git commit -a 
```
* Push commited Changes to remote repository
```
git push
```
* Fetch changes from remote repo and merge with your local repo to match the current state

```
git pull 
```
* Fetch changes from remote repo and merge with your local repo to match the current state

```
git pull origin
```


### Branch
* List All branches
```
git branch
```
* Create New Branch
```
git branch <branchname>
```
* Create Remote Branch
```
git push --set-upstream origin <branchname> // origin is remote repo 
```
* Checkout or Switch to New Branch
```
git checkout <branchname>
```
* Create a branch and checkout to new branch
```
git checkout -b <branchname>
```
* Copying changes from master to branch
```
git checkout <branchname>
git merge master
```
* Copying changes from branch to master
```
git checkout master
git merge <branchname>
```

* Delete remote branch
```
git push origin --delete <branchname>
```
* Delete local branch
```
git checkout -b <branchname>
```

### Others
* Get status of repository.
```
git status
```
* Compare differences done since last commit
```
git diff
Press Q to exit 
```
* Garbage Collection For your repository
```
git gc
```
* Force Exit from git command without changes
```
Press Esc + :q! 
```
* Force Exit from git command with changes
```
Press Esc + ZZ 
```
* Show logs of git 
```
git log
git log --oneline
git log --author ="Abhishek"
git log -5 // count of logs to show
git log --after="2018-1-1"
git log --before="2018-1-1"
git log --filename1.txt --filename2.md
```
