Challenge 7
## Explicit relative paths, from /

### My Solve
**Flag:** pwn.college{YPXo7pUH_mpYf281lCVBTaBLsPO.QXwUTN0wiN3EzNzEzW}

/challenge/run is a relative path, invoked from the right directory! 
hacker@pathsexplicit-relative-paths-from-:$ cd / hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!! ./challenge/run is a relative path, invoked from the right directory!

Here I ran /challenge/run using . in the relative paths.

### New Learnings
I explored more explicit relative paths. And that the following relative paths are also all identical to each other: 
challenge ./challenge ./././challenge challenge/.

### References
None
