# Position thy self
The challenge asks us to cd(change directory) to a directory(/sys/kernel), which is obtained by executing '/challenge/run', 
because '/challenge/run lies in that directory.

## My solve
**Flag:** `pwn.college{gPpQGbihHEgQ0eniRZMsZIF6caI.QX2QTN0wyNwQzNzEzW}`

We first executed the /challenge/run program, but it lies in the /sys/kernel directory. So we have to first cd(change directory) to the /sys/kernel directory
(confirm using pwd command) and then execute the /challenge/run program to obtain the flag.

```
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /sys/kernel directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd /sys/kernel
hacker@paths~position-thy-self:/sys/kernel$ pwd
/sys/kernel
hacker@paths~position-thy-self:/sys/kernel$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{gPpQGbihHEgQ0eniRZMsZIF6caI.QX2QTN0wyNwQzNzEzW}
```

## What I learned
We can navigate around directories by using the cd (change directory) command and passing a path to it as an argument.
We can use pwd command to verify if we are present in the required directory.
'~' in the prompt shows the current path that your shell is located at.

## References 
pen.college
