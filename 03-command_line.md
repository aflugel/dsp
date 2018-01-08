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
> >   * `chmod` general:
> >      * Who are we changing the permission for? [ugoa] - user (or owner), group, others, all
> >      * granting or revoking the permission = indicated with either a plus (+) or minus (-)
> >      * Which permission are we setting? - read (r), write (w) or execute (x)
> > * shebang (specifies interpreter/program for the rest of the script = `#!<path>` eg. `#!/bin/bash`
> > * command substitution (save output as variable) = `variable=$(<commands>)` (only saves first line of output!)
> > * make variable available to child processes = `export <variable>`
> > * get manual for a command = `man <command>`
> >   * search while in manual = `/` + `<search term>` + enter
> >   * quit = `q`
> >   * search all manual pages = `man -k <search term>`
> > * view contents of file = `cat <filename>`
> >   * cancel = `^C`
> > * view contents of a larger file piece by piece = `less <filename>`
> >   * move up and down with arrow keys
> >   * move forward by a whole page with spacebar
> >   * move backward by a whole page with `b`
> >   * quit = `q`  
> > * Find length of a variable (how many characters) = `${#variable}`

> > #### FILTERS  
> > * `head [-number of lines to print] [path]` = prints first X lines of input (default =10)
> > * `tail [-number of lines to print] [path]` = like head, but looks at the LAST lines
> > * `sort [-options] [path]` = sorts output, default is alphabetical
> > * `nl [-options] [path]` = numbers the lines
> >   * `-s [string]` = specifies what to print after each number
> >   * `-w [int]` = specifies how much padding before the numbers
> > * `wc [-options] [path]` = word count (words, characters, lines)
> >   * `-l` = lines only
> >   * `-w` = words only
> >   * `-l` = lines only
> >   * `-m` = characters only
> > * `cut [-options] [path]` = pulls specified data from input
> >   * `-d '<string>'` = specifies separators (default is tab)
> >   * `f <number(s)>` = specifies desired fields
> > * `uniq [options] [path]` = removes duplicate lines (only when adjacent)
> > * `tac [path]` = backwards `cat`, reads input last line -> first line
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

> > `xargs` allows the user to run a command on every item in a list. By default, it takes the stdinput and echoes it.  If you pipe the output from another command or program into `xargs`, you can perform a task on each output item.  
> > #### Example:
> > If I take a bunch of screenshots on my Mac, I'll end up with a messy desktop cluttered with dated screenshot files (eg. 'screenshot 2017-12-23 at 5.54.37 PM.png'). I can run the following script to move all of those files to a folder called 'screenshots'.  
> > `find screenshot*.png -print0 | xargs -0 -I{} mv {} screenshots/{}`

 

