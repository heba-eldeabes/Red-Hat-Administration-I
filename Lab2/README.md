## 1:1. Create a user account with the following attribute
 username: islam
 Fullname/comment: Islam Askar
 Password: islam 
 
![question1](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-09%2023-20-37.png)
 ##  2:Create a user account with the following attribute
 Username: baduser
 Full name/comment: Bad User
 Password: baduser 
 
![question1](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-09%2023-20-37.png)
## Create a supplementary (Secondary) group called pgroup with group ID of 30000 

 ![question2](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-09%2023-23-28.png)
 ## Create a supplementary group called badgroup
    
 ![question3](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-09%2023-29-01.png)
 ## Add islam user to the pgroup group as a supplementary group
 
 ![question3](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-09%2023-29-01.png)
 ## Modify the password of islam's account to password
 
![question4](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-09%2023-29-09.png)
## Modify islam's account so the password expires after 30 days
![img](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-19%2017-41-26.png)
## Lock bad user account so he can't log in   
![question5](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-10%2001-09-22.png)
## Delete bad user account 
![img](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-19%2017-18-32.png)
## Delete the supplementary group called badgroup.
 
 ![question6](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-10%2001-13-28.png)
 ## Create a folder called myteam in your home directory and change its permissions to
 ## read only for the owner. 


![question6](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-10%2001-20-27.png)
## -Log out and log in by another user

![question7](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-10%2001-22-00.png)
 ## Try to access (by cd command) the folder (myteam) 
cd  myteam 
bash: cd: myteam: Permission denied  
## Using the command Line
##  Change the permissions of oldpasswd file to give owner read and write
## permissions and for group write and execute and execute only for the others
##  using chmod in 2 different ways
  
 ![question7](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-10%2001-30-52.png)
 ![Question8](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-10%2001-36-22.png)
 ![question9](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-10%2001-37-18.png)
 ![question10](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-10%2001-42-17.png)
 ![question11](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-10%2001-47-31.png)
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
 
 ![question12](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-19%2017-21-28.png)
 ## What is the difference between the “x” permission for a file and for a
 ## directory?
x in file  executable file  
x in dir we can execute to the dir    