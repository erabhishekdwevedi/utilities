#Git Commands

* Git initiate a repository.

```
git init
```
* Clone existing repository to your local machine.

```
git clone <repo url>
```
* Get status of repository.
```
git status
```
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
git pull origin
```
* Compare differences done since last commit
```
git diff
Press Q to exit 
```
* List All branches
```
git branch
```
* Create New Branch
```
git branch <branchname>
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
