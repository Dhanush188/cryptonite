# home sweet home 
The challenge asks us to run /challenge/run with a single argument that is less than 3 characters before shell expansion, and which expands to an absolute path inside your home.

## My solve
**Flag:** `pwn.college{osru30-SOr9v9R3bdNU_IADuf5T.QXzMDO0wyNwQzNzEzW}`

We just specified our path as an argument to /challenge/run as : hacker@dojo:~$ /challenge/run ~/x  . Here ~/x expands to /home/hacker/x.
```
hacker@paths~home-sweet-home:~$ /challenge/run ~/x
Writing the file to /home/hacker/x!
... and reading it back to you:
pwn.college{osru30-SOr9v9R3bdNU_IADuf5T.QXzMDO0wyNwQzNzEzW}
```

## What I learned
the expansion of ~ is an absolute path, and only the leading ~ is expanded. This means, for example, that ~/~ will be expanded to /home/hacker/~ rather than /home/hacker/home/hacker.
cd will use your home directory as the default destination.

## References 
pwn.college
