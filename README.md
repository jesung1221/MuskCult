Practice using git with freecodecamp git tutorial.
#if want to edit initial setups in Git Bash:
~/.bash_profile

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



