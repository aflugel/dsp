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

> > * show current working directory path = `pwd`
> > * creating a directory = `mkdir [options] <directory_name>`
> >   * make parent directories as needed = `-p`
> >   * print out what the command is doing = `-v`
> > * deleting a directory = `rmdir [options] <directory_name>`
> > * creating a file using `touch` command = `touch [options] <filename>` 
> >   * this changes the access/modification times on a file, or creates the file if it doesn't exist
> > * deleting a file = `rm [options] <filename>`
> >   * delete directory and all files/directories it contains = `-r` (recursive)
> >   * prompt before removing each file/directory = `-i` (interactive)
> > * renaming a file = `mv <oldname> <newname>` within the same directory as source
> > * listing hidden files = `ls -a`
> > * copying a file from one directory to another = `cp [options] <source> <destination>`
> >   * copy directory and all files/directories it contains = `-r` (recursive)
> > * assign read, write, and execute permissions= `chmod 755 <script>`
> > * shebang (specifies interpreter/program for the rest of the script = `#!<path>` eg. `#!/bin/bash`
> > * command substitution (save output as variable) = `variable=$(<commands>)` (only saves first line of output!)
> > * make variable available to child processes = `export <variable>`
> > * get manual for a command = `man <command>`
> >   * search while in manual = `/` + `<search term>` + enter
> >   * quit = `q`
> >   * search all manual pages = `man -k <search term>`

---

### Q2.  List Files in Unix   

What do the following commands do:  
> > `ls` = list files and directories in current working directory (or other specified location)  
> > `ls -a` = list INCLUDING hidden files/directories  
> > `ls -l` = list in long format  
> > `ls -lh` = list in long format with unit suffixes for file sizes  
> > `ls -lah` = list in long format, with unit suffixes, and include hidden items  
> > `ls -t` = list, sorting by time modified (recent first)  
> > `ls -Glp` = list in long format, with colorized output, adds `/` after file name for directories


---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > `-R` = recursively lists subdirectories as well  
> > `-d` = displays only directories  
> > `-g` = long format, minus owner name  
> > `-m` = returns results as a comma-separated list  
> > `-F` = lists with flagged file names
> >   * directories end with `/`
> >   * executables end with `*`
> >   * symbolic links end with `@`
> >   * sockets end with `=`
> >   * whiteouts end with `%`
> >   * FIFOs end with `|`

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > REPLACE THIS TEXT WITH YOUR RESPONSE

 

