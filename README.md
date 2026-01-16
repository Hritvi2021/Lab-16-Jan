# Lab-16-Jan

STEP-1

EC2 Setup and Linux Basics: Install Amazon Linux1.
Create a Virtual Machine:
VM: Create a new VM, allocate 2 GB RAM, 2 CPU cores, and 20 GB disk space.
<img width="1366" height="768" alt="Screenshot (13)" src="https://github.com/user-attachments/assets/f6170b09-2af1-433d-9c40-88c7b2947e7e" />

STEP-2

# Install Git:
    - Amazon Linux/Debian: sudo yum install git
    - Configure Username and Email:
     # Command
      bash
      git config --global user.name "Your Name"
      git config --global user.email "your.email@example.com"
   
# Initialize a Local Git Repository
1. Create a new directory: mkdir my-git-repo
3. Navigate to the directory: cd my-git-repo
4. Initialize a Git repository: git init
5. Verify the .git directory: ls -a (you should see a .git directory)
<img width="1366" height="768" alt="Screenshot (22)" src="https://github.com/user-attachments/assets/cb436e04-d498-42f4-b608-ab57b591a066" />

STEP-3

# Create Files and Track Changes
1. Create a new file: touch file1.txt
2. Add content to the file: echo "Hello, World!" > file1.txt
3. Check the status: git status (you should see the file as untracked)
4. Add the file to staging: git add file1.txt
5. Commit the file: git commit -m "Initial commit"
6. Check the status again: git status (you should see the file as committed)
<img width="1366" height="768" alt="Screenshot (23)" src="https://github.com/user-attachments/assets/1a337ac6-6a7c-418a-8231-5ead54c4a5dc" />

STEP-4 
# Create a GitHub Repository and Link with Local Repo
1. Create a new repository on GitHub: Lab-16-Jan
2. Copy the SSH or HTTPS URL: git@github.com:your-username/my-git-repo.git or https://github.com/your-username/my-git-repo.git
3. Link the local repository to GitHub: git remote add origin <URL>



