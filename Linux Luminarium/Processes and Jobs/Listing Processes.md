Learnt ps command and its different modes combined different arguments 
```bash
Connected!
hacker@processes~listing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.1  0.0   1056   640 ?        Ss   17:08   0:00 /sbin/docker-init -- /nix/var/nix/profiles/default/bi
root           7  0.0  0.0   5052  2560 ?        S    17:08   0:00 /run/dojo/bin/sleep 6h
root          68  0.0  0.0   4132  2560 ?        S    17:08   0:00 /challenge/8785-run-32135
root          72  0.0  0.0   2744  1280 ?        S    17:08   0:00 sleep 6h
hacker        73  0.1  0.0   5372  4160 pts/0    Ss   17:08   0:00 /run/dojo/bin/ssh-entrypoint
hacker        90  0.0  0.0   7868  3200 pts/0    R+   17:09   0:00 ps aux
hacker@processes~listing-processes:~$  /challenge/8785-run-32135
Yahaha, you found me! Here is your flag:
pwn.college{wWBZn468SSDen1CogBKACSJ5DMv.dhzM4QDL3MTN0czW}
```
