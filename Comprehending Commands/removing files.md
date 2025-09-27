# removing files
The challenge asks us to remove the 'delete_me' file in the home directory then run /challenge/check,
which will make sure we've deleted it and then give us the flag.

## My solve
**Flag:** `pwn.college{8qt5mi-vT7gAABD9HLWBN45QoQt.QX2kDM1wyNwQzNzEzW}`

First we listed out all the files present in the home directory and found out the 'delete_me file' , which was to be removed using the rm command and we did the same
we later listed the the files in the home directory again and this time that file was not there beacause we have deleted it. Now, we have to run the /challenge/check
command to obtain the flag.

```
hacker@commands~removing-files:~$ ls
delete_me  x
hacker@commands~removing-files:~$ rm delete_me
hacker@commands~removing-files:~$ ls
x
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{8qt5mi-vT7gAABD9HLWBN45QoQt.QX2kDM1wyNwQzNzEzW}
```

## What I learned
In Linux, you can remove files with the 'rm' command.

## References 
pwn.college
