# An introduction to Linux
## Intro
This repo is mainly aiming at helping a person to get familiar with Linux and can start using Linux.
Some of these are written by me, and some are referred to other resources.
I constructed a structure of the knowledge on a gradual base, and hopefully can help you get into the world of Linux.

Disclaimer: English is my second language. If you are confused, please let me know. Also if you find anything that is not correct, please do let me know; I hope this repo can help people but not mislead them.


## Brief History of Linux
Before going into linux, read this might help you understanding the relations between different Linux distributions and why some programmers prefer Macbooks. 

* [What is POSIX?](https://stackoverflow.com/questions/1780599/what-is-the-meaning-of-posix)
* [History of Unix and Linux](https://www.oreilly.com/library/view/running-linux-third/156592469X/ch01s02.html)


## What is Operating System
To understand what is OS, you need to understand hardware and how programs are ran on hardwares.
Here we use SCM (Single Chip Microcomputer) as an example.
How can multiple programs run on one chip?
Even if we have multiple programs running, how can we stop them intervene each others' memory?
How do we manage files?
What about interrupts?

Now we need something to operate these 'resources', which introduces us into Operating Systems.

### Kernel
To my understanding, kernel is the most essential part of an OS, which includes all necessary functions to "operate" the resources. But this is just a simple and partial description, you can read this.
[What is kernel](https://stackoverflow.com/questions/2013937/what-is-an-os-kernel-how-does-it-differ-from-an-operating-system)


### Shell
After you have a kernel, how would you interact with it? When you want to send commands to the kernel, you have your very OG user interface ---- the shell.
* [What is shell?](http://linuxcommand.org/lc3_lts0010.php)
> 🚧🚧🚧 this part might need redo 🚧🚧🚧


## Basic Shell Commands (BASH)
So now we know what kernel and shell are, we can go into shell commands.
Here, we will be talking about [Bash](https://www.gnu.org/software/bash/manual/html_node/What-is-Bash_003f.html).

In case you want to save some time, [here](https://www.digitalocean.com/community/tutorials/basic-linux-navigation-and-file-management) is a tutorial from digital ocean.

### Navigate
Before we start navigating the file system, we need to have the concept about working directory, file system, as well as physical path and relative path.

#### Home Directory
If you start your terminal, you will be in a directory. This directory is your "Home Directory". 
In shell, "~" is used to represent your home directory. 
([Teleport](http://www.linfo.org/home_directory.html))

#### Working Directory
After you log into your system, your working directory is your home directory. 
After you navigate to different directories, 
the working directory will be the directory you are in.

#### Brief Intro to File system
1. Everything in Linux is file.
2. Each file has a path.
3. The file system is like a tree (hierarchical directory structure) with links here and there, but generally a tree.
4. The root (path) of the file system is '/' aka root directory.

#### Physical Path and Relative Path
Physical path is the relative path of the file with the root directory (need double check).

Path ".." or "../" means parent folder.

Path "." means current folder.

Path "../../" means two folders up.

Path ".././" means one folder up and current folder, which in total is one folder up.

In this case, if we are in path "/usr/../usr/./" you are actually in "/usr/"

#### Commands
##### pwd
Shows your working directory, which is your current directory.
##### cd
Change directory.
You need to know "cd -", "cd ~", "cd /" and use with relative paths.


> 🚧🚧🚧 everything below is under construction 🚧🚧🚧

[Teleport to file system(currently under construction)]()


### Manipulate File System

#### Read Files

 touch
* mv
* cp
* mkdir
  * mkdir -p 
* cat
* less
    |key|usage|
    |---|---|
    |j|one line down|
    |k|one line up|
    |d|half page down|
    |u|half page up|
    |space/f|page down|
    |b|page up|
    |/\<content\> + Enter| search |
    |/\<content\>/-i + Enter| search ignore case|
    |n|find next|
    |N|find previous|
    |G|go to bottom|
    |gg|go to top|

* tail
* head
* cut
* sed
* echo

### Conventional Paths
[Here](https://en.wikipedia.org/wiki/Filesystem_Hierarchy_Standard) are some conventional Linux paths, you will understand why some packages are storaged under certain folders
### .bash_profile
#### Environmental Variables
#### Understanding $PATH
#### Alias
### Pipeline Redirection

[this](./content/basic_linux_commands.md)
* [Pipeline, Redirection & Environmental Variables](./content/pipeline_redirection_and_environmental_variables.md)
* [Shell Script](./content/shell_script.md)
* [User, 
Group & File Access](./content/user_group_and_file_access.md)
* [Iptables & Firewalld](./content/iptables_firewalld.md)
* [ssh](./content/ssh.md)


* [Vim](./content/vim.md)