## Git and GitHub
## what is Git :-
    • Source control, version control is a way of tracking your file progress over time.
    • It is usually saved in a series of snapshots and banches which you can move back and forth between 
## what is Githib :-
    • GitHub is an application allowing you to store remote repositories(local machine)
    • you can interact with your GitHub repositorie through the push/pull system on your machine 
## the Difference :-
    • Git is a source control software allowing you to take snapshots and distribute your creations and modification over time
    • GitHub is an application allowing you to store and intreact with your repository on a remote server
    • Git is the bones and flesh of source control, while GitHub gives you the platfrom to work with your repository
## installing Git :-
    • Go to Google Chrome Search for Git 
    • Go to “git -scm.com” this website and than Downloads and choose your OS(Windowns, Linux)
    • For Linux Treminal > sudo apt install git 
    • For Windows Download and install and press NEXT NEXT.... 
      Go to control panle > program & freature > Turn windows freature on or off >search for windows subways for Linux > Turn it on than,
      Go to windows store and search for ubuntu and install the application

## Treminal Commands :-
	ls > list of files
	Mkdir > make a Folder 
	cd > opem Folder
	cd .. > going back in Folder
	rm -rf <FloderName> > delete the Folder
	rm file.txt > delete the file
	touch file.txt > make a file

## Creating a new repository in Local Machine:-
	mkdir  Folder 
	cd Folder
	git inti 

## Adding & Removing Files :-
	cd Folder
	git status
	git add NewFile.txt
	git status
	touch file1.txt
	touch file2.txt
	git status > now we can see the Difference b/w track and un-track files
	git add . > . mean all files
	rm NewFile.txt  >  delete the file
	git status 
	git rm – cached file2.txt > remove the specific file from the staging area
	git status
	Your First Commit :-
	cd Folder 
	git status
	git config –global user.emal “your@gmail.com”
	git config –global user.name “yourname”
	git commit -m “Added New file”
	git commit -a -m “Added All files”
	git log > show the changes commited

## Git checkout :- checkout the basically Revert the File deleted in local machine and also used as switch b/w branch

	cd folder 
	git log
	git checkout  <FileName>

## Git Revert & Reset :-
	Revert:
	git log 
	git revert <CommitID> > Bring Back the Old Functionally
	git log
	Reset: Reset is 3 types Soft,Mix,Hard
	git log
	git reset – hard <CommitID> 

	Creating git ignore File :- this File is ignored by the commite command
	cd Folder
	git status
	git add . 
	git commit -m “ModifiedFile”
	git status
	touch .gitignore > open it using GUI and write anything
	git status
	git commit -m “ignorefile”

## Git Branch :-

what is Branch ?
    • Git Branch are a way to create separate Development paths without Overring or Creating copies of your project
    • Branch can be Added Deleted and Merged like Commit


## Working with Branch:-
	mkdir MyNewDir
	cd MyNewDir
	git init 
	mkdir src
	mkdir lib
	cd src
	touch file1.txt
	touch file2.txt
	cd ..
	cd ..
	touch lib.py
	touch file2.txt
	cd ..
	git status
	git add . >
	git commit -m “intial commit”
	git checkout – b dev > creating a branch and switching to that branch
	git checkout master > switching Back to Master
	git branch <BranchName> >another way of creating branch
	git branch –a > list of Branch
	git branch -d <BranchName> > deleting the Branch

## Mergring  Branch:-
	git checkout dev (branch name is dev)
	git status
	git add
	git commit -m “Merging the branch into master”
	git checkout master 
	git status
	git merrge dev
	git log

## Git Push & Pull :- here i’m creating own new repo in GitHub and clone it, pulling it and deleting the Readme.md File than Pushing it back.

	git pull > this pull eveything 
	( first you have to flok the repo and clone in your local machine)
	git pull origin master > tjhis pull master branch
	git status
	git log 
	ls 
	rm readme.md
	ls
	git add .
	git status
	git commit -m “Removed”
	git log
	git push -u origin master
	git status
	vim
## Git Clone, Pull, Merge, Push:- Here for example in GitHub repo there is a Error in Funtion.js file So we can fix like this

	git clone http://www.github.com/userid/repo
	git pull
	ls
	git checkout -b Error1 > branch created and switching to that branch
	ls
	vim funtion.js
	git add .
	git status
	git commit -m “Fixed” 
	git checkout master > Switching back to master branch
	git merge Error1 > merging our branch with master branch
	git log
	git push origin Error1 > push the change 
	git log > show the activity of the git.
	git push origin  - -delete Error1 > after the change push to GitHub repo we can delete the branch

