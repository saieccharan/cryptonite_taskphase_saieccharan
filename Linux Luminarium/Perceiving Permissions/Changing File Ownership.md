Learnt what ls-l and chown does and how only root user can change the ownership(will be learning how to exploit it in the latter modules)
```bash
hacker@permissions~changing-file-ownership:~$ ls -l /flag
-r-------- 1 root root 58 Oct 14 17:55 /flag
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ ls -l /flag
-r-------- 1 hacker root 58 Oct 14 17:55 /flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{sFmLr-W85U2k_udFMzP3-D8e0v1.dFTM2QDL3MTN0czW}
hacker@permissions~changing-file-ownership:~$ pwn.college{sFmLr-W85U2k_udFMzP3-D8e0v1.dFTM2QDL3MTN0czW}
```
