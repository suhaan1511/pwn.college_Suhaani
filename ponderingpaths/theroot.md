Challenge 1
## The Root

**Flag:**  pwn.college{4-3ZC5AcOAUXKnHOgCn5b1KbNK3.QX4cTO0wiN3EzNzEzW} 

### My Solve
hacker@pathsthe-root:$ /pwn BOOM!!! 

The filesystem starts at /.
Under that, there are a whole mess of other directories, configuration files, programs, and, most importantly, flags. 
In this level, I added a program right in /, called pwn, that will give the flag.
I launched a terminal and invoked the pwn program using its absolute path.

### New Learnings :
I learned that filesystem starts with / and that absolute path starts with root directory. (/) I can invoke a program by providing its path on the command line.

### References:
None
