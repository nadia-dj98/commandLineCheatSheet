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
### Deleting files a.k.a DANGER ZONE
The following commands are for when we want to delete a file. Be careful because there is no turning back once you've deleted something so be sure what you are doing is corrrect.

The rm command deletes a file ***permanently***
```
rm my_renamed_file.txt
```
What we cannot do with an rm is delete a directory, to do this we would have to also add the -r command. This will delete the directory as well as everything inside of it.
```
rm -r my_directory
```

&nbsp;

### Initialising your Repo
Now that we've familiarised ourselves with using the terminal and some basic commands. Let's learn how to create a repository which tracks changes we make to a file. This is useful because if we ever need to go back to an older version we can. 

&nbsp;


This command initialises an existing directory as a Git repository. In other words, it creates your repository.

```
git init

```


&nbsp;
---

### Staging and Commiting Changes

Once we've made some changes to our file that we want to be tracked we use the git add command.

This essentially adds a file as it currently looks ready for our next stage.
```
-git add . 
```

Our next step is to commit the changes we've made. Commit is like the save function, it takes a snapshot or a record of the code at the moment the commit has been made. You're creating a point at which the code is being saved to the repository.

```
git commit -m "insert description/message of the changes you made"
```

Last but not least we want to send a copy of these changes to a remote repository. By doing this it means anyone with internet access (and with permissions) can have a copy of our code and make changes to it too.

We use the push command to do this, we "push" our changes to the cloud or in our case *GitHub*.
```
git push 
```

If we want to check the changes we have committed we can use the log command to do so.

```
git log
```

## Conclusion and Further Reading
The Terminal, Git, and GitHub are useful tools and worth getting to grips with. This cheat sheet is just scratching the surface but is a great place to start. For further reading and fun resources the following resources are great:

1. [Git and GitHub Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)
2. [A game to learn and practice Git commands](https://schoolofcode.github.io/line-commander/)
3. [Oh my Git! : Another Game to learn and practice using Git](https://ohmygit.org/)
4. [BNTA Documentation on Git, GitHub, and the Command Line](https://brightnetwork-technology-academy.github.io/curriculum/git/lessons/intro_to_git/intro_to_git/#sharing-code-with-github)

