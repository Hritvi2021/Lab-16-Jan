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
<img width="1366" height="768" alt="Screenshot (24)" src="https://github.com/user-attachments/assets/a4d9698b-4a52-4375-89cf-91c7a578b41c" />

STEP-5
 
 # Push Local Commits to Remote GitHub Repository
 1. Push the changes: git push -u origin master (or main if your default branch is main)
    <img width="1366" height="768" alt="Screenshot (25)" src="https://github.com/user-attachments/assets/c9de3f61-3501-4d63-a409-7a186f3aedd5" />

STEP-6

# Create a New Branch, Make Changes, and Merge
1. Create a new branch: git branch feature/new-feature
2. Switch to the new branch: git checkout feature/new-feature
3. Make changes: echo "New feature" > file2.txt
4. Add and commit the changes: git add . and git commit -m "Add new feature"
5. Switch back to the main branch: git checkout master (or main)
6. Merge the changes: git merge feature/new-feature
7. Delete the feature branch: git branch -d feature/new-feature
<img width="1366" height="768" alt="Screenshot (26)" src="https://github.com/user-attachments/assets/96f20aea-3bb0-4558-b62b-0651c79d9dca" />

STEP-7

1. Practice Rollback1. Check the commit log: git log
2. Reset to a previous commit: git reset <commit-hash> (use --soft or --hard options as needed)
3. Checkout a previous commit: git checkout <commit-hash> (use -b option to create a new branch)




