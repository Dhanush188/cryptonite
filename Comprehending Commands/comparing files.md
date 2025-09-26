# comparing files
The challenge asks to compare two files and find the difference between them.

## My solve
**Flag:** `pwn.college{YmaJNjTTeYnY9wOfubIWlWIR-O5.01MwMDOxwyNwQzNzEzW}`

here, we just dfound the difference between two files /challenge/decoys_only.txt and /challenge/decoys_and_real.txt.
And the difference here is that the 2nd file contains one extra real flag. The computer denoted it by 37a38, which means
"after line 37 of file1, add line 38 of file2"

```
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
37a38
> pwn.college{YmaJNjTTeYnY9wOfubIWlWIR-O5.01MwMDOxwyNwQzNzEzW}
```

## What I learned
diff compares two files line by line and shows you exactly what's different between them.
1a2 means "after line 1 of file1, add line 2 of file2".

## References 
pwn.college
