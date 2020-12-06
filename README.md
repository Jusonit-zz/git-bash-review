# Review notes for Git Bash

## Git is a version control system for tracking changes in computer files.

*Initialize a local git repository, creates a .git folder*
`$ git init`

*Add file(s) to index  (to be committed)*
`$ git add <filename>`

*Add all files to index*
`$ git add .`

*To discard changes in the directory*
`$ git restore <file>`

*Remove file(s) from index (not to be committed)*
`$ git rm --cached <filename>`

*Check status of working tree*
`$ git status`

*Commit changes in index*
`$ git commit`

*Commit changes without using an editor for the comment*
`$ git commit -m "comment"`

*Push to remote repository*
`$ git push -u origin master`
*another way:*
`$ git push -f origin master`

*Pull latest changes from remote repository*
`$ git pull`

*Clone repository into a new directory*
`$ git clone <url>`

*Create a new branch*
`$ git branch <branch_name>`

*Merge branches to master*
`$ git merge <branch_name>`

*Go to different branch*
`$ git checkout <branch_name>`

*Create a gitignore file*
`$ touch .gitignore`

*Remove files/folder with gitignore that are already in the repository*
`$ git rm -rf --cached .`
`$ git add .`

------------

<br>

## Bash commands
### (file commands)

*lists your files in current directory *
`ls`

*list files in specific directory*
`ls <dir>`

*lists your files in long format, which contains the exact size of the file, who owns the file and who has the right to look at it, and when it was last modified*
`ls -l`

*lists all files in long format, including hidden files (name beginning with '.')*
`ls -a`

*creates or updates (edit) your file*
`touch <filename>`

*prints file raw content (will not be interpreted)*
`cat <filename>` 

*outputs the first lines of file (default: 10 lines)*
`head <filename>`

*outputs the last lines of file (useful with -f option) (default: 10 lines)*
`tail <filename>`

*opens a file in VIM (VI iMproved) text editor, will create it if it doesn't exist*
`vim <filename>`

*moves a file to destination*
`mv <filename1> <dest>`

*copies a file*
`cp <filename1> <dest>`

*removes a file*
`rm <filename>`

*searches for a file or a directory in the current directory and all its sub-directories by its name*
`find . -name <name> <type>`

*compares files, and shows where they differ*
`diff <filename1> <filename2>`

*tells you how many lines, words and characters there are in a file. Use -lwc (lines, word, character) to ouput only 1 of those informations*
`wc <filename>`

*sorts the contents of a text file line by line in alphabetical order, use -n for numeric sort and -r for reversing order.*
`sort <filename>`

*lets you change the read, write, and execute permissions on your files*
`chmod -options <filename>`

*compresses files*
`gzip <filename>`

*uncompresses files compressed by gzip*
`gunzip <filename>`

*lets you look at gzipped file without actually having to gunzip it*
`gzcat <filename>`

*prints the file*
`lpr <filename>`

*looks for the string in the files*
`grep <pattern> <filenames>`

*search recursively for pattern in directory*
`grep -r <pattern> <dir>`

------------

### (directory commands)

*makes a new directory*
`mkdir <dirname>`

*remove an empty directory*
`rmdir <dirname>`

*remove a non-empty directory*
`rmdir -rf <dirname>`

*rename a directory from dir1 to dir2*
`mv <dir1> <dir2>`

*changes to the parent directory*
`cd ..`

*changes directory*
`cd <dirname>`

*copy dir1 into dir2 including sub-directories*
`cp -r <dir1> <dir2>`

*tells you where you currently are*
`pwd`

*changes to home*
`cd ~`

------------