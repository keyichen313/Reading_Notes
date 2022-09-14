# The most useful commands in Linux terminal

1.How to push updates into GitHub?

- make change

  on your computer top bar, chose Fil->Save (unless you set it to Auto Save already)

- type in your local VS Code's Terminal: git status
  
  if it is red color, then you need to save it again by doing git add .; if it is green color, it is already saved successfully.

- type in your local VS Code's Terminal: git add .

  (this command is adding staging area)

- type in your local VS Code's Terminal: git commit -m 'Whatever Your Descriptive Name Here to Help You Recall your memory of What you did In VS Code'

  (-m means make, it is to save a change by doing commitment)

- type in your local VS Code's Terminal: git push origin main

  (push change into GitHub finally)

<br>
2.How to insert a photo?

  ![Description of what you want to show in your website link](./Your Photo Name Here.JPG)
  
  for example: ![image](./image/sunset.jpg)

<br>
3.How to go back to home page?

./
  
<br> 
4.How to know where I am now and open it in local VS Code?
  
  Code .

  >(Note: code . will open the VS Code with the folder that you are currently in in the computer terminal,<br> 
  while the code will open the VS Code with the entire computer, without a specific folder)

<br>
5.How to change name inside the same folder?
type mv (stands for move)

Example: change the name of Improve_Notes to Reading Notes as following:
mv Improve_Notes Reading_Notes

Note: mv can also change the location

<br>
6.How to merge the change I made in GitHub with local VS Code?
  
>You will need to pull the change back to VS Code by typing following command in the VS Code Terminal:<br>
_git pull origin main_

<br>
7.How to delete files in local computer?

- rm stands for remove

- rf stands for recursive force (a lot of time the computer does not want to delete things)

- Type following command to delete a file:

  rm -rf 'The Name Of The File That Needs To Be Deleted Here'

<br>
8.different creation

- create a directory: mkdir
- create a file: touch

<br>
9.touch--> create a new file within your current directory

  mkdir--> create a directory/folder

<br>
10.pwd--> print working directory-->where am i?

<br>
11.cd ..--> go back/up one directory
cd-->change directory

<br>
12.tree--> show all directories and files where I currently in

<br>
13. 
    ls --> list the names only

    ls -l --> Your list file in an actual list form with more information

    ls -a --> list not only the name of the regular files, but also the names of the hidden files too.
    
    ls -la --> your regular and hidden files are all listed in detail information 

<br>
14.Basic Command

- pwd: print working directory
  - you are here
- ls: list directory contents
  - shows you what is inside the folder you are in
- ls -a: list all (even hidden)
  - shows all files, including hidden files
- cd: change directory
  - how you move to a new folder
  - example: cd projects/courses
- cd .. : change directory back one level
  - moves you back one level in your folder structure
- mkdir: make directory
  - creates a new folder/directory
- touch: create new file
  - example: touch newfilename.md, touch newfile.html 

folder/file notes

folder and directory are the same,a collection of a notebook

repository is a folder/directory that Git is paying attention to

File is a single file, like a page in a note book