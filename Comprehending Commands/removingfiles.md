Challenge 8
## Removing files

### My Solve
**Flag:** pwn.college{MAmIn9RVbisPBvvMq-dzaUsihmQ.QX2kDM1wiN3EzNzEzW}

hacker@commands~removing-files:~$ touch delete_me
hacker@commands~removing-files:~$ ls
a  college  delete_me  pwn
hacker@commands~removing-files:~$ rm delete_me
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. 

I created a "delete_me' file using the touch command then used ls command to list the files.
After that, I deleted this file and checked for it using /challenge/check.

### New Learnings
I learned that I can remove files with the rm command.

