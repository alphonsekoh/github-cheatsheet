# github-cheatsheet

## 1. Set-up [Do it only once]
### Configure user info and across local repo

#### set a name that is identifiable for credit when review version history
```
git config --global user.name "[firstname lastname]"
```

#### set an email address that will be associated with each history marker
```
git config --global user.email "[valid-email]"
```

#### set automatic command line coloring for Git for easy reviewing
```
git config --global color.ui auto
```


## 2. Set-up and Init
### Initialising and Cloning repo 

#### initialize an existing directory as a Git repository
```
git init
```

#### retrieve an entire repository from a hosted location via URL
```
git clone [url]
```

## 3. Staging and Snapshot
### Working with Snapshot and git staging area

#### show modified files in working directory for next commit
```
git status
```

#### add a file as it looks now to your next commit (stage). You can also use `git add .` to stage and commit all files in the directory
```
git add [file]
```

#### remove a file from the staging process while retaining the change in working directory
```
git reset [file]
```

#### diff of what is changed but not staged
```
git diff
```

#### diff of what is staged but not yet committed
```
git diff --staged
```

#### commit staged content as new commit snapshot
```
git commit -m "[commit message]"
```

## 4. Branch and Merge 
### Isolating work in branches, changing context, and integrating changes

#### list all your branches. a * will appear next to the currently active branch
```
git branch
```

####  create a new branch at current commit
```
git branch [branch-name]
```

#### switch to another branch and check into own working directory
```
git checkout
```

#### merge the specified branch history into the current one
```
git merge [branch]
```

#### show all commits in the current branch history
```
git log
```

## 5. Inspection and Comparison 
### Examining logs, diff and object info

#### show commit history for current active branch
```
git log
```

#### show commit on branch A that are not on branch B
```
git log branchB..branchA
```

#### show the commits on that file, even renames
```
git log --follow [file]
```

#### show the diff of what is in branch A that is not in branch B
```
git diff branchB...branchA
```

#### show any objects in Git in human-readable format
```
git show [SHA]
```

## 6. Share and update 
### Retrieving updates from another repo and update local repo

#### add a git url as an alias
```
git remote add [alias] [url]
```

#### fetch down all the branches from the git remote
```
git fetch [alias]
```

#### merge a remote branch into current branch to bring it up to date
```
git merge [alias]/[branch]
```



