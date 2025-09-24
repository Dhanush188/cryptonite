# explicit relative paths
The challenge is asking you to run the /challenge/run program using a relative path that includes '.' (the current directory reference).

## My solve
**Flag:** `pwn.college{UYGZ2hyx2qAoLy2KV8nN30BCJpT.QXwUTN0wyNwQzNzEzW}`

We have to first cd(change directory) to '/', to set it as the current working directory to be able to use relative path.
now to execute using relative path, execute ./challenge/run to get the flag. The '.' in the starting redirects to '/'.

```
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{UYGZ2hyx2qAoLy2KV8nN30BCJpT.QXwUTN0wyNwQzNzEzW}
```

## What I learned
The '..' refers to the parent directory.
The '.' refers to the directory you are currently in.
I learned using '.' in your relative paths.

## References 
pwn.college
