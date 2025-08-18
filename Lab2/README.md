## 1:1. Create a user account with the following attribute
 username: islam
 Fullname/comment: Islam Askar
 Password: islam 
 1 : username 
    1:sudo useradd islam
    2:[sudo] password for heba:
    3:tail -1 /etc/passwd
    4:islam:x:1003:1003::/home/islam:/bin/bash   
2:Fullname/comment: Islam Askar
    sudo useradd  -c"islam Askar" -md /home/user3  -s /bin/bash user2
3:Password: islam   
 sudo passwd islam
 New password:
Retype new password:
passwd: password updated successfully  
![question1](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-09%2023-20-37.png)
 ##  2:Create a user account with the following attribute
 Username: baduser
 Full name/comment: Bad User
 Password: baduser 
 1: Username: baduser
  sudo useradd baduser
  tail -1 /etc/passwd
  baduser:x:1017:1017::/home/baduser:/bin/bash
 
 2:Full name/comment: Bad User 
 sudo useradd   -c"bad user " -md /home/user2 -s  /bin/bash user2
tail -1 /etc/passwd
user2:x:1004:1017:bad user :/home/user2:/bin/bash  
![question1]()
## Create a supplementary (Secondary) group called pgroup with group ID of 30000 
 sudo groupadd pgroup -g 30000  
 ![question2]()
 ## Create a supplementary group called badgroup
 sudo groupadd badgroup   
 ![question3]()
 ## Add islam user to the pgroup group as a supplementary group
 sudo usermod -aG pgroup islam 
 ![question3]()
 ## Modify the password of islam's account to password
sudo passwd islam 
New password:
Retype new password: 
passwd: password updated successfully  
![question4]()
## Modify islam's account so the password expires after 30 days
sudo chage -M 30days islam 
## Lock bad user account so he can't log in
sudo usermod -s/sbin/nologin baduser    
## Delete bad user account 
sudo userdel baduser 
## Delete the supplementary group called badgroup.
 sudo groupdel badgroup  
 ## Create a folder called myteam in your home directory and change its permissions to
 ## read only for the owner. 

 1- mkdir myteam

 2-ls -ld myteam
 3- -rw-rw-r-- 1 heba heba 0 Aug  6 23:33 halp
 4-chmod 400 myteam 
 5 - ls -l myteam
dr-------- 2 heba heba 4096 Aug 10 01:15 
## -Log out and log in by another user
su - islam 
Password: 
Authentication failure . 
 ## Try to access (by cd command) the folder (myteam) 
cd  myteam 
bash: cd: myteam: Permission denied  
## Using the command Line
##  Change the permissions of oldpasswd file to give owner read and write
## permissions and for group write and execute and execute only for the others
##  using chmod in 2 different ways
::1:: 
chmod u=rw,g=wx,o=x oldpasswd
-rw--wx--x 1 heba heba 0 Aug 10 01:27  
::2::
chmod 631 oldpasswd 
-rw--wx--x 1 heba heba 0 Aug 10 01:27 

::3::
umask -S 146 
777-631 =146 
umask u=rw,g=wx,o=x  

::4::
umask -s u=rw,g=rw,o=rw 
umask 000 
touch Ahmed 
ls-l Ahmed 
-rw-rw-rw- 1 heba heba 0 Aug 10 01:41 Ahmed
 :5:
umask 777
 touch life 
 ls -l life 
 ---------- 1 heba heba 0 Aug 10 01:47
 
 mkdir life2 
 ls -ld life2 
 d--------- 2 heba heba 4096 Aug 10 01:50  
 ## 17. What are the minimum permission needed for:
 Copy a directory (permission for source directory and permissions for target
parent directory)  rx ----wx
 Copy a file (permission for source file and and permission for target parent
directory) r------------wx
 Delete a file = nopermissin
 Change to a directory x
 List a directory content (ls command) r
 View a file content (more/cat command) r
 Modify a file content  rw
 ## 18- 
 touch kil 
 chmod 444 kil 
 -r--r--r-- 1 heba heba 0 Aug 10 01:52 kil
 by this permission we can just read and remove the file but can't edit the file 
 rm kil
 ## What is the difference between the “x” permission for a file and for a
 ## directory?
x in file  executable file  
x in dir we can execute to the dir    