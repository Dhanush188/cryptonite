# implicit relative path 
This challenge asks us to invoke /challenge/run with the using relative path with the use of '.' .

## My solve
**Flag:** `pwn.college{Ef1SxUqGInRHVNybkWkWj52mtxD.QXxUTN0wyNwQzNzEzW}`

First we cd(change directory) to the /challenge directory and then we use relative path to launch 'run'. But if Linux searched the current directory for programs every time you entered a naked path, you could accidentally execute programs in your current directory that happened to have the same names as core system utilities,
so the way to do this is to tell Linux that you explicitly want to execute a program in the current directory, using '.' . so we have executed ./run 
instead of just run.

```
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{Ef1SxUqGInRHVNybkWkWj52mtxD.QXxUTN0wyNwQzNzEzW}
```

## What I learned
Linux explicitly avoids automatically looking in the current directory when you provide a "naked" path.
if Linux searched the current directory for programs every time you entered a naked path, you could accidentally execute programs in your current directory that happened to have the same names as core system utilities,As a result, the above commands will yield the following error: bash: run: command not found.
The way to do this is to tell Linux that you explicitly want to execute a program in the current directory, using '.' .

## References 
pwn.college
