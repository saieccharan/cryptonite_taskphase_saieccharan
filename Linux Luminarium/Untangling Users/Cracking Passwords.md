Learnt how to use John the Ripper tool and other useful info about where passwords will be stored and etc.
```bash
hacker@users~cracking-passwords:~$ cat /challenge/shadow-leak
root:*:19873:0:99999:7:::
daemon:*:19873:0:99999:7:::
bin:*:19873:0:99999:7:::
sys:*:19873:0:99999:7:::
sync:*:19873:0:99999:7:::
games:*:19873:0:99999:7:::
man:*:19873:0:99999:7:::
lp:*:19873:0:99999:7:::
mail:*:19873:0:99999:7:::
news:*:19873:0:99999:7:::
uucp:*:19873:0:99999:7:::
proxy:*:19873:0:99999:7:::
www-data:*:19873:0:99999:7:::
backup:*:19873:0:99999:7:::
list:*:19873:0:99999:7:::
irc:*:19873:0:99999:7:::
gnats:*:19873:0:99999:7:::
nobody:*:19873:0:99999:7:::
_apt:*:19873:0:99999:7:::
hacker::20000:0:99999:7:::
zardus:$6$ggMeIURtK6gu8sCo$C4yj4F6ymWJakTulPUJBfFTgDAbjrcem5S.kp1KJ9ONFs2TxKETap99Sij5rELYOSeVLaVkCGu5cmKvGPM4E6/:20010:0:99999:7:::
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
aardvark         (zardus)
1g 0:00:00:24 100% 2/3 0.04055g/s 236.1p/s 236.1c/s 236.1C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ john --show /challenge/shadow-leak
hacker:NO PASSWORD:20000:0:99999:7:::
zardus:aardvark:20010:0:99999:7:::

2 password hashes cracked, 0 left
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{kEQ8Ix6i967aUVLcEYoVi_P7hQW.ddTN0UDL3MTN0czW}
```
