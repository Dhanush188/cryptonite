# more catting practice
The challenge asks us to read the 'flag' file in some crazy directcory at it's absolute path.

## My solve
**Flag:** `pwn.college{gqp8Nen4jZC6JKwiP0AcU1JEdm_.QXwITO0wyNwQzNzEzW}`

Here, we are not allowed to use cd(vhange directory), so no cat flag.
So, we have to retrieve the flag by absolute path from /usr/local/man/flag.

```
hacker@commands~more-catting-practice:~$ cat /usr/local/man/flag
pwn.college{gqp8Nen4jZC6JKwiP0AcU1JEdm_.QXwITO0wyNwQzNzEzW}
```

## What I learned
We can retrieve the flag by absolute path without using cd(change directory).

## References 
pwn.college
