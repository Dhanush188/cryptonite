# touching files
The challenge asks us to create two new files: /tmp/pwn and /tmp/college, and run /challenge/run to get the flag

## My solve
**Flag:** `pwn.college{0AcmFrVjPWdWumwie2YELddJaP8.QXwMDO0wyNwQzNzEzW}`

First we cd(changed our directory) to tmp and created a new file 'pwn' by touching it and also created 'college' by touching it in a similar way.
We can view the newly created files by listing their directory.

```
hacker@commands~touching-files:~$ cd /tmp
hacker@commands~touching-files:/tmp$ ls
bin  hsperfdata_root  tmp.4mK6TfTSUV
hacker@commands~touching-files:/tmp$ touch pwn
hacker@commands~touching-files:/tmp$ ls
bin  hsperfdata_root  pwn  tmp.4mK6TfTSUV
hacker@commands~touching-files:/tmp$ touch college
hacker@commands~touching-files:/tmp$ ls
bin  college  hsperfdata_root  pwn  tmp.4mK6TfTSUV
hacker@commands~touching-files:/tmp$ /challenge/run
Success! Here is your flag:
pwn.college{0AcmFrVjPWdWumwie2YELddJaP8.QXwMDO0wyNwQzNzEzW}
```

## What I learned
You can create a new, blank file by touching it with the touch command.

## References 
pwn.college
