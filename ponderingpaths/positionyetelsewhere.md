Challenge 5
## Position yet elsewhere

**Flag:** pwn.college{c7jJn1dpnjn0zz5O030VhGctwn6.QX4QTN0wiN3EzNzEzW} 

### My Solve
hacker@pathsposition-yet-elsewhere:$ cd /challenge 
hacker@pathsposition-yet-elsewhere:/challenge$ /challenge/run Incorrect... You are not currently in the /usr/aarch64-linux-gnu/include/gnu directory. Please use the cd utility to change directory appropriately.
hacker@pathsposition-yet-elsewhere:/challenge$ cd /usr/aarch64-linux-gnu/include/gnu hacker@paths~position-yet-elsewhere:/usr/aarch64-linux-gnu/include/gnu$ /challenge/run Correct!!! /challenge/run is an absolute path, invoked from the right directory!

Here I executed the /challenge/run program from a specific path. I cd to the directory.

### New Learnings
I learned that we can navigate around directories by using change directory (cd) command.

### References
None
