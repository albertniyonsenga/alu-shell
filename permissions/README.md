# Shell permissions

## My name is Betty - 0
In this task we crafted a script that switches the current user to the user `betty`, where we assumed that user already exist by the time we will run the script.
> We used `su` and then the user and in our case is `betty`.

## Who am i - 1
In this task we did a script that prints the effective username of the current user by using command `whoami`.

## Groups - 2
We used `groups` command to print out all the group associated with current user.

## New owner - 3
We aim to change the owner of the file `hello` to the user `betty`
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
We then changed the permission of the `hello` file so that both owner and group will have no permissions at all and then other user have all permissions by using `chmod 007 hello`.



## Amazing work
whhakkakjakjskjksaksajkjkasjkjsakjkjsa
hjajh
---
Wanna test on yourself :smile: feel free to use use those scripts.
