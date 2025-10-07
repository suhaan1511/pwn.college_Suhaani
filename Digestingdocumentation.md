# Digesting Documentation

## Learning From Documentation

### Solve
**Flag:** pwn.college{wPz_-VzRi0XfLfSB0bnPz56ub1-.QX0ITO0wiN3EzNzEzW}

```bash 
hacker@man~learning-from-documentation:~$ /challenge/challenge --giveflag
Correct argument! Here is your flag:
pwn.college{wPz_-VzRi0XfLfSB0bnPz56ub1-.QX0ITO0wiN3EzNzEzW}
```
I invoked the program /challenge/challenge in order to get the flag. 

### New Learnings
Learned how to read documentation

### References
None


## Learning Complex Usage

### Solve
**Flag:** pwn.college{c5qHCbZqt3mSwxyI3PdcGHk3z9Z.QX1ITO0wiN3EzNzEzW}
```bash
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile /flag
Correct argument! Here is the /flag file:
pwn.college{c5qHCbZqt3mSwxyI3PdcGHk3z9Z.QX1ITO0wiN3EzNzEzW}
```
I used --printflag /flag arguments in /challenge/challenge to get the flag.

### New Learnings
I learned  about --printfile.


## Reading Manuals

### Solve
**Flag:**  pwn.college{8mhrgJx3sDuMN4zOT5-0TZ5ZwCe.QX0EDO0wiN3EzNzEzW}

```bash
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ /challenge/challenge --fortune
Keep cool, but don't freeze.
                -- Hellman's Mayonnaise
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ /challenge/challenge --version
I'm exactly the version I need to be!
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ /challenge/challenge mhrgxs NUM
Incorrect usage! Please read the challenge man page!
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ /challenge/challenge mhrgxs 834
Incorrect usage! Please read the challenge man page!
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ /challenge/challenge mhrgxs NUM 834
Incorrect usage! Please read the challenge man page!
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ /challenge/challenge --mhrgxs 834
```
I used the man comand to get the manual page for the challenge command, read arguments out of which --mhrgxs had a description regarding the flag, executed it and obtained the flag.

### New Learnings
I learned how to read manual pages and about the man command.


## Searching Manuals

### Solve
**Flag:** pwn.college{cSKimJ8Zn1gVfHjoEzgDhVwm4Tk.QX1EDO0wiN3EzNzEzW}

```bash
hacker@man~searching-manuals:~$ man challenge
gzip: stdout: Broken pipe
hacker@man~searching-manuals:~$ /challenge/challenge --yr
Initializing...
Correct usage! Your flag: pwn.college{cSKimJ8Zn1gVfHjoEzgDhVwm4Tk.QX1EDO0wiN3EzNzEzW}
hacker@man~searching-manuals:~$ ^C
```
I used man comand to get the manual page for the challenge command,
searched for flag using '/' and then navigated through the manual page using n till i obtained the flag.

### New Learnings
I learned to scroll man pages with the arrow keys (and PgUp/PgDn) and search with /. 
I learned to hit n to go to the next result and N to go to the previous result. 


## Searching for manuals

### Solve
**Flag:** pwn.college{AlwqWFj2PFWgR5942N-KiSNh_pf.QX2EDO0wiN3EzNzEzW}

```bash
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -k flag
dpkg-buildflags (1)  - returns build flags to use during package build
Dpkg::BuildFlags (3perl) - query build flags
fegetexceptflag (3)  - floating-point rounding and exception handling
fesetexceptflag (3)  - floating-point rounding and exception handling
i386 (8)             - change reported architecture in new program environmen...
ioctl_iflags (2)     - ioctl() operations for inode flags
linux32 (1)          - change reported architecture in new program environmen...
linux64 (1)          - change reported architecture in new program environmen...
lwqjgihpfw (1)       - print the flag!
pcap-config (1)      - write libpcap compiler and linker flags to standard ou...
security_compute_av_flags (3) - query the SELinux policy database in the kernel
security_compute_av_flags_raw (3) - query the SELinux policy database in the ...
set_matchpathcon_flags (3) - set flags controlling the operation of matchpath...
set_matchpathcon_invalidcon (3) - set flags controlling the operation of matc...
set_matchpathcon_printf (3) - set flags controlling the operation of matchpat...
setarch (1)          - change reported architecture in new program environmen...
setarch (8)          - change reported architecture in new program environmen...
x86_64 (8)           - change reported architecture in new program environmen...
hacker@man~searching-for-manuals:~$ man lwqjgihpfw
hacker@man~searching-for-manuals:~$ /challenge/challenge lwqjgi --259
Incorrect usage! Please read the hidden challenge man page!
hacker@man~searching-for-manuals:~$ /challenge/challenge --lwqjgi 259
Correct usage! Your flag: pwn.college{AlwqWFj2PFWgR5942N-KiSNh_pf.QX2EDO0wiN3EzNzEzW}
```
I used man man to get information about man pages and what commands to use to find them.
I used sources to find about the -k command and used it with 'challenge' manpage i want and opened the manpage with man command and obtained the flag .


### New Learnings
I learned about -k flag 


## Helpful Programs

### Solve
**Flag:** pwn.college{Qe3AkGkhRa0Kcgxv9ioU6KXX0Mo.QX3IDO0wiN3EzNzEzW}

```bash
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge --p
The secret value is: 309
hacker@man~helpful-programs:~$ /challenge/challenge -g 309
Correct usage! Your flag: pwn.college{Qe3AkGkhRa0Kcgxv9ioU6KXX0Mo.QX3IDO0wiN3EzNzEzW}
```
I used --help to get program then from the instructions used --p to get the secret value and used the secret value to get the flag.

### New Learnings
I learned about --help which i can use for reading a program's documentation without man pages.


## Help for Builtins

###Solve
**Flag:** pwn.college{YG45cqTjfFyW1LLzZzU3n1odCFL.QX0ETO0wiN3EzNzEzW}

```bash
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!
    
    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "YG45cqTj".
hacker@man~help-for-builtins:~$ --secret YG45cqTj
bash: --secret: command not found
hacker@man~help-for-builtins:~$ /challenge/challenge --secret YG45cqTj
bash: /challenge/challenge: No such file or directory
hacker@man~help-for-builtins:~$ challenge --secret YG45cqTj
Correct! Here is your flag!
pwn.college{YG45cqTjfFyW1LLzZzU3n1odCFL.QX0ETO0wiN3EzNzEzW}
```
I used builtin command help to get information regarding obtaining the flag and -secret argument to obtain the flag.

### New Learnings
I learned differences between how programs and shell builtin commands are executed and the information of builtin commaands.



