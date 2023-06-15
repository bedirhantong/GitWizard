

### **Initialize**
- Attention to the right directory

````
git init
````


---


- to see git version

````
git --version
````


---





### **Clone**
- existing repo into a new directory

````
git clone <repo-url> <directory>
````
- existing repo into current directory

````
git clone <repo-url> .
````





---




### **Configure**
- email and name

````
git config --global user.name "username" 

git config --global user.email "email address"
````
- to see the name and email
````
git config user.name

git config user.email
````
- default editor (as an example I will change it to vim)

````
git config --global core.editor "vim"
````
- colorization on command line terminal

````
git config --global color.ui auto
````
- default editor (as an example I will change it to vim)

````
git config --global core.editor "vim"
````
- default editor (as an example I will change it to vim)

````
git config --global core.editor "vim"
````

---



### **Add new changes**
- To add all the files in the current directory, use "git add ."


````
git add .
````
- To add a directory 
````
git add <directory>
````




---




### **Commit**
- commit all local changes in tracked files. 
````
git commit -a
````
- commit all staged changes

````
git commit -m <commit message>
````



----


### **Compare Commits**
- compare two commits and output result in the terminal 
````
git diff <sha1> <sha2>
````
- compare two commits and output result in a file 

````
git diff <sha1> <sha2> > diff.txt
````



----




### **Revert**
`Use git log to see the hash of each commit `

- to last commit on local
````
git reset --hard
````
- to last commit on remote branch

````
git reset --hard <repo>/<branch>
````
- a specific commit

````
git revert <commit-hash>
````
- a specific file

````
git checkout <repo>/<branch> <filename>
````


----



### **Add new branch** 
- and remain in the current branch I am working from
````
git branch <new name>
````
- and switch to the new branch
````
git checkout -b <new name>
````
- from another branch
````
git checkout -b <new name> <another branch>
````

- change branch
````
git switch <to branch name>
````

---



### **Merge**
- another branch to the current branch

````
git merge <branch-name>
````

- merge single file to the given branch

````
git checkout <branch name> <path to file> --patch
````

----


### **View** 
- commit history
````
git log
````
- status of the including staged, unstaged and untracked files
````
git status
````
- uncommited changes
````
git diff
````
- commited/staged changes
````
git diff --staged
````
- branches and `the active branch is prefixed with *`
````
git branch
````
- repo's remote url
````
git remote -v
````

---


### **Remove** 
- a branch
````
git branch -D <branch name>
````
- multiple branch by name
````
git branch -D <branch name> <branch name> <branch name>
````
- from another branch
````
git checkout -b <new name> <another branch>
````

---


### **Ignore**
`Just modify/edit .gitignore file based on your project` 
