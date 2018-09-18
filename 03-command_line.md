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

* `pwd`: show current directory path
* `mkdir`: creating a directory
* `rm -rf`: deleting a directory
* `touch`: create empty file
* `rm`: deleting a file
* `mv`: renaming a file
* `ls -a | grep "^\."`: listing hidden files
* `cp`: copying a file from one directory to another
* `cat`: reads files sequentially, writing them to the standard output
* `grep`: searches any given input files, selecting lines that match one or more patterns

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

`ls`: lists the contents of a directory
`ls -a`: lists both hidden and unhidden contents of a directory
`ls -l`: lists files and directories as a table
`ls -lh`: lists files and directories as a table and use unit suffixes: Byte, Kilobyte, Megabyte etc.
`ls -lah`:  lists directory entries whose names begin with a dot
`ls -t`: orders files and directories by the time they were last modified.
`ls -Glp`: enables colorized output and writes a slash after each filename if that file is a directory

---

### Q3.  More List Files in Unix

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

`-a`: displays all files
`-d`: displays only directories
`-r`: displays files in reverse order
`-t`: displays newest files first (based on timestamp)
`-l`: displays the long format listing

---

### Q4.  Xargs

What does `xargs` do? Give an example of how to use it.

`xargs`: reads items from standard input as separated by blanks and executes a command once for each argument.
```shell
echo 'one two three' | xargs mkdir
ls
one two three
```


