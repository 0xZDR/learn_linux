# Manipulate Files
In Linux, everything is file this includes Configurations, Sockets, Process ids, etc. Hence, knowing how to interact with file system is crucial for you. Here we separate the actions into different categories.


## Show Files
### ls
Before we create or remove any file, we need to see what we have in your current working directory.

_ls_ is the command for listing files in your working directory.
```
# usage
# show files
ls
# show all files
ls -a
# show files in list
ls -l
# show all files in list and with human readable format
ls -alh
# the above command is the one I use the most due to the clear format it provides.
```
#### Hidden files
The files starting with "."
You need "-a" to show the hidden fiels.

## Create

### touch
This might be the easiest way to create a file in Linux.
```
# usage
touch file
# or
touch file1 file2 file3
```
Alternatively, one can use [pipeline redirection](../content/pipeline.md) or editors([vim](../content/vim.md)) to create a new file.

[Here](http://www.linfo.org/touch.html) is a more detailed instruction of touch.

## Remove

### rm
After you created a file, you should be able to delete it. The command to remove something in the file system is 'rm'.
```
# usage
# to remove one file
rm <file name>
# to remove multiple files
rm <file name 1> <file name 2> <file name 3>
# to remove a folder
rm -r <folder name>
```
> __IMPORTANT:__ do double check before you remove things

> __IMPORTANT:__ do not do rm -rf /

## Copy
### cp
```
# usage
cp <source file> <target file>
cp <source file 1> <source file 2> <target directory>
# copy recursively 
cp -R <source directory> <target directory>
```

## Move
### mv
```
mv source target
mv source ... directory
```

## Read
### cat
Concatenate and print files
```
# usage
# to simply print a file
cat file
# to concatenate files
cat file1 file2
# to concatenate files and save them to a new file 
cat file1 file2 > file3

# ctrl + d is the EOF signal, so you can use this
cat > file
# you can copy paste your file to the stdin at this time and hit ctrl + d to have everything casted into the file
```

here we mentioned [pipeline redirection](), you can click on the link to 
### less
http://man7.org/linux/man-pages/man1/less.1.html
### head
http://man7.org/linux/man-pages/man1/head.1.html
### tail
http://man7.org/linux/man-pages/man1/tail.1.html
```
# usage
# this is very useful for reading logs
tail -f
```
