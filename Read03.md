# Reading Git Tutorial: A Comprehensive Guide

[link of article](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/)

## Version Control

**a system that allows you revisit various versions of a file by recording changes.**

    - revert a file to previous version

    - track modification and modify individulas

    - compare changes

&nbsp;

### 1. Local Version Control

**entails one database on your hard disk that stores changes to files.**

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

> Situation 1: collaborators cannot work with each other on a file or save changes and new versions.
> Situation 2: if central database's hard disk is corrupted, the work will be lost

    - allows clients to create mirrored repositories

    - multiple mirrored repositories allows programmers working with each other in various way to complete a joint project, which enables the use of various simultaneous workflows

&nbsp;

### 4. So, What is Git?

&nbsp;
>**_Snapshots_**
>
>Git is a DVCS that stores data in a file system made up of snapshots
>>each time you save a changed version(commit), Git creates a snapshot of file and stores a reference to it.

&nbsp;
>**_Local Operations_**
>
>>Git relies on local operations.<br>
>> Eliminating the need to fetch history information from the server.<br>
>> Allows working without online or VPN

&nbsp;
>**_Tracking Changes_**<br>
Git will always detect file corruption or loss of information in transit.

&nbsp;
>**_Loss of Data_**<br>
Git minimize the possibility of irreversible damage to files.

&nbsp;
>**_States_**<br>
files in Git can reside in three main states:
>> Committed: stored in local database<br>
>> Modified: has been changed but not committed to the database<br>
>> Stated: flagged a file's changed version to be committed in the next snapshot<br>

&nbsp;

## History of Git

allows non-linear development via multiple branches, support large projects, possessed strong mechanisms preventing corruptions.

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
>- for Fedora: $ sudo yum install git
>- for Ubuntu: $ sudo apt-get install git

&nbsp;
>**_Git Website_**<br>

&nbsp;
>1.Graphical Clients<br>

>2.Initial Customization
 >>**_configuration of Variables_**:<br>
    an inherent git tool called git config allows the setting of configuration variables that control aspects of Git's operation and look <br>

 >>**_identify setting_**<br>
set the user name and email address that will be used for every Git commit<br>
-_git config --global user.name "Jane Smith"_<br>
-_git config --global user.email "example@email.com"_

>3.Default Text Editor<br>
 to configure a different text editor, such as Emacs, type:<br>
    _git config --global core.editor emacs_

>4.Check Settings: _git config --list_

>5.Getting Help: three ways to get more information on a particular command by accessing the manual:<br>
-_git help command_<br>
-_git command --help_<br>
-_man git-command_<br>

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

- Working Directory
- Index
- Head

&nbsp;

### 2.Saving Changes

>**_Tracked_**<br>Tracked files can be modified, unmodified, staged

>**_Untracked_**<br>Untracked files were not in the last snapshot and do not currently reside in the staging area
&nbsp;

&nbsp;

### 3.The Life Cycle of File Status

- Git flags an editted file
- You stage the modified file
- you commit staged changes
&nbsp;

&nbsp;

### 4.Check file Status

_$ git status_

&nbsp;

### 5.Tracking and staging a New File

>**_Single File_** <br>
+ git add filename

>**_All Files_**<br>
+ git add *

After using these commands, files are tracked and staged for committing.

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

> Git will automatically give the name "origin" to the server from which you cloned and the name "master" to your local branch.

### 2.Seeing Your Remotes

>_git remote_: review the short names of all specified remote handles.<br>
>_git remote -v_: view all the remote URLs next to their corresponding short names.

### 3.Adding Remotes

>_git remote add shortname url_

### 4.Fetching

>Fetching entails pulling data that you don't have from a remote project.
>>_git fetch [remote-name]_ <br> 
>>For cloned repositories, use _git fetch origin_ to pull down any new changes that were pushed to the server since you cloned or last fetched from it.

### 5.Pushing
>_git push [remote-name][branch-name]

### 6.Renaming/Removing Remotes
>Rename
>> git remote rename js jane (short name has been changed from js to jane)<br>
>> git remote (list our existing remotes) <br>
>> origin<br>
>> jane<br>

>Remove
>>_git remote rm jane_ (git remote rm is to remove a remote)<BR>
>>_git remote_
>>_origin_

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

### 3.General Workflowrea
