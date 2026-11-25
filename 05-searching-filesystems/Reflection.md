# Topic 5: Searching and Navigating the Linux File System

## Practical Commands

During this lab, I explored ways to locate files and search for specific text within Linux. I learned that these commands are useful when working with a server that contains many files and directories.

I practised using `find` to locate a file by its name. For example:

`find /home/ubuntu -name "notes.txt"`

The command located my `notes.txt` file inside the `practice` directory.

I also used `grep` to search for specific words within a text file. I added sample Linux-related sentences to `notes.txt` and ran:

`grep "Linux" notes.txt`

The command displayed the lines containing the word "Linux".

## What I Learned

The main difference I noticed is that `find` searches for files and directories, while `grep` searches for text within files. Both commands make it easier to locate information without manually opening every file.

These skills are useful when troubleshooting Linux servers, searching through configuration files and checking log files. For example, system administrators can use `grep` to identify error messages in server logs.
