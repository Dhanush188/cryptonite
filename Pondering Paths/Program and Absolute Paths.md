# Program and Absolute Paths
This challenge asks you to invoke the program 'run', which is in the 'challenge' directory to obtain the flag.

## My solve
**Flag:** `pwn.college{g44e6ba3IZ6itsCFriUispqBQkL.QX1QTN0wyNwQzNzEzW}`

We first enter the root directory '/', which contains the 'challenge' directory, which then contains the program 'run'.
Now this program 'run' contains the required flag.

```
hacker@paths~program-and-absolute-paths:~$ /challenge/run
Correct!!!
/challenge/run is an absolute path! Here is your flag:
pwn.college{g44e6ba3IZ6itsCFriUispqBQkL.QX1QTN0wyNwQzNzEzW}
```

## What I learned
The root directory '/' further may contain many directories, programs and files.
The challenges in the pwn.college are in the 'challenge' directory. to access them :- /challenge.

## References 
pwn.college
