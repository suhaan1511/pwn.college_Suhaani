Challenge 5
## Comparing files

### My Solve
**Flag:** pwn.college{Ip8LLT88fB1Bt0siZujC3vxs8lB.01MwMDOxwiN3EzNzEzW}
hacker@commands~comparing-files:~$ cat /challenge/decoys_only.txt
hacker@commands~comparing-files:~$ cat /challenge/decoys_and_real.txt
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
63a64
I used the diff command to find the difference between the files challenge/decoys_only.txt and /challenge/decoys_and_real.txt
As when looking for changes between similar files, eyeballing them might not be the most efficient approach.

### New Learnings
I learnt that diff compares two files line by line and shows you exactly what's different between them. 
