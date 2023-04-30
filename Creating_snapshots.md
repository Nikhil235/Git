First time Setup →

1. Check version
   $ git —version
   (git version “current version”)
2. Set Config values.
   a. Define author name to be used for all commits in current repo. Devs commonly use —global flag to set config options for current user.

→$git config —global [user.name](http://user.name) “Nikhil Arjun”

b. Define author email id to commit in repo

→$git config —global [user.email](http://user.email) “nikhilarj338@gmail.com”

c. To check Those values
→$git config —list

1. Having trouble remembering commands or options for commands, you can use _Git Help_
   → $ git command -help
   → $ git help command
   → $ git help -all

1. Getting Started…
   Two Common Scenerios →
   a. Existing project on your local machine
   b. Existing project remotely

1. Create empty git repo in specified directory. Run with no arguments to initialize the current directory as a git repository.
   → $ git init

1. Before First Commit
   List which files are staged, unstaged and untracked.
   → $ git status

1. Add gitignore file
   Simple text file where we can add files that we want git to ignore
   .e.g. .DS_Store
   .project
   \*. Pyc (any extension)

![Screenshot 2023-04-30 074759.png](https://"C:\Users\Nikhil Arjun\Pictures\Screenshots\Screenshot 2023-04-30 074759.png")

2. Add files to staging area
   Stage all changes in <directory> for the next commit.
   Replace < directory> with a <file> to change a specific file.
   → $ git add <directory>

To add all files from local directory
→ $ git add -all
→ $ git add -A
→ $ git add . (adds untracked, renamed, modified, deleted (remove files from a directory) files)

Check list which files are staged, unstaged and untracked.
→ $ git status

1. Remove Files From Staging area.
   Files that we want to remove form git
   → $git reset <file >
   → $git reset (Remove everything)

2. Our first commit
   → $ git add -A
   → $ git commit -m “Initial Commit”
   ( Commit the staged snapshot, but instead of launching a text editor, use <message> as the commit message )

→ $ git status
→ $ git log
( Display the entire commit history using the default format. For customization see additional options. )

3. Show unstaged changes between your index and working directory
   → $ git diff

4. Cloning a Remote repo
   Clone repo located at <repo> onto local Machine. Original repo can be located on the local filesystem or on a remote machine via HTTP or SSH.

→ $ git clone <url> < where to clone>
→ $ git clone ../remote_repo.git (url)

1. Viewing information about The remote repository
   → $ git remote -v
   (list the information about remote repository)

→ $ git branch -a

2. Pushing Changes
   Commit Changes Like we did previously
   → $ git diff
   ( Show difference between working directory and last commit.)

→ $git status
→ $git add -A
→ $ git commit -m “message” 3. Then push
→ $ git pull origin master
( Fetch the specified remote’s copy of current branch and immediately merge it into the local copy.)

→ $ git push origin master
( Push the branch to <remote>, along with necessary commits and objects. Creates named branch in the remote repo if it doesn’t exist )

### Common Workflow

1. Create a Branch for desired feature
   → $ git branch <new branch name>
   ( List all of the branches in your repo. Add a <branch> argument to create a new branch with the name <branch>.

→ $ git checkout -b <branch name>
( Create and check out a new branch named <branch>. Drop the -b flag to checkout an existing branch )

→ $ git merge <branch>
( Merge <branch> into the current branch.)

1. After Commit Push branch to remote
   → $ git push -u origin < branch-name >
   → $ git branch -a

### Merge a branch

1. → git checkout master
   → git pull origin master
   ( Fetch the remote’s copy of current branch and rebases it into the local copy. )

→ git branch —merged
(List all of the branches in your repo, Add a < branch > argument to create a new branch with the name < branch >

→ git merge < branch >
( Merge <branch> into the current branch )

→ git push origin master
(Push the branch to <remote>, along with necessary commits and objects. Creates named branch in the remote repo if it doesn’t exist.)

### Deleting a branch

1. → $ git branch —merged
   → $ git branch -d < branch >
   → $ git branch -a
   → $ git push origin - delete <branch>
