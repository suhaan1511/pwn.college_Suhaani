Challenge 6
## Implicit relative paths, from /

**Flag:** pwn.college{40gWNI3_n3dCGVatZjyrs8PchKy.QX5QTN0wiN3EzNzEzW} 

### My solve
hacker@pathsimplicit-relative-paths-from-:$ cd / 
hacker@paths~implicit-relative-paths-from-:/$ challenge/run 
Correct!!! challenge/run is a relative path, invoked from the right directory! 

Here I ran the program using a relative path while having a current working directory of /. 

### New Learnings
I learned that relative path does not start at root (does not start with /). A relative path is interpreted relative to cwd.

### References
None
