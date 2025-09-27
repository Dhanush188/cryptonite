# moving files
The challenge asks us to move the /flag file into /tmp/hack-the-planet.

## My solve
**Flag:** `pwn.college{EJfi5ifS8CeNVB1z1qrzO8vI2Z4.0VOxEzNxwyNwQzNzEzW}`

Here, we have moved the /flag file into /tmp/hack-the-planet using the 'mv' command and the we have run the  /challenge/check command to obtain the flag.
```
hacker@commands~moving-files:~$ mv /flag /tmp/hack-the-planet
Correct! Performing 'mv /flag /tmp/hack-the-planet'.
hacker@commands~moving-files:~$ /challenge/check
Congrats! You successfully moved the flag to /tmp/hack-the-planet! Here it is:
pwn.college{EJfi5ifS8CeNVB1z1qrzO8vI2Z4.0VOxEzNxwyNwQzNzEzW}
```

## What I learned
We can move files around with the 'mv' command. 

## References 
pwn.college
