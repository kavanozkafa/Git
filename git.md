# Git Tutorial
## Created by kavanozkafa


#### for usage manuel
	#git help

#### config our username and email
	#git config --global user.name "sammas"
	#git config --global user.email "sammas@gmail.com"


#### show everything configs

    #git config --list


#### create repo
	#cd path_folder 
	#git init 

#### clone a repo
    #git clone repo_url

#### commit all files
	#git add .
	#git commits -m "this is commit message"
	this means take snapshots of all things and maybe you later fuck things up and takes it back.

#### Pushing to a GitHub Repository
	#git remote add project_name https://github.com/user/repo.git 
	#git push -u project_name branch(master vs)

#### Commit Directly to the Repository
	#git commit -am "message"


#### view logs 
	#git log
	#git log --author="sammas"

#### view working status
	#git status

#### view the changes you made
	#git diff

#### delete files
	#git rm file.uzantı


#### rename files
	#git mv msg.txt mesaj.txt

#### moving files
	#git mv msg.txt home\sammas\msg.txt


#### Getting Old Versions from the Repository
	#git log
	#git checkout 0128dba..... -- index.html





![git](https://github.com/kavanozkafa/Git/blob/master/git%20workflow.jpg)