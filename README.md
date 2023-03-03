# Eagles Team - Git & Githud practicals 
## ********** How to connect to the remote repo to add your name to the members list  **********

### Step 1 : Set up Git 
Before you start working with Git, you need to set up your Git configuration.

1.1 Open your terminal (or Git Bash on Windows) and run the following command to check if you have already set up Git:   
$ git config --list 

If you get a list of Git configurations, it means that Git is already set up on your computer. Otherwise, 
you need to set up Git by running the following two commands (replace "username" and "email" with your GitHub username and email address):

$ git config --global user.name "username"                             
$ git config --global user.email "email address"

note: when coping command do not include $ sign 

### Step 2 - Create a new folder and initialize git.

2.1 Open your terminal and navigate to the directory where you want to create the folder
example cd /home/ec2-user

2.2 Create a new folder called "Eagles" by running the following command 
$ mkdir Eagles 

2.3 Navigate into the "Eagles" folder by running the following command:
$ cd Eagles 

2.4 Initialize Git in the folder by running the following command:
$ git init

2.5 Change the default branch name from "master" to "main" by running the following command:
$ git branch -m main 

### Step 3 - Connect to your remote repository  

3.1 Check if you are already connected to a remote repository by running the following command:
$ git remote -v 

If you get a list of remote repositories, it means that you are already connected to a remote repository. 
Otherwise, you need to connect to the remote repository by following the next step 

3.2 Add github 
$ git remote add origin https://github.com/Lamptechsys/Eagles.git

3.3 Check if the remote repository is connected by running the following command: 
$ git remote -v 

### Step 4 - Pull files from the remote repository  

4.1 Run the following command to pull the files from the remote repository:
$ git pull origin main 

4.2 check if the content has been sucessfully pulled by running the following command:
$ git status 

### step 5 - Add your name to the list of members 

5.1 Open the "Eagles.md" file by running the following command:
$ vi Eagles.md 

5.2 Press "i" to enter insert mode, and add your name to the list of members under the last name.

5.3 Press "Esc" to exit insert mode, and type ":wq!" to save and exit the file.

### Step 6 - Commit and push your changes to the remote repository 

6.1 Run the following commands to add and commit your changes
$ git status                                       
$ git add .                                                         
$ git commit -m " "name" has update his/her name on the memebers list "                                 

6.2 Run the following command to push your changes to the remote repository: 
$ git push -u origin main  

# Congratulations! You have successfully added your name to the members list in the remote repository. 
You can check the remote repository on GitHub to see your name in the commit history.



