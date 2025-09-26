# grepping for a needle in a haystack
The challenge asks us to use the 'grep' command instead of 'cat' because the files to read are too big.

## My solve
**Flag:** `pwn.college{QmR9wZHtRxXaaCodN-XngNwFHJL.QX3EDO0wyNwQzNzEzW}`

In this challenge we just used the grep command intead of the cat command because the files to be read are too big.
they have put a hundred thousand lines of text into the /challenge/data.txt file. So, we just need to grep it for the flag and it has also been mentioned that the flag always starts with the text pwn.college.

```
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep pwn.college /challenge/data.txt
pwn.college{QmR9wZHtRxXaaCodN-XngNwFHJL.QX3EDO0wyNwQzNzEzW}
```

## What I learned
We can grep the files instead of catting them if they are too big.

## References 
pwn.college
