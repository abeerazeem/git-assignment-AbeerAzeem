# Git Assignment — Answers
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

