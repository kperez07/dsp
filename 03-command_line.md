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

> > pwd = shows current working directory path
mkdir = make directory (or folder)
rmdir = delete a directory
touch filename = create a file
rmfilename = delete a file
mv oldfilename newfilename = change a file name
ls -ld .?* = list hidden files/directories
cp filename directoryname = copying file from one location to another
grep = search for the word/file you are looking for from history
history = shows all last commands that were written
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

> > ls = lists everything in the current directory
ls -a = list with hidden files
ls -l = displays mtimes (last file data modification times)
ls -lh = lists long format with readable file size
ls -lah = lists long format with readable file size with hidden files
ls -t = sorts files/directories by time/date
ls -Glp = in a long listing don't print group names, displays modification times, append indicator to directories (adds a slash to directories)
---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > ls -t = displays in order by timestamp
ls -d = displays only directories
ls -R = displays subdirectories as well
ls -u = displays files by file access time
ls -o = Displays the long format listing, but excludes group name.
---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > xargs divides a big list of into a sub list received from standard input. 
ls | xargs grep searchterm = this adds the output of ls files to grep searchterm files, so it will ID which files in the ls have your searchterm that you are looking for. 
 

