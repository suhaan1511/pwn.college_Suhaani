Challenge
## Hidden files

### My Solve
**Flag:** pwn.college{o8xbOSB0JH04r2mTHc4a4E1_rP-.QXwUDO0wiN3EzNzEzW}
hacker@commands~hidden-files:~$ ls -a
.  ..  .bash_history  .college  .config  a  college  pwn
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv           bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-1017172598766  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-1017172598766

### New Learnings
I learned taht Linux has a convention where files that start with a . don't show up by default in ls and in a few other contexts. To view them with ls, you need to invoke ls with the -a flag.
