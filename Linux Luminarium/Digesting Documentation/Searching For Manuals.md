```bash
hacker@man~searching-for-manuals:/challenge$ man -f /challenge/challenge
krcijnyfbq (1)       - print the flag!
hacker@man~searching-for-manuals:/challenge$ man krcijnyfbq

CHALLENGE(1)                  Challenge Commands                  CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --krcijn NUM
              print the flag if NUM is 735

AUTHOR
       Written by Zardus.

hacker@man~searching-for-manuals:/challenge$ /challenge/challenge        --krcijn NUM
Incorrect usage! Please read the challenge man page!
hacker@man~searching-for-manuals:/challenge$ /challenge/challenge        --krcijn 735
Correct usage! Your flag: pwn.college{kr7YcijnUSyVf3KP58bq9FsvmX9.dZTM4QDLzYTN0czW}
```
