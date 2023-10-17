# LearnGit
This contains my (Version Control System) git learning.

## Introduction

_Git is a version control system that helps in maintaining code and multiple versions of any software._ <br>
Git provides two prominent features:
- History of Code :: Git saves snapshots of codes to which we can revert any time.
- Collaboration   :: Allows multiple collaborators to work independently then merge.

## Basic Set-up

**_Configuration of Contributor(Editor)_**
```sh
 git config --global user.name _"User Name"_
 git config --global user.email _"user123@email.com"_
 git config --list
```
**_Working of Git_**
Git stores all the history (snapshots) and track every changes being made. <br>
All these are stored in a hidden {.git} file. <br>
A folder must be initiated with .git folder to work with git

```sh
git init    
```

**_Status of file_**
A file go through different stages in git. <br>

- **U : Untracked**
New files that git does not ye track. VSCode shows it by U / A.
- **M : Modified**
When ever there is uncommitted change. VSCode shows it by M.
- **Staged**
Files added to be saved with next commit.
- **Unmodified**
Files not touched/mofified

_To see these status and change them:_
```sh
git status

git add <filename> //add specific
git add .          //add all

git commit -m "Message is absolute neccesity"
```

**_Basic Commands_**
Basic terminal commands also works in git
- **ls** : list down all
- 
