# cat: not the pet, but the command!
The challenge is just asking us to read the 'flag' file in the home directory.

## My solve
**Flag:** `pwn.college{wdKxPbRZr6OuhuZH3un7YSTfj0X.QXxcTN0wyNwQzNzEzW}`

I just used the 'cat' command to read the 'flag' file present in the home directory.

```
hacker@commands~cat-not-the-pet-but-the-command:~$ cat flag
pwn.college{wdKxPbRZr6OuhuZH3un7YSTfj0X.QXxcTN0wyNwQzNzEzW}
```

## What I learned
 cat is most often used for reading out files.
 cat will concatenate (hence the name) multiple files if provided multiple arguments. 
 if you give no arguments at all, cat will read from the terminal input and output it.

## References 
pwn.college
