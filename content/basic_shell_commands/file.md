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
# to remove a folder
rm -r <folder name>
```


## Copy
cp
cp -r

## Move
mv

## Read
cat
less
head
tail

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
