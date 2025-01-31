# Shell scripting
In this repository we will explore together  shell scripting, from crafting simple automation scripts.

Here is some quick tasks will explore in this repository:
## Displaying our working directory-0
Automate the work of printing our working directory using `Shell` scripts.
## Displaying our current directory-1
We are required write script to display the contents in our current directory.
## No place like home-2
We crafted script to change the working directory to the user's home directory with ease, here we just used simple command `cd  ..` but incorporated in `shell` script to automate the task
## The long format-3
We are required to display the contents in a long format. I used `ls -l` command to perform that automation.
## Hidden files-4
Displaying the current directory contents including hidden files, i used `ls -la`.
## Loving numbers-5
We have to display contents in long format, hidden files and also with their user and group IDs numerically.
Here i used `ls -lan`, lemme explain more about this command:
- `ls`: we normally use it to display content within current directory.
- `-l`: used to display content in long format(showing permissions, owners, etc.)
- `-a`: used to show all files including hidden ones
- `-n`: used to display numerical user and group IDs instead of names.
So to achieve that automation, i used `ls -lan` and here we go :tada:.

## Welcome-6
We created script a script to change directory to `/tmp` and create new file named `my_first_directory` in that directory. 
## Betty-7&8
In Question 7 and 8 we created new file `betty` and move it from one directory to another and then delete it in its current directory. 
## Bye bye, Back-9&10
In this tasks we crafted script to delete `my_first_directory` and then after we go back to our previous directory.
## Lists-11
In this task we craft script to list all files(including the hidden files) in the `current directory`, `parent directory` and the `/boot` directory in long format as well.
Here is quick descri about the commands:
- `ls -la`: used to list all files in long format and display hidden files, `-l` to list in the long format, and then as well `-a` to include the hidden files and then combine them in one we are ready to go.
- `.`: to display the files in the current directory.
- `..`: to display the files in the parent directory.
- `/boot`: to display all files in the `boot` directory

## Am the file-12
We crafted script to print the type of the file `iamafile` in directory `tmp`; and here we used command `file` and then the path where the file is located which is `/tmp/iamafile`. As addition, talking about the type you can think about the command `type` instead of `file` but `type` is used for commands not the files.

## The symbols-13
In this task we are required to create a symbolic link to `/bin/ls` and name it `__ls__` and make sure the symbolic link is in our current working directory. Ah seems to be challenging let's go through all its parts:
- `ln` : command used to create links between files and it has two types (`Hard links` which  create duplicate reference to given file and `soft links` create shortcut pointing to a file or dir), and for `soft link` we have to use flag `-s`
- `/bin/ls` : our targeted file path
- `__ls__` : the name of symbolic link that we have created in our current directory.

## Copy HTML-14
We are required to copy all `HTML` files from current directory to the parent directory and also make sure they didn't exist in the parent directory. we used `-u` to check if they are newer than destination file or not present at the destinational directory. But for cool stuff is better to make sure that it restrict search to only current directory with `-maxdepth 1` by leveraging `find` command.
## Move-15
We have to create script to move all files with uppercase letter at the beginning to the directory `/tmp/u` and in this scenario we assumed that thid directory exists.
So here we used simple stuffs `[A-Z]*` to specify all uppercased files at beginning and then move them into desired directory.
## Clean and climb-16&17
Starting with Task 16, we have to clean all the files ended by `~` in our current directory. And for Task 17 we are required to directories at the same time `welcome/`, `welcome/to/` and `welcome/to/school` all in our current director.

---

All in all we're mastering terminal by automating the boring stuff :smile: 
