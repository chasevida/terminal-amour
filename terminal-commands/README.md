# Terminal Commands
Listed here are a few of the most common day to day commands you may find yourself needing when using the terminal.

The command structure is pretty simple and follows a well defined path:

	$ command [-option(s)] [argument(s)]


Command    | Operation
---------- | -------------
pwd        | print working directory
ls         | list all files in the current working directory
cd         | change directory
touch      | create file or if it exists update it's read time
mkdir      | create a new directory
mv         | move or rename a file or directory
rm         | delete a file or directory
cp         | copy file
chown      | change owner
chmod      | change permission


## LS
`$ ls` has a few additional options that make it a little more useful.

Command    | Operation
---------- | -------------
ls         | list all files in the current working directory
ls -l      | format the list vertically
ls -a      | include all hidden/system files
ls -h      | format the size as human readable
ls -lah    | combines all the above options

## RM
`$ rm` has a few additional options that make it a little more useful.

Command    | Operation
---------- | -------------
rm         | delete a file or directory
rm -f      | force the deletion
rm -r      | delete the content recursively
rm -rf     | combines all the above options