# **GIT Introduction**

* GIT  stands for 'Global Information Tracker'.
* It is a free and open source distributed version control system.
* It is usually used for Collaboration where multiple developers work together.
* It is used to tracking changes in the souurce code. 

## **Version Control System**
 
  <p>It is a system that records changes made to a file or a set of files.The system records all the made changes to a file so a specific version may be rolled if required in the future.

  The responsibility of the Version control system is to keep all the team members on the same page. It makes sure that everyone on the team is working on the latest version of the file and, most importantly, makes sure that all these people can work simultaneously on the same project.</p>

### **Types**

### 1.**Distributed version control system(DVCS)**

   ![DVCS](https://github.com/ShibaniRath23/missingskill-learning/blob/master/Images/DVCS.png)

### 2.**Centralised version control system(CVCS)**

   ![CVCS](https://github.com/ShibaniRath23/missingskill-learning/blob/master/Images/CVCS.png)

### **Difference between DVCS and CVCS**

|DVCS|CVCS|
|---|-----|
|Every user has a local repository.|Only central repository.|
|More developers work together at a time.|Only  one developer work.|
|e.g. GIT|e.g. Subversion|

## **Git Commands**

### * Working with Local directories:-


  1. git init :
     --------

  This command turns a directory into an empty Git repository. This is the first step in creating a repository. After running git init, adding and committing files/directories is possible.

    Usage: git init [repository name]

 

  2. git add :
     --------

  Adds files in the to the staging area for Git. Before a file is available to commit to a repository, the file needs to be added to the Git index (staging area). There are a few different ways to use git add, by adding entire directories, specific files, or all unstaged files.

    Usage: git add [file]  
    

  3. git commit:
     ------------

  Record the changes made to the files to a local repository. For easy reference, each commit has a unique ID.Adding a commit message helps to find a particular change or understanding the changes.

    Usage: git commit -m “[ Type in the commit message]”  

  4. git status:
     -----------

  This command returns the current state of the repository.

    Usage: git status  

  5. git config:
     ------------

   git config is used for two important settings (user user.name and user.email).These values set what email address and name commits will be from on a local computer.
     
    Usage:git config –global user.name “[name]”  

    Usage: git config –global user.email “[email address]”  
 
  6. git branch:
     ----------
   To determine what branch the local repository is on, add a new branch, or delete a branch.

    Usage: git branch  
 
  7. git checkout:
     -----------
  To start working in a different branch, use git checkout to switch branches.
   
    Usage:git checkout [branch name]  

  8. git merge:
     ---------
  Integrate branches together. git merge combines the changes from one branch to another branch. For example, merge the changes made in a staging branch into the stable branch.

    Usage:git merge [branch name]  

### **Working with remote repositories**

   1. git remote:
      -------------
  To connect a local repository with a remote repository. A remote repository can have a name set to avoid having to remember the URL of the repository.

    Usage:git remote add [variable name] [Remote Server Link]  

   2. git clone:
      ------------
  To create a local working copy of an existing remote repository, use git clone to copy and download the repository to a computer. Cloning is the equivalent of git init when working with a remote repository. Git will create a directory locally with all files and repository history.

    Usage:git clone [url]  

   3. git pull:
      ---------
  To get the latest version of a repository run git pull. This pulls the changes from the remote repository to the local computer.

    Usage: git pull [Repository Link]  

   4. git push:
      ----------
  Sends local commits to the remote repository. git push requires two parameters: the remote repository and the branch that the push is for.

    Usage:git push [variable name] master  

 ### **Advanced Git Commands**
  
   1. git stash:
      -----------
  To save changes made when they’re not in a state to commit them to a repository. This will store the work and give a clean working directory.

    Usage:git stash save  

   2. git log:
      ---------
  To show the chronological commit history for a repository. This helps give context and history for a repository. git log is available immediately on a recently cloned repository to see history.

    Usage:git log  

   3. git rm:
      --------
  Remove files or directories from the working index (staging area). With git rm, there are two options to keep in mind: force and cached.
      
    Usage:git rm [file]  

## **Git Workflow**
![GIT workflow](https://github.com/ShibaniRath23/missingskill-learning/blob/master/Images/GIT%20WORKFLOW.png)