# Git Assignment — Answers

# Part 1 — Concepts & Theory (20 marks)
## Q1. Terminal basics (2 marks each = 6 marks)
### 1. What is a terminal? How is it different from clicking through folders in a file explorer?
A terminal is an interface where you type commands to do actions with your computer. You can use it to create files, make folders, run programs. instead of manually doing these things, you can do them with just 1 command.
A terminal lets you control your computer by typing commands, while file explorer  lets you control it by clicking a graphical interface. both have the same purpose, a terminal makes things quicker as you can do everything in one place

### 2. Write the terminal command to: (a) list all files including hidden ones, (b) create a folder called project , (c) move into that folder.
we can use ls to list all the files, if we want the hidden ones too we can use ls -Force . mkdir project is the command to make a folder . cd project is change directory that helps u move into that folder.

### 3. What does the cd .. command do? What about cd ~ .
the cd .. helps you move one step back in the directory, for eg if u are in desktop/gd, and you do cd .. you will move back in desktop.  cd ~  moves you to the home directory.

## Q2. Version control concepts (2 marks each = 8 marks)
### 4. Explain what version control is in your own words. Give one real-world analogy (not Google Docs — pick your own).
Version control tracks changes made to files over time. It helps us to see what changed, who made the changes, and when they were made. it helps make things easier and more organized if more than 1 person works on something.
its like when youre doing a science project and tasks are divided, if one person is supposed to make a volcano model and the other  makes the volcano mixture, both do their tasks parallel wiithout one disturbing the other.

### 5. What is the difference between Git and GitHub? Can you use Git without GitHub?
git is a version control tool that tracks changes in our code. It lets you create commits, branches, update and push your changes in your repo.
github is an online platform where we can make repositories where u can store your code, share code with others, and work with other people. no we cannot use git without github as it needs a repo to version control

### 6. Name three features GitHub provides that Git alone does not.
Allows team members to review and discuss code changes before merging them. generate pull requests and join code
stores repositories online so multiple people can access and contribute to the same project.
lets users create their own copy of another person's  repository  thru forking to experiment  or contribute changes.

### 7. What is a repository? What is the difference between a local repository and a remote repository?
a repository  is a place where your project files are stored. It tracks changes made to files, commits, and branches.
a local repository is stored on your own computer, where you can manage files, track changes, and save commits. A remote repository is stored on a cloud server or a platform like github that allows you to back up your code and share it with others.

## Q3. Git internals (3 marks each = 6 marks)
### 8. Explain what HEAD means in Git. What happens to HEAD when you switch branches?
head in git is a pointer that tells you which commit you are currently working on, that is usually through your current branch. when you switch branches  head moves to  the new branch's latest commit.

### 9. What is a .gitignore file? Write a .gitignore that ignores: all .log files, a folder called node_modules/ , and any file ending in .env 
a .gitignore file tells  which files and folders to ignore so they are not tracked or included in future commits. It is  used for log files, files containing sensitive information like .env.
*.log
node_modules/
*.env





# Exercise 2.2 — The staging area (8 marks)

We committed features A and B separately from  C to keep our changes organized into smaller commits so they dont get messy. If feature A abd B are dependant or related to each other, they should be committed together so we know theyre related.  
keeping them separate will help us track the changed we made in the files and understand why we did the commit.
we will separate c when its unrelated to a and b 

Joined:
September 2026 

# Exercise 2.3 — Push & pull (7 marks)

If  you make a local commit without pulling first, you  will be making changes to an updated branch, if we are working with multiple people and they are making changes too, pulling first will update our work locally that will include commits by other people too. if we commit withoout pulling, it will create conflicts , if someone else had already worked on the file ypure working on and you wont have that updated wprk if u hadnt pulled. 

# Exercise 3.1 — Branch basics (10 marks)
it was a fast forward merge, when i ran the command git merge feature/profile-page , the terminal stated 
Updating bfe3c67..9f0e917
Fast-forward anf upon running the command git log --oneline --graph --all  the out showed a linear commit history without any separate merge commit.

# Exercise 3.2 — Deliberate conflict (15 marks)
the conflict happened because we changed the same line in the 2 files in the 2 branches, no there would be no conflict if different lines were edited 
there would also be no changes if if one branch edited team.txt and the other edited about.md because both are different files  when we merge bpth, none of them are contradictory

# Exercise 4.1 — Feature branch workflow (15 marks)

## 1. What is the purpose of a Pull Request? Why not just merge directly?
A pull request allows the hehad/ team lead  to review , discuss and test code changes before merging them into the main branch. The main brnach is where all the bug free , tested code is, if we merge it directly.  there will be no code tests, no catching bigs, there is a high chance that a buggy code will be merged into the main and ruin the wholw project.

## 2. Name two things a reviewer should check in a Pull Request
the reviwer should test whether  the code works as expected and does not have  bugs.
he should also check the quality, that it is readable, follows coding standards like being modular etc

## 3. What is the difference between a merge commit and a fast-forward merge?
Merge commit is when  git creates a new commit that joins the histories of two branches this is when both branches have commits.
In fast forward merge, Git  moves the current branch  forward to the latest commit of the other branch when there are no diverging commits.

