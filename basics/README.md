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
So to achieve that automation, i used `ls -lan` and here we go:tada:.

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
- `/boot`: to display all files in the `boot` directory.

---

All in all we're mastering terminal by automating the boring stuff :smile: 
