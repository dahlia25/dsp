# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > Below is a short list of commands:
1. `pwd` shows current working directory path
2. `mkdir` creates a new directory/file
3. `rmdir` deletes a directory
4. `touch *new_file_name_here*` creates a file using `touch` command
5. `rm` deletes a file
6. `mv` can rename or move a file
7. `ls -a` lists all hidden files
8. `cp` copies a file from one directory to another
9. `cd` changes the directory
10. `sudo` command allows you to temporarily become another user

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

> > Below is a description of the commands listed above:
* `ls` lists all files in current working directory
* `ls -a` lists all *hidden* files, including those that start with '.'
* `ls -l` lists all files in long format, where the owner (permissions), group, size and time are shown
* `ls -lh` lists all files with readable file size in long format
* `ls -lah` lists all hidden files with readable file size in long format
* `ls -t` lists and sorts all files by date and time
* `ls -Glp` lists all files in a long format without including group names, and appends **/** indicator to all directories

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > The following are some of my favorites:
1. `ls -r` lists and sorts all files in reverse alphabetical order
2. `ls -X` lists and sorts by extension names
3. `ls -u` lists and displays files by file access time
4. `ls -R` lists and shows subdirectories as well
5. `ls -q` lists and shows all nonprinting characters as **?**

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > The **xargs** command allows commands such as mkdir, rm to accept standard inputs as arguments. By default, the command is executed once on all arguments in standard input, separated by blanks.

*For Example:* Assuming the following three directories exist: 'a', 'b' and 'c'. In this case, the three directories are the standard inputs. We will use `xargs` to execute the `echo` and `rmdir` commands on each standard input in which are converted to arguments.
`echo 'a b c' | xargs rmdir`

Dicectories 'a', 'b' and 'c' will be deleted after the code aboveis executed.
 

