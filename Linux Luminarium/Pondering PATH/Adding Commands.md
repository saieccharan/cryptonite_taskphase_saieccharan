Learnt more about PATH and this was one hell of a tricky challenge.
```bash
hacker@path~adding-commands:~$ pwd
/home/hacker
hacker@path~adding-commands:~$ nano /home/hacker/win
hacker@path~adding-commands:~$ ls -l win
-rwxr-xr-x 1 hacker hacker 17 Oct 12 04:53 win
hacker@path~adding-commands:~$ export PATH=/home/hacker:$PATH
hacker@path~adding-commands:~$ echo $PATH
/home/hacker:/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
pwn.college{8BBSnItY8vxFUgCdBNBAmiAs-Mn.dZzNyUDL3MTN0czW}
```
