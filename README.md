# LearnGit
This contains my (Version Control System) git learning.

## Introduction

_Git is a version control system that helps in maintaining code and multiple versions of any software._ <br>
Git provides two prominent features:
- History of Code :: Git saves snapshots of codes to which we can revert any time.
- Collaboration   :: Allows multiple collaborators to work independently then merge.

## Basic Set-up

**_Configuration of Contributor(Editor) :_**
```sh
 git config --global user.name _"User Name"_
 git config --global user.email _"user123@email.com"_
 git config --list
```
**_Working of Git :_**
Git stores all the history (snapshots) and track every changes being made. <br>
All these are stored in a hidden {.git} file. <br>
A folder must be initiated with .git folder to work with git.

```sh
git init    
```

Once a local repo has been created, and multiple files has been added; repo need to be push to a remote server. Before that, all files must be committed and there need a reference onto which this local directory can be pushed. 

**_Status of file :_**
A file go through different stages in git. <br>
untracked/modified (edit) ---> staged (add) ------> unchanged (commit) <br>

- **U : Untracked**
New files that git does not yet track. VSCode shows it by U / A.
- **M : Modified**
When ever there is uncommitted change. VSCode shows it by M.
- **Staged**
Files added to be saved with next commit.
- **Unchanged**
Files not touched/mofified

_To see these status and change them:_

```sh
git status

git add <filename>      
git add .               

git commit -m "Message is absolute neccesity"
```
add    : add specific file or all by `add .` <br>
commit : record of changes                   <br>

**_set Origin_ :**
There need a connection between **remote** github repository and our local **repos**. <br>
To establish that connection, we create a remote and give it a (alias). <br>

Here [origin] is an alias for the remote repository.

```sh
git remote add origin <LINK>
git remote -v 

git branch
git branch -M master
```
`git remote -v` verifies origin fetch and push pathways (link). <br>
`git branch` shows current working branch, `-M` to rename it.

**_Clone a Repo :_**
Instead of creating a repo from scratch on local machine, a remote repository can be cloned directly with all the above settings already intact.

```sh
git clone <ssh_link>
```

**_Push commits :_**
Once files are commited on the local machines, we need to push them onto the remote servers. </br>
To push our commits to the github site, `push` cmd is used.

```sh
git push -u origin master
# next time
git push

```
All the **commits** will be push to origin (alias of the repo) in the master branch. <br>
`-u` flag used in the first command will do the work and set an **upstream** i.e next time `git push` will be enough to push onto 'origin master' (like alias).


**_Basic Commands_**
Basic terminal commands also works in git
- **ls** : list down all
- **clear** : Clear console
- 
