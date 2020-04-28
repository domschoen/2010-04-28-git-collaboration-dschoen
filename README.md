# 2010-04-28: Git Collaboration Notes
Git collaboration workshop

- `git clone <URL>`: downloads the repository from the web to our computer
    - Make sure you don't nest this command in another repository
    - just like `git init`do this only once per repository

```    
git remote -v
origin	https://github.com/domschoen/2010-04-28-git-collaboration-dschoen.git (fetch)
origin	https://github.com/domschoen/2010-04-28-git-collaboration-dschoen.git (push)
```

## Branches
### Create a new branch
``` 
git branch my_first_branch
``` 
### List all branches
``` 
git branch -a    
``` 
git switch my_first_branch
or  
git checkout my_first_branch

Delete a branch
git branch -d my_first_branch

create and go directly to the branch
git switch -c my_first_branch
git checkout -b my_first_branch

git --version
git version 2.15.0
Trainer: 2.26.2 
```

### List all branches
```
git log --oneline --all --decorate
``` 
```
git log --oneline --graph --all --decorate
```
### Merge
Let's do it on the web interface (to get the review and all other stuff)


### Stashing
writing a temporary commit
```
git stash
```
Then we can switch to master and go back to the branch reapply the stash to retrieve your work.
```
git stash apply
```
```
git stash list
```
```
git stash clear
```


git push --set-upstream origin my_first_branch
git push origin my_first_branch

Deleted branch 
git fetch --prune

git branch -d my_first_branch
git branch -a
git log --oneline --graph --decorate --all

### Exercise
1. create a new branch
```
git checkout master
git checkout -b mybranch
```
2. edit the reame file 
  add/commit
```
git add README.md
```  
3. push the branch to the remote
```
git push origin mybranch
```
4. create the PR
  - master compare mybranch
  - create PR
5. look around
6. merge the PR
7. delete the branch on GH
8. go to master on local computer 
9. pull merged changes
```
git checkout master
git pull origin master
```
10. clean up all your branches
--all if you have multiple remotes.
```
git fetch --prune --all
git branch -a
git branch -d mybranch
git log --oneline --graph --decorate --all
```

if muliple people merging at the same time
git is a acyclic graph
second person problem

What if we merge and we have also modification in the master

Let's try
2 branches




