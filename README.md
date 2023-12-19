Practice using git with freecodecamp git tutorial.
#if want to edit initial setups in Git Bash:
~/.bash_profile

# Most common flow of commands:

git add .
git status # Lists all new or modified files to be committed
git commit -m "Second commit"
git push -u origin master


Commands:
ssh -T git@github.com    //for github ssh connection 
#start git
git init

# Add all the files in the local repository and stages them for commit
git add .
	#for a specific file
git add README.md

#See which files are staged:
git status

#commit changes to Git Repo
git commit -m "first commit"

#uncommit changes made to Git Repo
option1: git reset HEAD~1

option2: 
JaeSeong@JAE-PC2 MINGW64 /c/Users/JaeSeong/Desktop/MuskCult (master)
$ git log
commit e763748029d183bee3be1c67bc5316d0923adc6a (HEAD -> master)
Author: JaeSeong Kim <jesung1221@hotmail.com>
Date:   Tue Dec 19 14:49:45 2023 +0200

    First commit

JaeSeong@JAE-PC2 MINGW64 /c/Users/JaeSeong/Desktop/MuskCult (master)
$ git reset --soft e763748029d183bee3be1c67bc5316d0923adc6a

#Add a remote origin (Github)
Option 1: 
git remote add origin git@github.com:jesung1221/MuskCult.git

Option2:
git remote add origin remote_repository_URL
git remote set-url origin git@github.com:jesung1221/MuskCult.git

#git remote command lets you create, view and delte connections to other repositories
# List the remote connections you have to other repositories

git remote -v

#Push changes in your local repository up to the remote repository 

git push -u origin master

#see difference between current working file to the last committed one

git diff

# revert back to the last committed version to the Git Repo:

git checkout . 

OR for a specific file

git checkout -- <filename>

#view commit history

git log


