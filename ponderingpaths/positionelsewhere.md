Challenge 4
## Position elsewhere

**Flag:** pwn.college{kq9z--dKCjvDO_3Zj662ORQpNZz.QX3QTN0wiN3EzNzEzW} 

### My Solve
hacker@pathsposition-elsewhere:$ cd /challenge 
hacker@pathsposition-elsewhere:/challenge$ /challenge/run Incorrect... You are not currently in the /proc/145 directory. Please use the cd utility to change directory appropriately.
hacker@pathsposition-elsewhere:/challenge$ cd /proc/145 
hacker@paths~position-elsewhere:/proc/145$ /challenge/run Correct!!! /challenge/run is an absolute path, invoked from the right directory!

Here I executed the /challenge/run program from a specific path.

### New Learnings
I learned that we can navigate around directories by using change directory (cd) command.

### References
None
