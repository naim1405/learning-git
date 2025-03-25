# Learning Git


### Basic commands
- initialize git in a folder
```
git init
```
- stage all the files in the current directory
```
git add .
```

- stage the specified file
```
git add filename
```

- commits the staged files with message
```
git commit -m "message"
```

- renames the current branch to Main. Required for github.
```
git branch -m Main
```

- add remote repository
```
git remote add origin [github link]
```

- push the changed commit in th main branch to remote. Tracks the remote branch
```
git push -u origin main
```
- After tracking remote branch only this command is required to push changes to remote
```
git push
```


## Branch
There can be other branch than main branch. These branches allow developer to test new features or fix bugs without affecting the original code. Once feature is developed or bug is fixed it can be merged with the main branch.
 
- Swtich to branch witn [branch-name], if doesn't exist create a new branch.
```
git branch [branch-name]
```

- Pushes the newly created branch to github. Wihout it this branch will not show up in github.
```
git push origin [branch-name]
```

- When pushing to remote repository useing ```git push``` only the main branch is pushed to the remote repo. To push all commits of all the branches to the remote repository the following command can be used.
```
git push --all origin
```

### Merging
- This command merges the commit made in [branch-name] with the current working branch without modifying the [branch-name].
```
git merge [branch-name] -m [message]
```
- The following command while working on branch2 will merge the commits from branch 1 with merge2. It will not change the branch1. Only the branch2 will be changed.  
```
git merge branch1 -m "merging branch1 with branch2"
```

  
- To merge the current branch to the main without changing the current branch:
```
git checkout main
git merge [branch-name] -m "merging branch"
```
