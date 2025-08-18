# Lab 1
#  What is the difference between cat and more command?
  cat - concatenate files and print on the standard output view enter file at once 
 
 more - display the contents of a file in a terminal view files in parts .

  ## What is the difference between rm and rmdir using man? 

  rm - remove files or directories
  rmdir - remove empty directories 
 ## 3-Create the following hierarchy under your home directory: 
 ## dir1
 ## dir11
 ## docs
 ## dir12
 ## mycv
 ## file1

   mkdir dir1 ,cd dir1
   mkdir dir11 , mkdir dir12 
   cd dir11 , touch file1
   cd .. ,cd ..
  
   tree dir1
dir1
├── dir11
│   └── file1
└── dir12
 
  mkdir docs ,cd docs
    touch mycv ,cd ..
 
   ls
   dir1  docs
  
   ls dir1 
dir11  dir12
 ls dir1/dir12
 ls dir1/dir11
file1
ls docs
mycv 
tree docs
docs
└── mycv
![Question2](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-07-31%2023-08-39.png)

## Remove dir11 in one-step. What did you notice? And how did you overcome that? 
    rm -r dir1/dir11  
    ![Question1](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-07-31%2023-08-06.png) 

 ## then remove dir12 using rmdir –p command. State what happened to the
 ## hierarchy (Note: you are in your home directory ). 
 rmdir -p  dir1/dir12
will remove dir12 and dir1 because dir1 
 -p, --parents 
   remove DIRECTORY and its ancestors; e.g., 'rmdir -p a/b' is sim‐ilar to 'rmdir a/b a'  
  ## The output of the command pwd was /home/user. Write the absolute and relative path for the file mycv 
  absolute  path   /home/heba/docs/mycv
 relative path    docs/mycv
              
  ## Copy the /etc/passwd file to your home directory making its name is mypasswd
  cp /etc/passwd ~/mypasswd 
  ##  Rename this new file to be oldpasswd. 
    mv mypasswd oldpasswd 
 ## You are in /usr/bin, list four ways to go to your home directory 

 1.cd
pwd
/home/heba
 cd /usr/bin/   -----> cd -
2. cd ~ 
pwd
/home/heba
 cd /usr/bin/
3. cd ~heba
  pwd
  /home/heba
 cd /usr/bin/
pwd
4.cd /home/heba
 pwd
/home/heba
cd /usr/bin/
pwd
5.cd $HOME
pwd
/home/heba 
 ## List Linux commands in /usr/bin that start with letter w 
  ls /usr/bin/w* 
  ## Display the first 4 lines of /etc/passwd
  $ head -4 /etc/passwd
root:x:0:0:root:/root:/bin/bash
daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
bin:x:2:2:bin:/bin:/usr/sbin/nologin
sys:x:3:3:sys:/dev:/usr/sbin/nologin
## .Display the last 7 lines of /etc/passwd 
tail -7 /etc/passwd
  colord:x:118:120:colord colour management daemon,,,:/var/lib/colord:/usr/sbin/nologin
gnome-initial-setup:x:119:65534::/run/gnome-initial-setup/:/bin/false
gdm:x:120:121:Gnome Display Manager:/var/lib/gdm3:/bin/false
nm-openvpn:x:121:122:NetworkManager OpenVPN,,,:/var/lib/openvpn/chroot:/usr/sbin/nologin
heba:x:1000:1000:Heba:/home/heba:/bin/bash
snapd-range-524288-root:x:524288:524288::/nonexistent:/usr/bin/false
snap_daemon:x:584788:584788::/nonexistent:/usr/bin/false 
 ## .Display the man pages of passwd the command and the file sequentially in one command 
 man -a passwd 
  ## Display the man  page of the passwd file. 
   man -s5 passwd  
 
  ## Display a list of all the commands that contain the keyword passwd in their man page  .
   man -k passwd

whatis passwd

passwd (1)           - change user password
passwd (1ssl)        - OpenSSL application commands
passwd (5)           - the password file
whatis -s1 passwd 
passwd (1)           - change user password
passwd (1ssl)        - OpenSSL application commands

 
