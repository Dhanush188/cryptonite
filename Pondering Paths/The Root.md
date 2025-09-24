# The Root
We have to invoke a program which contains the flag, by providing its path on the command line.
## My solve
**Flag:** `pwn.college{UXQ7fbllMJ3-uvkrH6aUrHcXHI2.QX4cTO0wyNwQzNzEzW}`

We have to first start with '/',which is the root directory which contains different programs and files , in this case it is the 'pwn' program.
after invoking the 'pwn' program in the root directory,we will get the required flag.

```
hacker@paths~the-root:~$ /pwn
BOOM!!!
Here is your flag:
pwn.college{UXQ7fbllMJ3-uvkrH6aUrHcXHI2.QX4cTO0wyNwQzNzEzW}
```

## What I learned
'/' is the root directory.
The style of path that starts with the root directory, is referred to as an "absolute path".

## References 
pwn.college
