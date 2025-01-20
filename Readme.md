# Learning Git
I'll learn git and add what I learned here.

### Basic commands
```
git init
```
above command initialize git in a folder
```
git add .
```
stage all the files in the current directory

```
git add filename
```
stage the specified file

```
git commit -m "message"
```
commits the staged files with message

```
git branch -m Main
```
renames the current branch to Main. Required for github.

```
git remote add origin [github link]
```
add remote repository
```
git push -u origin main
```
push the changed commit in th main branch to remote. Tracks the remite branch
```
git push
```
After tracking remote branch only this command is required to push changes to remote

## Branch
There can be other branch than main branch. These branches allow developer to test new features or fix bugs without affecting the original code. Once feature is developed or bug is fixed it can be merged with the main branch.
 
```
git branch [branch-name]
```
creates a new branch with the name [branch-name]
```
git branch [branch-name]
```
switches to the branch [branch-name].  

### Merging
```
git merge [branch-name] -m [message]
```
This command merges the commit made in [branch-name] with the current working branch without modifying the [branch-name].
If branch1 and branch2 both have some commits, then the following command while working on branch2
```
git merge branch1 -m "merging branch1 with branch2"
```
will merger the commits from branch 1 with merge2. It will not change the branch1 branch. Only the branch2 will be changed.  
  
To merge the current branch to the main without changing the current branch:
```
git checkout main
git merge [branch-name] -m "merging branch"
```

