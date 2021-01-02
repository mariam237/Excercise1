# Excercise1
1.
$ mkdir LC && cd LC

2.
$ touch test

3.
$ echo '#!/bin/bash' > test
$ echo "curl --head --silent google.com" >> test

SH (SHell)
Is a specific shell
a command interpreter and a programming language
Predecessor of BASH

BASH (Bourne-Again SHell)
Is a specific shell
a command interpreter and a programming language
Has sh functionality and more
Successor of SH
BASH is the default SHELL

4.
$ ./test
$ ls -l
The permission bits is -rw-r--r--, so we are not allowed to execute the file.

5.
we dont need permission to run test using sh, but we need permission when using ./test

6.
chmod is the command and system call which is used to change the access permissions of file system objects (files and directories). It is also used to change special mode flags. The request is filtered by the umask. The name is an abbreviation of change mode.

7.
Chmod 744 (chmod a+rwx,g-wx,o-wx) sets permissions so that, (U)ser / owner can read, can write and can execute. (G)roup can read, can't write and can't execute. (O)thers can read, can't write and can't execute
As the first line in the file is #!/bin/sh , the program loader is instructed to run the file with /bin/sh.

8.
$ echo '#!/usr/bin/python3' > test.py
$ echo "print("Hello World!")" >> test.py
$ chmod 755 ./test.py
$ ./test.py

9.
The >> appends to a file or creates the file if it doesn't exist.
The > overwrites the file if it exists or creates it if it doesn't exist.

10.
$ echo "alias ll='ls-alh'" >> ~/.bashrc
$ source ~/.bashrc
$ ll


## Excercise 2
1. Done

2. 
It reads lines from stdin , launches an interactive finder dialogue, and finally writes selected items to stdout . The key point and difference from tools like GNU find , is its interactive finder dialogue that filters items instantly as you type.

3.


4.
The history command shows a list of the commands entered since you started the session.
if you need the output of the .bash_history file cat ~/.bash_history

5.
A symbolic link creates a file in your directory and acts as a shortcut to a file or folder.
ln is a command-line utility for creating links between files. By default, the ln command creates hard links. To create a symbolic link, use the -s (--symbolic) option.
ln -s

6.
diff works by cataloging the changes between the two files or folders. Patch can take those changes, put them in a file, and update older versions with it.
