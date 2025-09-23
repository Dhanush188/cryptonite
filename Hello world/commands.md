# Intro to Commands
the challenge asks us to invoke the 'Hello' command in the shell.

## My solve
**Flag:** `pwn.college{AwKyiVu1Gl6nBEXjl3KrmKqD169.QX3YjM1wyNwQzNzEzW}`

First we execute the 'whoami' command in the terminal, which simply prints the username to the terminal
In a similar way, we can use the 'hello' command to obtain the flag.

```
hacker@hello~intro-to-commands:~$ whoami
hacker
hacker@hello~intro-to-commands:~$ hello
Success! Here is your flag:
pwn.college{AwKyiVu1Gl6nBEXjl3KrmKqD169.QX3YjM1wyNwQzNzEzW}
```

## What I learned
The 'whoami' command prints the username to the terminal
Linux commands are case sensitive, hello is different from Hello.

## References 
pwn.college
