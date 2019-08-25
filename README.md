# Git Tutorial
## Created by kavanozkafa


***

### **User Settings**

#### for usage manuel
	#git help

#### config our username and email
	#git config --global user.name "sammas"
	#git config --global user.email "sammas@gmail.com"


#### show everything configs

    #git config --list



***

### **Create**

#### create repo
	#cd path_folder 
	#git init 

#### clone a repo
    #git clone repo_url

***


### **Local Changes**


#### view working status
	#git status

#### track changed files
    #git diff

#### add a file to next commit
    #git add -p <filename>
 
#### commit all files
	#git add .
    this means take snapshots of all things and maybe you later fuck things up and takes it back.

#### commit message
	#git commits -m "this is commit message"
	

#### change the last commit 
    #git commit --amend
    dont do it to pushed commits

#### Search for commits that include a keyword
    #git log -S"config.menu_items"


***
### **Local History**


#### view logs 
	#git log
	#git log --author="sammas"
    #git log -p file

#### show stats
    #git log --stat

#### Print out visualization of your log
    #git log --pretty=oneline --graph --decorate --all

#### look at who and what changed in file
    #git blame file

#### show pathces
    #git log -p



***
### **Branches**


#### list branches
    #git branch -av

#### switch HEAD branch
    #git checkout <branch>

#### create a new branch based on your current HEAD
    #git branch <newBranch>

#### delete local branch
    #git branch -d <branch>

#### mark the commit
    #git tag <tagName>

#### create branch from remote branch
    #git checkout --track <remoteBranch>

***

### **Publish**

#### Pushing to a GitHub Repository
	#git remote add project_name https://github.com/user/repo.git 
	#git push -u project_name branch(master vs)


#### Commit Directly to the Repository
	#git commit -am "message"

#### list all configured remotes
    #git remote -v

#### show info about remote
    #git remote show <remotename>

#### download all changes from remote but dont integrate into HEAD
    #git fetch <remote>

#### download all changes from remote and merge to HEAD
    #git pull <remote> <branch>

#### publish your tags
    #git push --tags


***
### **Merge**


#### merge branch into your current HEAD
    #git merge <branch>
#### rebase your current HEAD onto branch
    #git rebase <branch>


#### abort rebase
    #git  rebase --abort



***
### **Undo**

#### delet all local changes
    #git reset --hard HEAD

#### delete one file changes
    #git checkout HEAD <file>


#### reset your HEAD to previous commit
    #git reset --hard <commit>

    preserve all changes as unstaged changes
    #git reset <commit>

    and preserve uncommitted local changes
    #git reset --keep <commit>



#### delete files
	#git rm file


#### rename files
	#git mv msg.txt mesaj.txt

#### moving files
	#git mv msg.txt home\sammas\msg.txt


#### Getting Old Versions from the Repository
	#git log
	#git checkout 0128dba..... -- index.html



![git](https://github.com/kavanozkafa/Git/blob/master/git%20workflow.jpg)



***
## Create Alias

    alias gitA="git add -A ."
    alias gitC="git commit -m"
    alias gitP="git push"


#### List all git aliases
    #git config -l | grep alias | sed 's/^alias\.//g'





