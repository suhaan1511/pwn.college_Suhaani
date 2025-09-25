MODULE NAME
Pondering Paths

Challenge 1
The Root
*Flag:* pwn.college{4-3ZC5AcOAUXKnHOgCn5b1KbNK3.QX4cTO0wiN3EzNzEzW}
hacker@paths~the-root:~$ /pwn
BOOM!!!
The filesystem starts at /. Under that, there are a whole mess of other directories, configuration files, programs, and, most importantly, flags. 
In this level, I added a program right in /, called pwn, that will give the flag. 
I launched a terminal and invoked the pwn program using its absolute path.
New Learnings: I learned that filesystem starts with / and that absolute path starts with root directory. (/) I can invoke a program by providing its path on the command line.

Challenge 2 
Program and absolute paths
*Flag:* pwn.college{IXP_lDCvYTbwMwOSzvnf1gC_5Yg.QX1QTN0wiN3EzNzEzW}
hacker@paths~program-and-absolute-paths:~$ /challenge/run
Correct!!!
/challenge/run is an absolute path!
The challenges in pwn.college are in the challenge directory and the challenge directory is, in turn, right in the root directory (/). 
The path to the challenge directory is, thus, /challenge. The name of the challenge program in this level is run, and it lives in the /challenge directory. 
Thus, the path to the run challenge program is /challenge/run.
I executed it by invoking its absolute path. 
New Learnings: I learned that challenges are in the challenge directory and the challenge directory is, in turn, right in the root directory (/). 
I learned that run is the name of the challenge program and the path is /challenge/run.

Challenge 3 
Position thy self 
*Flag:* pwn.college{QhhPiCsfdVMRmsjZjmQBbKX1aBH.QX2QTN0wiN3EzNzEzW}
hacker@paths~position-thy-self:/$ cd /challenge
hacker@paths~position-thy-self:/challenge$ /challenge/run
Incorrect...
You are not currently in the /usr/share/zoneinfo/posix/Asia directory.
Please use the cd utility to change directory appropriately.
hacker@paths~position-thy-self:/challenge$ cd /usr/share/zoneinfo/posix/Asia
hacker@paths~position-thy-self:/usr/share/zoneinfo/posix/Asia$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
The Linux filesystem has tons of directories with tons of files.
I can navigate around directories by using the cd (change directory) command and passing a path to it as an argument.
Here I executed the /challenge/run program from a specific path. 
New Learnings: I learned that we can navigate around directories by using change directory (cd) command and executed programs from a specific path.

Challenge 4
Position elsewhere
*Flag:* pwn.college{kq9z--dKCjvDO_3Zj662ORQpNZz.QX3QTN0wiN3EzNzEzW}
hacker@paths~position-elsewhere:~$ cd /challenge
hacker@paths~position-elsewhere:/challenge$ /challenge/run
Incorrect...
You are not currently in the /proc/145 directory.
Please use the cd utility to change directory appropriately.
hacker@paths~position-elsewhere:/challenge$ cd /proc/145
hacker@paths~position-elsewhere:/proc/145$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here I executed the /challenge/run program from a specific path. 
New Learnings: I learned that we can navigate around directories by using change directory (cd) command.

Challenge 5
Position yet elsewhere
*Flag:* pwn.college{c7jJn1dpnjn0zz5O030VhGctwn6.QX4QTN0wiN3EzNzEzW}
hacker@paths~position-yet-elsewhere:~$ cd /challenge
hacker@paths~position-yet-elsewhere:/challenge$ /challenge/run
Incorrect...
You are not currently in the /usr/aarch64-linux-gnu/include/gnu directory.
Please use the cd utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:/challenge$ cd /usr/aarch64-linux-gnu/include/gnu
hacker@paths~position-yet-elsewhere:/usr/aarch64-linux-gnu/include/gnu$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{c7jJn1dpnjn0zz5O030VhGctwn6.QX4QTN0wiN3EzNzEzW}
Here I executed the /challenge/run program from a specific path. I cd to the directory.
New Learnings: I learned that we can navigate around directories by using change directory (cd) command.

Challenge 6 
implicit relative paths, from /
*Flag:* pwn.college{40gWNI3_n3dCGVatZjyrs8PchKy.QX5QTN0wiN3EzNzEzW}
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{40gWNI3_n3dCGVatZjyrs8PchKy.QX5QTN0wiN3EzNzEzW}
Here I ran the program using a relative path while having a current working directory of /. 
New Learnings: I learned that relative path does not start at root (does not start with /). A relative path is interpreted relative to cwd.

Challenge 7 
explicit relative paths, from /
*Flag:* ./challenge/run is a relative path, invoked from the right directory!
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{YPXo7pUH_mpYf281lCVBTaBLsPO.QXwUTN0wiN3EzNzEzW}
Here I ran /challenge/run using . in the relative paths.
New Learnings: I explored more explicit relative paths. And that the following relative paths are also all identical to each other:
challenge
./challenge
./././challenge
challenge/.

Challenge 8
Implicit relative path
*Flag:* pwn.college{A5kwWiN1tFl58CODqyl1Ggqk7QC.QXxUTN0wiN3EzNzEzW}
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{A5kwWiN1tFl58CODqyl1Ggqk7QC.QXxUTN0wiN3EzNzEzW}
Here I explicitly used relative paths to launch run. (using .) 
New Learnings: Linux explicitly avoids automatically looking in the current directory when you provide a "naked" path.

Challenge 9
home sweet home
*Flag:* pwn.college{45q0cpOhdQWFJUATwTuvI30nOA1.QXzMDO0wiN3EzNzEzW}
hacker@paths~home-sweet-home:~$ /challenge/run ~/a
Writing the file to /home/hacker/a!
... and reading it back to you:
pwn.college{45q0cpOhdQWFJUATwTuvI30nOA1.QXzMDO0wiN3EzNzEzW}
