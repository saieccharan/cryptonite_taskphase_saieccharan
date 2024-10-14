Leant how to kill a processes
```bash
hacker@processes~killing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 17:15 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/default/bin/dojo-init /ru
root           7       1  0 17:15 ?        00:00:00 /run/dojo/bin/sleep 6h
root          71       1  0 17:15 ?        00:00:00 su -c /challenge/.launcher hacker
hacker        73      71  0 17:15 ?        00:00:00 /challenge/dont_run
hacker        74      73  0 17:15 ?        00:00:00 sleep 6h
hacker        75       0  0 17:15 pts/0    00:00:00 /run/dojo/bin/ssh-entrypoint
hacker        93      75  0 17:16 pts/0    00:00:00 ps -ef
hacker@processes~killing-processes:~$ kill 73
hacker@processes~killing-processes:~$  /challenge/run
Great job! Here is your payment:
pwn.college{AefRjdBoGWROrquzhYRe2S99uxl.dJDN4QDL3MTN0czW}
```
