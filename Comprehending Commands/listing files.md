# listing files
The challenge asks us to list the files in /challenge to find /challenge/run which has been named randomly.

## My solve
**Flag:** `pwn.college{4g4V86MbSQIvT82gZO34GhWiebP.QX4IDO0wyNwQzNzEzW}`

First we must list all the files in /challenge, and then we obtain a renamed file. And we can obtain the flag by simply reading it.

```
hacker@commands~listing-files:~$ ls /challenge
26193-renamed-run-1086  DESCRIPTION.md
hacker@commands~listing-files:~$ ls /challenge/^C
hacker@commands~listing-files:~$ ls /challenge/26193-renamed-run-1086
/challenge/26193-renamed-run-1086
hacker@commands~listing-files:~$ /challenge/26193-renamed-run-1086
Yahaha, you found me! Here is your flag:
pwn.college{4g4V86MbSQIvT82gZO34GhWiebP.QX4IDO0wyNwQzNzEzW}
```

## What I learned
ls will list files in all the directories provided to it as arguments.

## References 
pwn.college
