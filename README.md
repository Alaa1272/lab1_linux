1. Install Ubuntu [Dual-boot, VM, Multipass]
2. What is the difference between cat and more command?
3. What is the difference between rm and rmdir using man?
4. Create the following hierarchy under your home directory:

a. Remove dir11 in one-step. What did you notice? And how did you overcome that?
b. Then remove dir12 using rmdir –p command. State what happened to the
hierarchy (Note: you are in your home directory).
![Screenshot (18)](https://github.com/user-attachments/assets/0c2f4da5-2ca9-40f2-9cc9-3041a0ab7d12)
c. The output of the command pwd was /home/user. Write the absolute
and relative path for the file mycv

ubuntu@endorsed-anoa:~$ pwd
/home/ubuntu
ubuntu@endorsed-anoa:~$ readlink -f mycv
/home/ubuntu/mycv


5. Copy the /etc/passwd file to your home directory making its name is mypasswd.
6. Rename this new file to be oldpasswd.
   
ubuntu@endorsed-anoa:~$ cp /etc/passwd ~/mypasswd
ubuntu@endorsed-anoa:~$ mv mypasswd oldpasswd
 
8. You are in /usr/bin, list four ways to go to your home directory

ubuntu@endorsed-anoa:/$ cd bin
ubuntu@endorsed-anoa:/bin$ cd ..
ubuntu@endorsed-anoa:/$ cd home


ubuntu@endorsed-anoa:/home$ cd ..
ubuntu@endorsed-anoa:/$ cd bin

9. List Linux commands in /usr/bin that start with letter w

ubuntu@endorsed-anoa:/bin$ ls |grep ^[w]
w
wall
watch
watchgnupg
wc
wdctl
wget
whatis
whereis
which
which.debianutils
whiptail
who
whoami
wifi-status
write

10. Display the first 4 lines of /etc/passwd

ubuntu@endorsed-anoa:/$ head -4 etc/passwd

my name is alaa
smklwqmdk
odmkekdle
ed,l;e,,e

10.Display the last 7 lines of /etc/passwd

ubuntu@endorsed-anoa:/$ tail -7 etc/passwd

odmkekdle
ed,l;e,,e
jndkne
klemdkme
dkmkedk
kdekl
kwemdkme


11.Display the man pages of passwd the command and the file sequentially in one command.
12.Display the man page of the passwd file.

ubuntu@endorsed-anoa:~$ man 1 passwd ; man 5 passwd
ubuntu@endorsed-anoa:~$ man 5 passwd
![Screenshot (19)](https://github.com/user-attachments/assets/ad045caf-c472-4b18-8fcc-899f625a84c1)

13.Display a list of all the commands that contain the keyword passwd in their man page.

ubuntu@endorsed-anoa:~$ man -k etc/passwd
pam_localuser (8)    - require users to be listed in /etc/passwd
update-passwd (8)    - safely update /etc/passwd, /etc/shadow and /etc/group

14. Using vi write your CV in the file mycv. Your CV should include your name, age, school,
college, experience,...

ubuntu@endorsed-anoa:~$ sudo vi mycv
![Screenshot (22)](https://github.com/user-attachments/assets/2081a303-b68b-4b96-a2ba-0aa4b9a53636)


16. Open mycv file using vi command then: Without using arrows state how to:
a. Move the cursor down one line at time.
b. Move the cursor up one line at time.

ubuntu@endorsed-anoa:~$ vi mycv 
using j to down 
and k to up

c. Search for word age

ubuntu@endorsed-anoa:~$ vi mycv 
/age

![Screenshot (23)](https://github.com/user-attachments/assets/b9ba1a82-1bdd-4a7f-8b0d-63f5780d0788)

d. Step to line 5 (assuming that you are in line 1 and file is more than 5 lines).

5G

e. Delete the line you are on and line 5.

![Screenshot (24)](https://github.com/user-attachments/assets/1f39a267-786a-4b81-9dc0-1be75b74b934)

f. How to step to the end of line and change to writing mode in one-step.
18. st the available shells in your system.

ubuntu@endorsed-anoa:/$ cat /etc/shells

# /etc/shells: valid login shells
/bin/sh
/usr/bin/sh
/bin/bash
/usr/bin/bash
/bin/rbash
/usr/bin/rbash
/usr/bin/dash
/usr/bin/screen  
/usr/bin/tmux
