# Version control with Git

- Overview
  - Introduction to Version Control
  - Basic Concepts of Git
  - Setup Git Repository
  - Working with Git (add, Status, checkout)
    ( Using Git Command Line Tool )
  - Avoiding Merge Commits (rebase)
  - Going back in history (log)
  - Save work-in-progress changes (stash)
  - Reverting mistakes (revert, reset, etc)
  - Resolving Merge Conflicts
  - Concept of Branches

# Introduction

**Learning Objectives**

- Describe a repository.
- Identify benefits of using Git.
- Describe a commit .
- Create a local repository.
- Commit to a local repository.
- Create a remote repository.
- Push to a remote repository.
- Differentiate between the working tree, staging area, local repository and remote repository

### Introduction to git

→ Git is a modern and widely used distributed version control system

→ manage projects with high speed and efficiency

→ Version control system allows us to monitor and work together with team members at the workplace

### What is git ?

Git → open-source distributed version control system

### Features of Git

- Open Source → Git is an open source tool
- Scalable → Git is scalable (the number of users increases, the Git can easily handle such situations
- Distributed → Instead of switching the projects to another machine, can create a “Clone” of the entire repository
  Every user has their own repo and contains the entire commit history of the project
- Security → Git is secure. SHA1 (Secure hash function)→ name and identify objects within its repo.
  Files and commits are checked and retrieved by its checksum at the time of checkout.
  → stores its history ( The ID of particular commits depends upon the complete development history
- Speed → Fast (Complete all the tasks). Most of the git operations are done on the local repo. (Huge speed)
- Branching and Merging →
  great features of git, (SCM tools)
  Git allows the creation of multiple branches without affecting each other
  (Creation, deletion and merging on branches)

Create a separate branch → for a new module of the project, commit and delete it whenever we want

Production branch → which always has what goes into production and can be merged for testing in the test branch.

Demo branch → for the experiment and check if it is working. Remove it if needed.

The core benefit of branching is if we want to push something to a remote repository, we do not have to push all of our branches. Can select a few of our branches, or all of them together.

- Data Assurance →
  Git data model ensures the cryptographic integrity of every unit of project.
  It provides a unique commit ID to every commit through a SHA algorithm
  Can retrieve and update the commit by commit ID
- Staging Area →
  Can be considered as a preview of our next commit, moreover, an intermediate area where commits can be formatted and reviewed before completion
  D:\Git\git.jpg

- Maintain the clean history
  Git facilities with Git Rebase.
  It fetches the latest commits from the master branch and puts our code on top of that. Thus, it maintains a clean history of the project.
