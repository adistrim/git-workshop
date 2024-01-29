# Git workshop

## Basic Terminal / Git-bash Commands

### 'cd' - Change Directory
- ```cd directory-path``` Change your current working directory to the specified directory path.
```
Example:
cd Documents
```
- ```cd ..``` Go back to the parent directory/folder.

### 'ls' - List Files and Directories
- ```ls``` List files and directories in the current working directory.
- ```ls -a``` Lists hidden files also.
- ```ls directory-path``` List files and directories in long format, showing additional information.

### 'pwd' - Print Working Directory
- ```pwd``` Print the current working directory (absolute path).

### 'mkdir' - Make Directory
- ```mkdir directory-name``` Create a new directory/folder with the specified name.

### 'touch' - Create Empty File
- ```touch file-name``` Create an empty file with the specified name.

### Open VS Code
- ```code directory-name``` Opens that directory/folder in the VS Code
- ```code .``` Opens the current working directory/folder in VS Code.

## Git Commands
### Config

Configure your identity to associate your commits with your name and email.
<br>
```git config --global user.name "Your Name"```
<br>
```git config --global user.email "your.email@example.com"```
<br>
```git config --list```

### Initializing a Repository
- ```git init``` This command creates an empty Git repository in the current directory.

- ```git clone repository-URL``` This command copies a repository from a remote server to your local machine.

### Adding and Committing Changes
- ```git add filename```
Add a specific file to the staging area.

- ```git add .```
Add all changes in the current directory to the staging area.

- ```git commit -m "Your commit message"``` Create a new commit with the changes in the staging area.

### Checking Status and History
- ```git status``` View the status of your working directory and see which files are staged or modified.

- ```git log``` View the commit history, showing commit messages, authors, and timestamps.

### Branching
- ```git branch``` Check s the branch.
- ```git branch branch-name``` Create a new branch.
- ```git checkout branch-name``` Switch to the specified branch.
- ```git checkout -b new-branch-name``` Create and switch to a new branch in one command.
- ```git branch -d branch-name``` Deletes the branch basically.

### Merging Changes
- ```git diff target-branch-name``` Compares the branch.
- ```git checkout target-branch``` Switch to the target branch.
- ```git merge source-branch``` Merge changes from another branch.

### Remote Repositories
- ```git remote add origin repository-URL``` Associate a remote repository with your local repository.
- ```git remote -v``` Verifies the remote.

- ```git push origin branch-name``` Upload your local branch to the remote repository.

- ```git push -u origin brach-name``` Slighty helpful when you don't want to use whole long cmd. When ```-u``` is used it saves the upstream. So next time only ```git push``` is used.

- ```git pull remote-link branch-name``` Loads the remote repository's specific branch

- ```git pull origin branch-name``` Download changes from a remote repository and merge them into your local branch.

### Undoing changes
- ```git reset file-name``` Undo the add for a specific file.
- ```git reset``` Undo the add for the whole project folder.
- ```git reset HEAD~1``` Go to previous commit.
- ```git reset commit-hash``` Go to specific commit. ```commit-hash``` can be found using ```git log```.
- ```git reset --hard commit-hash``` Does the changes in code editor too.