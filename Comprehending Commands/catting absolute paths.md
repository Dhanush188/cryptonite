# catting absolute paths
The challenge asks us to read the 'flag' file at it's absolute path.

## My solve
**Flag:** `pwn.college{spOEXIwEcw1yLOTrJ7O7kqC99pr.QX5ETO0wyNwQzNzEzW}`

We just executed cat /flag instead of cat flag, because in this challenge  the 'flag' file is not copied into the home directory.
So we should read it with cat at its absolute path.

```
hacker@commands~catting-absolute-paths:~$ cat /flag
pwn.college{spOEXIwEcw1yLOTrJ7O7kqC99pr.QX5ETO0wyNwQzNzEzW}
```

## What I learned
We can specify cat's arguments as absolute paths.
/flag is where the flag always lives in pwn.college.

## References 
pwn.college
