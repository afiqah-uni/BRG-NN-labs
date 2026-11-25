# 2. Exploring Ubuntu Desktop and CLI Tools

## Introduction

This practical activity introduced me to the Ubuntu desktop environment and Linux command-line interface (CLI). I learned how to navigate directories, view files and folders, create directories and files, and explore the Linux file system using terminal commands.

## Tools Used

- UTM virtualisation software
- Ubuntu Linux
- Ubuntu Terminal

## Practical Experience

I started by opening the Ubuntu Terminal in my UTM virtual machine. I used several basic Linux commands to understand how to navigate and manage files and directories.

First, I used `pwd` to display my current working directory. The output showed `/home/ubuntu`, which is the home directory of my Ubuntu user account.

Next, I used `ls` to list the files and folders in my home directory. This displayed standard directories such as Desktop, Documents, Downloads, Music and Pictures.

I then practised creating and navigating directories using `mkdir` and `cd`. I created a directory named `practice` and entered it. After that, I used `touch notes.txt` to create an empty text file inside the directory.

I also tried `man ls` to access the manual page for the `ls` command. It displayed detailed information about the command and its available options.

## Exploring the Linux File System

After practising the basic commands, I explored the main Linux directory structure.

I used `ls /` to view the directories located at the root of the file system. I learned that Linux organises its files into different directories, each serving a specific purpose.

I explored two important directories:

**1. `/etc` – System Configuration**

I used `ls /etc` to view its contents. I noticed folders such as `apache2`, `ssh`, `apt` and `systemd`. This helped me understand that `/etc` stores configuration files used by the operating system and its services.

**2. `/var` – Variable Data**

I used `ls /var` to view its contents. I noticed directories such as `log`, `cache`, `backups` and `lib`. I learned that `/var` stores data that can change while the system is running. In particular, `/var/log` is important because it contains log files that can help administrators investigate system activity and errors.

## Commands Practised

| Command | Purpose |
|---|---|
| `pwd` | Displays the current working directory |
| `ls` | Lists files and directories |
| `mkdir practice` | Creates a directory named practice |
| `cd practice` | Changes into the practice directory |
| `touch notes.txt` | Creates an empty text file |
| `man ls` | Displays the manual for the ls command |
| `ls /` | Lists the main root directories |
| `ls /etc` | Lists system configuration files and directories |
| `ls /var` | Lists directories containing variable system data |

## Challenges and Reflection

At first, I was unfamiliar with the Linux directory structure and the purpose of the different terminal commands. However, practising each command individually helped me understand how they work and how they can be used together.

I also learned that Linux uses a structured directory system rather than organising everything in the same location. Understanding directories such as `/etc` and `/var` is useful when managing and troubleshooting a Linux server.

Overall, this activity helped me become more comfortable using the Ubuntu Terminal. These basic CLI skills will be important for the later practical activities involving Linux services, file permissions and server administration.
