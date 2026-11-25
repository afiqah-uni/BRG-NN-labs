
# 2. Exploring Ubuntu Desktop and CLI Tools

## Introduction

This practical activity introduced me to the Ubuntu desktop environment and Linux Command-Line Interface (CLI). I learned how to navigate directories, view files and folders, create directories and files, and explore the Linux file system using terminal commands.

## Tools Used

- UTM virtualisation software
- Ubuntu Linux
- Ubuntu Terminal

## My Practical Experience

I started by opening the Ubuntu Terminal in my UTM virtual machine. I practised several basic Linux commands to understand how to navigate and manage files and directories.

First, I used the `pwd` command, which stands for Print Working Directory. It displayed `/home/ubuntu`, showing that I was currently inside my Ubuntu user's home directory.

Next, I used the `ls` command to list the contents of my home directory. The output displayed folders such as Desktop, Documents, Downloads, Music, Pictures and Videos. This helped me understand how Ubuntu organises a user's personal files and folders.

I then practised creating and navigating directories. Using `mkdir practice`, I created a new folder called `practice`. After that, I used `cd practice` to enter the folder. I confirmed my new location by running `pwd` again, which displayed `/home/ubuntu/practice`.

While inside the practice directory, I used `touch notes.txt` to create an empty text file. I then ran `ls` to check that the file had been created successfully.

I also explored the `man` command by entering `man ls`. This opened the manual page for the `ls` command, which contained detailed information about its usage and available options. Although there was a lot of information displayed, I learned that the manual is useful when I need help understanding a Linux command.

## Exploring the Linux File System

After practising the basic commands, I explored the main Linux directory structure using `ls /`. This displayed the directories located at the root of the file system.

I learned that Linux organises its files into different directories, each serving a particular purpose. I focused on exploring `/etc` and `/var` because they are important when managing and maintaining a Linux system.

### Exploring `/etc`

I entered `ls /etc` to view the contents of the `/etc` directory. I noticed several configuration folders, including `apache2`, `ssh`, `apt` and `systemd`.

From this activity, I learned that `/etc` stores system configuration files. These files help control how the operating system and its installed services behave. For example, the `apache2` directory contains configuration files related to the Apache web server.

### Exploring `/var`

Next, I entered `ls /var` to explore the `/var` directory. The output displayed folders such as `backups`, `cache`, `lib`, `log` and `spool`.

I learned that `/var` stores data that changes while the system is running. One important example is `/var/log`, which contains system and application log files. These logs are useful for system administrators because they can help identify errors and troubleshoot problems.

## Challenges and Reflection

At first, I was unfamiliar with the Linux directory structure and the purpose of the different terminal commands. However, practising each command individually helped me understand how they work and how they can be used together.

One thing I found useful was being able to create my own directory and file using `mkdir` and `touch`. This allowed me to practise managing files directly through the terminal instead of relying only on the graphical desktop environment.

Exploring `/etc` and `/var` also helped me understand how Linux separates configuration files from changing system data. I realised that knowing where these files are stored is important when troubleshooting and managing a server.

Overall, this activity helped me become more comfortable using the Ubuntu Terminal. These basic CLI skills will be useful in the later practical activities involving Linux services, file permissions, server configuration and system administration.
