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