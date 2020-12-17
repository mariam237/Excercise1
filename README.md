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
