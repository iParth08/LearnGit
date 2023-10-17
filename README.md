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
- **U : Untracked**
- **M : Modified**
- **S : Staged**
- **UM : Unmodified**
**_Basic Commands_**
Basic terminal commands also works in git
- **ls** : list down all
- 
