# The Simple_Shell :
# A simple UNIX command interpreter.

## DESCRIPTION

__*Simple_Shell*__ is a type of program called an interpreter. An interpreter operates in a simple loop: It accepts a command, interprets the command, executes the command, and then waits for another command. The shell displays a "prompt," to notify you that it is ready to accept your command. 

The goal of the project is to make us understand how the shell works by coding a light version with basic command.

***

## REQUIREMENTS

* All files have been compiled on Ubuntu 20.04 LTS
* All your files should end with a new line
* A README.md file, at the root of the folder of the project is mandatory
* Code should use the Betty style
* Shell should not have any memory leaks
* No more than 5 functions per file
* All header files should be include guarded

## COMPILATION
```gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh```

## Return value
This function has no return value.


## LIST OF AUTHORIZED FUNCTIONS
* ***access*** (man 2 access)
* ***chdir*** (man 2 chdir)
* ***close*** (man 2 close)
* ***closedir*** (man 3 closedir)
* ***execve*** (man 2 execve)
* ***exit*** (man 3 exit)
* ***_exit*** (man 2 _exit)
* ***fflush*** (man 3 fflush)
* ***fork*** (man 2 fork)
* ***free*** (man 3 free)
* ***getcwd*** (man 3 getcwd)
* ***getline*** (man 3 getline)
* ***getpid*** (man 2 getpid)
* ***isatty*** (man 3 isatty)
* ***kill*** (man 2 kill)
* ***malloc*** (man 3 malloc)
* ***open*** (man 2 open)
* ***opendir*** (man 3 opendir)
* ***perror*** (man 3 perror)
* ***printf*** (man 3 printf)
* ***fprintf*** (man 3 fprintf)
* ***vfprintf*** (man 3 vfprintf)
* ***sprintf*** (man 3 sprintf)
* ***putchar*** (man 3 putchar)
* ***read*** (man 2 read)
* ***readdir*** (man 3 readdir)
* ***signal*** (man 2 signal)
* ***stat*** (__xstat) (man 2 stat)
* ***lstat*** (__lxstat) (man 2 lstat)
* ***fstat*** (__fxstat) (man 2 fstat)
* ***strtok*** (man 3 strtok)
* ***wait*** (man 2 wait)
* ***waitpid*** (man 2 waitpid)
* ***wait3*** (man 2 wait3)
* ***wait4*** (man 2 wait4)
* ***write*** (man 2 write)

## MAN PAGE EXECUTION
```man ./man_1_simple_shell```

## EXAMPLES
```
♥♥ WE LOVE SIPHAN ♥♥ ls -l
total 80
-rw-rw-r-- 1 simon simon   211 Dec  8 16:09 AUTHORS
-rw-rw-r-- 1 simon simon  2143 Dec  8 21:42 README.md
-rw-rw-r-- 1 simon simon   660 Dec  7 13:44 execve.c
-rw-rw-r-- 1 simon simon   277 Dec  7 13:44 freegrid.c
-rw-rw-r-- 1 simon simon   333 Dec  7 13:44 getenv.c
-rw-rw-r-- 1 simon simon   665 Dec  7 13:44 getpath.c
drwxrwxr-x 2 simon simon  4096 Dec  8 16:07 hack
-rwxrwxr-x 1 simon simon 18168 Dec  8 16:14 hsh
-rw-rw-r-- 1 simon simon   679 Dec  8 16:09 main_shell.c
-rw-rw-r-- 1 simon simon   257 Dec  7 13:44 printenv.c
-rw-rw-r-- 1 simon simon   420 Dec  7 13:44 readcmd.c
-rw-rw-r-- 1 simon simon   704 Dec  7 13:44 shell.h
-rw-rw-r-- 1 simon simon   520 Dec  7 13:44 split.c
-rw-rw-r-- 1 simon simon   475 Dec  7 13:44 splitenv.c
-rw-rw-r-- 1 simon simon  1195 Dec  7 13:44 struse.c
-rw-rw-r-- 1 simon simon   615 Dec  7 13:44 trim.c

♥♥ WE LOVE SIPHAN ♥♥ /bin/ls
AUTHORS  README.md  execve.c  freegrid.c  getenv.c  getpath.c  hack  hsh  main_shell.c	printenv.c  readcmd.c  shell.h	split.c  splitenv.c  struse.c  trim.c

♥♥ WE LOVE SIPHAN ♥♥ pwd
/home/simon/Documents/Holberton_School/simple-shell-test
```

## MEMORY CHECK
valgrind ./hsh

## BUG REPORT
* ```ls -l``` command have some error
* ```/bin/ls``` command have some error
* ```fork``` is called when a command doesn't exist
* ```exit``` Exectute a command that fails and exit without a parameter

## AUTHORS
Dinu MIRA : *[Github](https://github.com/EXTRADEEN)*
Simon RICHARD : *[Github](https://github.com/simonrichard-dev)*
