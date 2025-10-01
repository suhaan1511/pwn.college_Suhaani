Challenge 3
## Position thy self

**Flag:** pwn.college{QhhPiCsfdVMRmsjZjmQBbKX1aBH.QX2QTN0wiN3EzNzEzW} 

### My Solve
hacker@pathsposition-thy-self:/$ cd /challenge 
hacker@pathsposition-thy-self:/challenge$ /challenge/run 
Incorrect... You are not currently in the /usr/share/zoneinfo/posix/Asia directory. Please use the cd utility to change directory appropriately. 
hacker@pathsposition-thy-self:/challenge$ cd /usr/share/zoneinfo/posix/Asia 
hacker@pathsposition-thy-self:/usr/share/zoneinfo/posix/Asia$ /challenge/run 
Correct!!! /challenge/run is an absolute path, invoked from the right directory!

The Linux filesystem has tons of directories with tons of files. 
I can navigate around directories by using the cd (change directory) command and passing a path to it as an argument.
Here I executed the /challenge/run program from a specific path.

### New Learnings
I learned that we can navigate around directories by using change directory (cd) command and executed programs from a specific path.

### References
None
