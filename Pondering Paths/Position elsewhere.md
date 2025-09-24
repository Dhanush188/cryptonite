# Position elsewhere
The challenge asks us to cd(change directory) to a directory(/usr/share/doc/fontconfig), which is obtained by executing '/challenge/run', because '/challenge/run lies in that directory.

## My solve
**Flag:** `pwn.college{URSfSWLw6e4N43mgVW6TTQVIYiD.QX3QTN0wyNwQzNzEzW}`

We first executed the /challenge/run program, but it lies in the /usr/share/doc/fontconfig directory. So we have to first cd(change directory) to the /usr/share/doc/fontconfig directory and then execute the /challenge/run program to obtain the flag.

```
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /usr/share/doc/fontconfig directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /usr/share/doc/fontconfig
hacker@paths~position-elsewhere:/usr/share/doc/fontconfig$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{URSfSWLw6e4N43mgVW6TTQVIYiD.QX3QTN0wyNwQzNzEzW}
```

## What I learned
We can navigate around directories by using the cd (change directory) command and passing a path to it as an argument.
We can use pwd command to verify if we are present in the required directory.
'~' in the prompt shows the current path that your shell is located at.

## References 
pwn.college
