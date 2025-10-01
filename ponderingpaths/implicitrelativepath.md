Challenge 8
## Implicit relative path

### My solve
**Flag:** pwn.college{A5kwWiN1tFl58CODqyl1Ggqk7QC.QXxUTN0wiN3EzNzEzW} 

hacker@pathsimplicit-relative-path:$ cd /challenge 
hacker@paths~implicit-relative-path:/challenge$ ./run Correct!!! ./run is a relative path, invoked from the right directory! 

Here I explicitly used relative paths to launch run. (using .) 
 
### New Learnings
Linux explicitly avoids automatically looking in the current directory when you provide a "naked" path.

### References
None

 
