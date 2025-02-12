# I/O Redirections and Filters

## Hello World and Smiley - 0&1
Where in this tasks we are required to print `Hello, World ` and `confused smiley`  and we simply used echo command.

## Displaying a file - 2
In this repository we used simple `cat` command to display content of our file `/etc/passwd`.

## What about 2 - 3
As we are required to display content of the two files at the same time while maintaing the rules of the task , we simply used `cat` and then parse the first file_name and then parse the second file_name. 

## Last lines of a file - 4
To display the last lines of a file we have to use `tail` and parse the `-n` which is amodern form to specify that we will be working with lines and then number of last line to look for and in our case is `10` and then file_name as last.

## Prefering First lines - 5
As different to task 4 here we just have to display the first lines and instead of using `tail` we used `head` and it works the same way for other parts.

## Line2 - 6
We are required to write a script that will display the third line of the file `iacta`, so to accomplish that task we used:
- `head -n 3 file_name`: First we want to be able to get the first three lines using `head` from the file content.
- `tail -n 1`: And then parse the last line in the three lines we got before and here we go.

## Cut iron without making noise - 7
We are required to create file names exactly `\*\\'"Best School"\'\\*$\?\*\*\*\*\*:)` and to accomplish that we just have to use special character `\` before every character in the name of the file so that the interpreter will know that the following character is not special character; by using that logic we go with `echo " Best School" >` plus the file_name with backslach.

## Save current state of dir - 8
W achived the automation by simply parse command `ls -la` to the file `ls_csd_content` and accomplish that using `echo "command"> file_name`.

## Duplicate last line - 9
To duplicate the last line we must first get that last line and we get it by `tail -n 1 file_name` and then duplicate it using redirections `>>`so the complete commands are `tail -n 1 file_name <iacta>> iacta`.

## No more js - 10
To remove all regular files with a `.js` extension in the current directory and all its subfolders, we used 
- `find .` : to look in the current directory, and 
- `-type f`: to specify that we will be looking for files only
- `-name "*.js"`: We also clarify to look for the files which ends with `.js`, and then 
- `-delete`: Finally to the action of deleting it.

## Don't count - 11
To count the number of dirs and sub-dirs in the current dir and then make sure the hidden dirs are counted and not include the current and parental dirs. As the way to accomplish that we used `echo "logic"`to print the output. Okay let's elaborate more on the logic behind:
- `find .`: to find in the our current dir.
- `-type d`: to specify the type of stuffs we will be looking for.
- `-not path '.'` and `-not path './..'`: To clarify that we will not include current dir and parental dir as well.

## What's new - 12
In this task we have to display the 10 newest files in the current directory, one file per line and then sort from the newest to the oldest one , so to accomplish this kind of automation we used `ls -1t` to sort the files basing on the date/time and then we used `head -n 10` to get the lastest 10 files asap.

## Uniqueness - 13
we was required to write a script that tales a list of words as input and prints only words that appear exactly once and also we must make sure the words are being sorted, so here we used `sort` first to sort all the words and then we parse `uniq -u`.

## In that file - 14
By using `grep` and then the pattern plus the file_name we can simply display the lines containing that pattern from file's  content.

## Count that word - 15
We simply required to display the number of lines that contain pattern `bin` in the given file and we accomplish that by using `cat"pattern " filename `and then pipe `wc -l`to count the lines.

## What's next - 16
Displaying the lines containg patter `root` and add 3 lines after them where we used `grep` and then `-A 3` to specify that we will add 3 lines after, and finally pattern plus file_path.

## Hating bins - 17
Display all the lines in the file `/etc/pasword`that don't contain the pattern `bin`, and we did that by using `grep !"bin"` and then parse file_path.

## Letters only - 18
Display all lines of the file `/etc/ssh/sshd_config` starting with a letter including capital letters as well. We used `grep "^[A-Za-z]"` and then parse the file path.

## A to Z - 19
We leveraged the `tr` and then `Ac Ze`and get the work done.

## Hiago - 20
As required to remove all letters `c` and `C` from input we accomplished that automation using `tr -d "cC"`. 
