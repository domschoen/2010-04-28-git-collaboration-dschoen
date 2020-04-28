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

