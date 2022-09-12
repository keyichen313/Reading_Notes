# Linux Tutorial 1. Command line

## Command line

A command line, or terminal, is a text based interface to the system.

1. First command line arguments OR option: -l

    ### is used to modify the behaviour of the command

    ### usually listed before other arguments

    ### start with a dash (-)

2. Out put of running the command.

3. Prompt again: after the command has run and the terminal is ready for a new command


## Opening a terminal

Applications -> Utilities


## The Shell, Bash

    ### Shell: is within a terminal, defines how the terminal will behave, and running commands for you

    ### Bash: Bourne again shell, one of the most common shell

    ### Echo a shell: if you want to know which shell you are using, use the command **_Echo_**

for example: echo $SHELL, then the sceen will show something that ends in bash: for example: /bin/bash


## Shortcuts

using up and down arrow keys to traverse historical commands

using left and right arrow keys to move the cursor



# Linux Tutorial 2. Navigation

## pwd:Print Working Directory
    where you are (where your current directory is )

## ls: List Directory contents
    what is there

    1.You can do more thing with ls:
        (1)ls[options][location]: []means optional

        (2)l: use a long listing format

        (3)t: sort by modification time, newest first
        
    2. breaking down:
        (1)example
        ls l

        total 3
        drwxr-xr-x  2 ryan users 4096 Mar 23 13:34 bin
        drwxr-xr-x 18 ryan users 4096 Feb 17 09:12 Documents
        drwxr-xr-x  2 ryan users 4096 May 05 17:25 public_html
         
        Breakdown explain:

        drwxr-xr-x  2 ryan users 4096 Mar 23 13:34 bin
            d first character: normal file(-) or directory(d)

            next 9 characters: permissions ofr the file

            2 block: the number of blocks

            Ryan block: the owner of the file/directory

            users: the group the file/directory belongs to (user in this example)

            4096: file size

            Mar 23 13:34: Modification time

            bin: actual name of the file/directory

    3. command line argument: /etc
        (1)example
            ls /etc: 
            a2ps.cfg aliases alsa.d cups fonts my.conf systemd
            
            Explain:
            it tells ls NOT to list our current directory but instead to list that directories contents.

        (2)example
            ls -l /etc:
            total 3
            -rwxr-xr-x  2 root root 123 Mar 23 13:34 a2ps.cfg
            -rwxr-xr-x 18 root root 78 Feb 17 09:12 aliases
            drwxr-xr-x  2 ryan users 4096 May 05 17:25 alsa.d

            Explain: the -l /etc are
            both command line option and argument. It will do a long list of the directory /etc

## Path
a path is a means to get to a particular file/directory on the system

### absolute and relative path

1. root directory: it is denoted by a single slash(/), the very top of the structure

2. absolute path specify a location(file/directory) in relation to the ROOT directory, and they ALWAYS begin with forward slash(/)

This command will provide the same output regardless of our current location when we run it.

3. relative path specify a location(file/directory)in relation to where we CURRENTLY are in the system. They will NOT begin with slash

Example:
ls Documents
file1.txt file2.txt file3.txt

Documents is a directory in our current location. This commands could produce different results depending on where we are.

4. ~(tilde): home directory
    Ex: /home/ryan/Documents = ~/Documents

   .(dot): current directory
   Ex: ls Documents = ./Documents

   ..(dotdot): parent directory, use it several times in a path to keep going up the hierachy, until reach the root directory


# Move around a bit

cd: change directory (move to another directory)

cd[location]: if you run the command cd without any arguments then it will always take you back to your home directory

/etc - Stores config files for the system.

/var/log - Stores log files for various system 
programs. (You may not have permission to look at everything in this directory. Don't let that stop you exploring though. A few error messages never hurt anyone.)

/bin - The location of several commonly used programs (some of which we will learn about in the rest of this tutorial.

/usr/bin - Another location for programs on the system.

# Linux Tutorial 3. More About Files

## Everything is a File

## Linux is an Extensionless System

1. Linux ignores the extension and looks inside the files to determine what type of file it is. (Regardless how I change the extension of the file, Linux will make its own decision base on the fact)

2. file[path]: to find out the real type
    
    a path is a means to get to a particular location in the system and that location is a file.

## Lunix is Case Sensitive

## Spaces in Names

Example: Holiday Photos is a name of a file, to access it, the following is wrong:

cd Holiday Photos 
Because command cd only recognized the first command line argument only

Two ways to fix it:
    1. Quote: anything inside a single quotes is considered one item 'Holiday Photos'

    Ex: cd 'Holiday Photos'
        pwd
        /home/ryan/Documents/holiday Photos

    2. Escape Characters with Backslash (\) nullify the special meaning of the next character

    Ex: cd Holiday\ Photos
        pwd
        /home/ryan/Documents/Holiday Photos

        the special meaning of the space which is to separate them as distinct command line argument is removed.

## Hidden files and Directories

1. hidden file's name: . + file/directory's name
    (* starts with a . (full stop))

    we can rename a file to hide it

    ls will not list the hidden file

2. ls -a: will show the hidden file


book in github