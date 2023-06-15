<!--Satırların sonundaki "\" işareti bir alt satıra geçirmek için kullanılıyor. Kullanmazsanız linkler birbirine girebilir. -->

# GitWizard

Welcome Coder to GitWizard, where I will explain the basics of Git, one of the version control systems.

Before you start, please make sure you have a basic understanding of terminal so that you can feel comfortable using the Git interface.

Git, a popular distributed version control system, is a software/tool that helps you track changes, collaborate with others, and seamlessly manage your codebase throughout its lifecycle.

This project will be a resource for you to improve your skills with Git and its various features. Whether you are new to the basics, a beginner, or an experienced developer looking for advanced techniques, you can contribute to both yourself and GitWizard.

In this repository you will find a series of guides, tutorials and practical examples covering a wide range of Git commands and workflows. You will learn about branching and merging strategies, remote repository management, conflict resolution, and much more.

I want you to be an active participant in this project by sharing your feedback, asking questions, and suggesting improvements. I'm not a version control expert by myself, but together we can provide a huge resource for everyone. 

`I'm trying to free your mind, Neo. But I can only show you the door. You're the one who has to walk through it.`

---


### **Attention**
- `Before you begin, please be sure that you have a basic understanding of terminal so that you can feel comfortable with the git interface.`

---

## Contents
* [Git commands](#initialize)
    * [Setup](#setup)
    * [initialize](#initialize)
    * [Clone](#clone)
    * [Configure](#configure)
    * [Changes](#changes)
    * [Commit](#commit)
    * [Revert / Reset](#revert)
    * [Branch](#merge)
    * [Merge](#merge)
    * [Commit](#commit)
    * [View](#view)
    * [Remove](#remove)
    * [ignore](#ignore)
* [Useful Links](#links)
    

---



### **Setup**
- To install git on your device you can use following secure websites
    - [Git Guides](https://github.com/git-guides/install-git)
    - [Git official website](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)



---


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
- To add a directory use "git add <directory>"

````
git add
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




### Links

- The entire Pro Git book, written by Scott Chacon and Ben Straub. Use [me](https://git-scm.com/book/en/v2)

- To find needed commands easily. Use [me](https://gitexplorer.com/)

- Learning git with visualization? Use [me](https://learngitbranching.js.org/)


