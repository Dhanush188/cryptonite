# implicit relative paths
The challenge is asking us to run the program /challenge/run using a relative path, while having a current working directory of /.

## My solve
**Flag:** `pwn.college{gpaOM1k70kUZ9c7aPJlDTWCpNTL.QX5QTN0wyNwQzNzEzW}`

We have to first cd(change directory) to '/', because they asked us to have '/' as the current working directory.
and then we can execute the program challenge/run directly without using '/', because we are following relative path.

```
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{gpaOM1k70kUZ9c7aPJlDTWCpNTL.QX5QTN0wyNwQzNzEzW}
```

## What I learned
If you put in absolute paths everywhere, then it really doesn't matter what directory you are in.
The current working directory does matter for relative paths.
A relative path is any path that does not start at root.
A relative path is interpreted relative to your current working directory.
The '..' refers to the parent directory.
The '.' refers to the directory you are currently in.

## References 
pwn.college
