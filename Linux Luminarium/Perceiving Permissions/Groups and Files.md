Learnt what groups are and the command chgrp
```bash
hacker@permissions~groups-and-files:~$ ls -l /flag
-r--r----- 1 root root 58 Oct 14 18:06 /flag
hacker@permissions~groups-and-files:~$ chgrp hacker /flag
hacker@permissions~groups-and-files:~$ cat /flag
pwn.college{wF4_ZVG_OUiBAXfCV5azorTvOoy.dFzNyUDL3MTN0czW}
```
