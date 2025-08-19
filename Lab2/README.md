## 1:1. Create a user account with the following attribute
 username: islam
 Fullname/comment: Islam Askar
 Password: islam 
 ![img](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-19%2021-26-07.png)
 ![img](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-19%2021-35-56.png)
 ##  2:Create a user account with the following attribute
 Username: baduser
 Full name/comment: Bad User
 Password: baduser  
![img](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-19%2021-32-10.png)
![img](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-19%2021-35-20.png)
  
## Create a supplementary (Secondary) group called pgroup with group ID of 30000 
![img](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-19%2021-46-20.png)
![img](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-19%2021-46-46.png)
 
 ## Create a supplementary group called badgroup
    
 ![img](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-19%2021-50-41.png)
 ## Add islam user to the pgroup group as a supplementary group
  ![img](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-19%2021-55-25.png)
 
 ## Modify the password of islam's account to password 
 ![img](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-19%2021-56-29.png)
 

## Modify islam's account so the password expires after 30 days
![img](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-19%2021-58-07.png)
![img](https://github.com/heba-eldeabes/Red-Hat-Administration-I/blob/main/images/Screenshot%20from%202025-08-19%2022-00-24.png)

## Lock bad user account so he can't log in   

## Delete bad user account 

## Delete the supplementary group called badgroup.
 

 ## Create a folder called myteam in your home directory and change its permissions to
 ## read only for the owner. 



## -Log out and log in by another user


 ## Try to access (by cd command) the folder (myteam) 

## Using the command Line
##  Change the permissions of oldpasswd file to give owner read and write
## permissions and for group write and execute and execute only for the others
##  using chmod in 2 different ways
  
 
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
 
 
 ## What is the difference between the “x” permission for a file and for a
 ## directory?
x in file  executable file  
x in dir we can execute to the dir    