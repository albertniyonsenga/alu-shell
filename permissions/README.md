# Shell permissions

## My name is Betty - 0
In this task we crafted a script that switches the current user to the user `betty`, where we assumed that user already exist by the time we will run the script.
> We used `su` and then the user and in our case is `betty`.

## Who am i - 1
In this task we did a script that prints the effective username of the current user by using command `whoami`.

## Groups - 2
We used `groups` command to print out all the group associated with current user.

## New owner - 3
We aim to change the owner of the file `hello` to the user `betty`.

## New - 4
We created the new file using `touch` command and then file_name.

## Execute - 5
We are required to add scripts that will execute permissions to the owner of the file in our working directory, permission is `-rwxr--r--` where we used `chmod numbers` of `744` to get intended the result. Here is the quick view of the solution:
- `7`: which stands for `rwx` stands for read, write and execute.
- `4`: which stands for `r--` stands for read.
So here the file owner will be able to add, and execute file as well as reading the file content.

## Multiple permissions - 6
For the scripts that adds execute permissions to the owner and the group owner and then read permissions to other users on our `hello` file we used 
> `754`as by adding `5` to add the read and execution permission.
## Everybody - 7
To add the execution permission to all users we used `chmod +x file_name`and boom we are ready to go :smile:.
## James Bond - 8
We then changed the permission of the `hello` file so that both owner and group will have no permissions at all and then other user have all permissions by using `chmod 007 hello` .

## John Doe - 9
To set the mode of our file to `-rwxr-x-wx`, we used `chmod 753 file_name` to set to that permissions while it's located in our working directory.

## Look in the mirror - 10
We have to craft a script that set the mode of file `hello` the same as `olleh` mode and we used `--reference` command to  accomplish that with ease so that it can work for any mode.

## Directories - 11
We crafted script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed.
Where we used `find` to get all the current directories and then execute `chmod 755` to set the permissions and then here we are :smile:.

## More directories - 12
In this task we was required to craft script that create directory `my_dir` withe permission of `751` in current directory. And here we used simple command `mkdir` and then parse `-m` so that we can be able to specify the permission and then the name of new directory.

## Change group - 13
As we are required to change the group owner of `hello` file to `school`, we used simple `chgrp` command and then assign new group and finally the file_name.

## Owner and group - 14
We are required to change the owner and group of all files and our directories in the working directory; here we used `chown` command and then use `vincent:staff` to specify that we will change the ownership in recusive way and then `./*` so that all files and directories will be included  form our working directory

## Symbolic links - 15
Here we crafted script that change the owner and the group owner of `_hello` to `vincent` and `staff`, and this file is symbolic link. So we used `chown -h vincent:staff _hello` as simple as we did in **Task 14** and using `-h` we specified that we are working with symbolic link.

## If only - 16
Finally here we have to craft script that changes the owner of a file but only when it's owned by user called `guillaume` and by using `--form=current_user` between the `chown` and `vincent hello` we can simply achieve that; as from will be testing only current owner files and after we go for changing.

---
Wanna test on yourself :smile: feel free to use use those scripts.
