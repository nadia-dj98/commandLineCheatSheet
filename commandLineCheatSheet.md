# Command Line Cheat Sheet

## Introduction

**Terminal**, **Git**, and **GitHub** are important tools software engineers use on a daily basis. Most (regular) users interact with computers using the GUI (graphic user interface) which is already built in to their operating sytem. Essentially, this means they can look through their files, open and create folders, etc. by simply clicking with their cursor. However, programmers use the command line (a.k.a the console, shell, or CLI), whereby commands are typed into a text terminal to tell the computer what to do directly. Although it takes time to learn, once you get the hang of it, this method saves so much time and is worth learning.

## Important Commands

### Command Line Basics

The ls command lists everything in your current directory, by including -a this list also includes hidden files. 

By including -l the list also includes details about each file such as permissions and date of creation.

```
ls 
ls -a
ls -l
```

Lost? Haven't got a clue where you are in your directory? This command prints your current directory and lets you know.
```
pwd
```

cd allows you to change directory. Essentially, if you wanted to go from one folder to another you would use this command to take you there.


If you use this command without any destination (i.e. cd alone) you will be taken to the home directory, no matter where you are.
```
cd
```


### Directory structure and commands

![directory structure](/Screenshot%202022-11-08%20at%2009.55.00.png)
- A directory's structure is like a tree with branches you have the root which is the home directory (~), and the further down you go the further away you get from it.
- In this example, Documents and Desktop would be parent directories, and the files below them would be sub-directories.
- Two dots (..) symbolise the parent directory, and one dot (.) symbolises the current directory.
    - So, if we were in the zoom folder and wanted to change directory to its parent (Documents) we would type the following command:
```
cd ..
```
&nbsp;

This command allows us to create a directory, by adding the name of the directory after the command.


Be careful not to use any whitespaces, unless you want to create multiple folders.
```
mkdir my_directory
```


To create a file in a folder use the touch command followed my the file name.
```
touch my_file.txt
```

To open a file we use the open command followed by the file name.

This would then open your file in a new window.
```
open my_file.txt
```

To move a file we use the mv command followed by the destination we want to move it to (example 1)

This command can also be used to rename a file by typing the file you want to rename followed by the new name (example 2).
```
mv my_file.txt ..
mv my_file.txt my_renamed_file.txt

```


&nbsp;

### Initialising your Repo
```
git init

```
- This command initialises an existing directory as a Git repository. In other words, it creates your repository.

&nbsp;
---

### Staging and Commiting Changes

```