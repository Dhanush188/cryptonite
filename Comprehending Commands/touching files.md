# Challenge Name
The challenge asks us to create two new files: /tmp/pwn and /tmp/college, and run /challenge/run to get the flag

## My solve
**Flag:** `pwn.college{0AcmFrVjPWdWumwie2YELddJaP8.QXwMDO0wyNwQzNzEzW}`

type in your solve and your thought process behind solving the challenge. Include as much as info as possible. Use triple ticks for bash.

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
explain what you learned

## References 
pwn.college
