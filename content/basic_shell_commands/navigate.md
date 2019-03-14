# Navigate
Before we start navigating the file system, we need to have the concept about working directory, file system, as well as physical path and relative path.

## Home Directory
If you start your terminal, you will be in a directory. This directory is your "Home Directory". 
In shell, "~" is used to represent your home directory. 
([Teleport](http://www.linfo.org/home_directory.html))

## Working Directory
After you log into your system, your working directory is your home directory. 
After you navigate to different directories, 
the working directory will be the directory you are in.

## Brief Intro to File system
1. Everything in Linux is file.
2. Each file has a path.
3. The file system is like a tree (hierarchical directory structure) with links here and there, but generally a tree.
4. The root (path) of the file system is '/' aka root directory.

## Physical Path and Relative Path
Physical path is the relative path of the file with the root directory (need double check).
| | |
|-|-|
| .. or ../ | parent folder. |
| . | current folder. |
| ../../ | two folders up. |
| .././ | one folder up and current folder, which in total is one folder up. |
|/usr/../usr/./ | you are actually in  /usr/ |

## Commands
These commands will help you move around in shell.
### pwd
Shows your working directory, which is your current directory.
### cd (chdir)
Change directory

| | |
|-|-|
| cd - | change to the previous working directory. |
| cd ~ | change to home directory. |
| cd / | change to root directory. |
| cd /some/path | change to /some/path |
| cd .. | change to upper directory |
| cd . | change to current directory |


```
Tip: use tab to auto complete, click tab twice will show you the contents in entered path.
```

