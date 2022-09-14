# Reading Git Tutorial: A Comprehensive Guide 

[link of article](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/)

## Version Control

**a system that allows you revisit various versions of a file by recording changes**

    - revert a file to previous version

    - track modification and modify individulas

    - compare changes

&nbsp;
### 1. Local Version Control

**entails one database on your hard disk that stores changes to files**

&nbsp;
### 2. Centralized Version Control(CVCS)
**allows collaboration within a developer team**
&nbsp;

    - can be accessed by various clients

    - programmers can have more knowledge of team members' activities with certain files

    - give administrators much more control over divvying up revision privileges.

&nbsp;
### 3. Distributed Version Control(DVCS)
**Addresses major vulnerability of CVS: the server as a single point of failure**
&nbsp;

> Situation 1: collaborators cannot work with each other on a file or save changes and new versions 

> Situation 2: if central database's hard disk is corrupted, the work will be lost
    
    - allows clients to create mirrored repositories

    - multiple mirrored repositories allows programmers working with each other in various way to complete a joint project, which enables the use of various simultaneous workflows

&nbsp;
### 4. So, What is Git?
&nbsp;
>**_Snapshots_** <br>
Git is a DVCS that stores data in a file system made up of snapshots

- each time you save a changed version(commit), Git creates a snapshot of file and stores a reference to it.

&nbsp;
>**_Local Operations_**<br>
Git relies on local operations.

- Eliminating the need to fetch history information from the server.

- Allows working without online or VPN

&nbsp;
>**_Tracking Changes_**<br>
Git will always detect file corruption or loss of information in transit.

&nbsp;
>**_Loss of Data_**<br>
Git minimize the possibility of irreversible damage to files.

&nbsp;
>**_States_**<br>
files in Git can reside in three main states:
- Committed: stored in local database

- Modified: has been changed but not committed to the database

- Stated: flagged a file's changed version to be committed in the next snapshot

&nbsp;
## History of Git
**allows non-linear development via multiple branches, support large projects, possessed strong mechanisms preventing corruptions**

&nbsp;
## Getting Started

### Download Git
    Git can be installed in three ways:
    1. install as a package

    2. install via another installer

    3. download and compile the source code.
&nbsp;

## Mac OS X
>**_Terminal_**<br>

&nbsp;
>**_Git Website_**<br>

&nbsp;
>**_GitHub_**<br>

&nbsp;
## Windows
>**_Git Website_**<br>

&nbsp;
>**_GitHub_**<br>

&nbsp;
## Linux
>**_Package Manager_**<br>

>**_Git Website_**<br>

&nbsp;
1.Graphical Clients

&nbsp;
2.Initial Customization

&nbsp;
3.Default Text Editor

&nbsp;
4.Check Settings

&nbsp;
5.Getting Help

&nbsp;
## Setting up a Git Respository

&nbsp;
### 1.Importing
>(1)Switching to the target project's directory: $ cd test (cd = change directory) 

>(2)Use the git init command: $ git init

>(3)To start tracking these repository files, perform an initial commit by typing the following:
    >- $ git add *.c
    >- $ git add LICENSE 
    >- $ git commit -m "any message here"

&nbsp;
### 2.Cloning: copy an existing Git repository from a server to local
>- $ git clone https://github.com/test 
>- Or with another name: <br>$ git clone https://github.com/test mydirectory

&nbsp;
## Workflow
### 1.Local Repository Structure
&nbsp; 

&nbsp;
### 2.Saving Changes
>**_Tracked_**<br>Tracked files can be modified, unmodified, staged

>**_Untracked_**<br>Untracked files were not in the last snapshot and do not currently reside in the staging area
&nbsp;

&nbsp;
### 3.The Life Cycle of File Status
&nbsp;
- Git flags an editted file
- You stage the modified file
- you commit staged changes

&nbsp;
### 4.Check file Status
$ git status
&nbsp;

&nbsp;
### 5.Tracking and staging a New File

>**_Single File_** <br>
+ git add filename

>**_All Files_**<br>
+ git add *

&nbsp;
### 6.Committing a File
>- git commit -m "made change x,y,z"

&nbsp;
### 7.Committing all Changes
>- git commit -a

&nbsp;
### 8.Pushing Changes
>- git push origin master

&nbsp;
### 9.Stashing Changes
>- git  stash<br>
(when you are not ready to commit changes but do not want to lose them either)
>- git stash apply<br>
(when you ready to comtinue working on the changes, this can retrieve the hidden changes.)


&nbsp;
## Remote Respositories

### 1.Cloned Repositories

### 2.Seeing Your Remotes

### 3.Adding Remotes

### 4.Fetching

### 5. Pushing

### 6.Renaming/Removing Remotes


&nbsp;
## Undoing Actions

### 1.Commit Mistakes

### 2.Untaging a File

### 3.Undo a Committed Snapshot

### 4.Unmodifying a File




&nbsp;
## Branching

enable collaborators to work simultaneously via multiple branches without affecting this main repository.

### 1.Creating a New Branch
>- $ git branch test

### 2.Switching Branches
>- $ git checkout test

### 3.Create a Branch and Checkout
>- $ git checkout -b test2<br>
create a new branch "test2" and switch to it.

### 4.list Branches
>- $ git branch


&nbsp;
## Merging

### 1.Fast-Forward Merging

### 2.No Fast-forward

### 3.Three-way Merge

### 4.Fetching and Merge

### 5.Deleting Branches

### 6.Merge Conflicts

### 7.Preview Changes

### 8.Listing Branches

### 9.See Latest Commits


&nbsp;
## Rebasing

### 1.The Basics

### 2.Rebase vs.Merge


&nbsp;
## Log


&nbsp;
## Tagging

### 1.Create a Tag
>**_Lightweight_**<br>
- Create Lightweight Tags
>**_Annotated_**
- Create Annotated Tags

### 2.Tag Sharing

### 3.Tag Checkout

&nbsp;
## Aliases


&nbsp;
## Ignoring Files


&nbsp;
## Distributed Workflows

### 1.Centralized Workflow

### 2.Integration-Manager Workflow

&nbsp;
## GitHub

### 1.Getting Started

### 2.Contributing to Projects

### 3.General Workflow
