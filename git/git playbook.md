# git playbook

## git faqs

1. [What is GIT?](#What is GIT?)
2. [What is ‘git add’?](#What is ‘git add’?)
3. [How do I rename a branch in Git?](#How do I rename a branch in Git?)


# What is GIT? 
GIT is a version control and source code management (SCM) system that is designed to handle both small and large projects quickly and efficiently.

# What is GIT version control? 
●GIT version control enables you to monitor the evolution of a group of files (code files).
●It allows for the creation of several versions of a file collection. Each version saves a snapshot of the files at a specific point in time, and the snapshot can be used to revert the collection of files. (The code can be developed in different versions of Java, and can be merged in Git)
●VCS permits switching between these versions. These versions are often maintained in a location known as a repository. (You can move between Java versions during the development process.)


# What is a Distributed Control System? 

Later, the code is sent from our local workstation to the central repository (GitHub). Working does not require a connection to a centralized repository.

# How to configure GitHub repository locally? 

# git config --global alias.lo "log --oneline" -----> To create an Alias to Command
# git config --global --unset alias.lo -----> To Remove an Alias
# git config --global --unset user.name -----> to remove username

# What is the git clone?

To download an existing repository from Centralized (Github) to local system. # git clone 

# What is ‘git add’?

To add files from work area to Index/staging/cache area. # git add  


# What is the use of ‘git log’? 

To see the commits by content or history, author

● git log -----> To show the Git Commits

● git log -5 -----> To show Recent 5 Commits

● git log --oneline -----> To Display the each commit in one line

● git log --since=2023-01-21

● git log --until=2023-01-01

● git log --author="user_name"

● git log --grep="Index"

● git log --oneline --author="user_name"

# How to edit an incorrect commit message in Git? Or How can you fix a broken

commit?

 git commit --amend -m "This is your new Git Message"

# How do you undo the last commit?
 
 git revert <your commit id>

# What is git reset?

Reset the current HEAD state to specific state.

# How to delete a Remote Branch? 

git push origin -d 

# How to see the difference between 2 branches

git diff <name of branch 1>..<name of branch 2>

# Why GIT better than Subversion (SVN)?

Git is an open-source version control system that allows you to perform a project's'version' command.

Each modification can be linked to a specific developer. Multiple developers can check out and post changes.

# What is git stash?

Stashing takes the Temporary stored state of your working directory.

# What is Git and how does it work?

Git is a version control system that tracks changes to files and directories. It allows multiple people to work on the same project simultaneously and keeps track of all changes made to the files.

# What is a Git repository?

A Git repository is a collection of files and directories that are tracked by Git. It is a place where all the changes to a project are stored and can be accessed by other users.

# What is a commit in Git?

A commit in Git is a snapshot of the current state of a project. It is a way of saving changes made to the files and directories in a Git repository.

# How do I create a new Git repository?
To create a new Git repository, you can use the command "git init" in the terminal or command prompt. This will initialize a new repository in the current directory.

# How do I clone a Git repository?
To clone a Git repository, you can use the command "git clone [repository URL]" in the terminal or command prompt. This will create a copy of the repository on your local machine.

# What is the difference between git pull and git fetch?

git pull is used to fetch changes from a remote repository and merge them into the current branch. git fetch is used to fetch changes from a remote repository, but it does not merge them into the current branch.

# How do I add a file to a Git repository?

To add a file to a Git repository, you can use the command "git add [file name]" in the terminal or command prompt. This will add the file to the repository and prepare it for a commit.

# How do I commit changes in Git?

To commit changes in Git, you can use the command "git commit -m [commit message]" in the terminal or command prompt. This will save the changes made to the files and directories in the repository.

 # How do I push changes to a remote repository?
 
 To push changes to a remote repository, you can use the command "git push [remote name] [branch name]" in the terminal or command prompt. This will send the changes made to the repository to the remote repository.

 # How do I create a new branch in Git?
To create a new branch in Git, you can use the command "git branch [branch name]" in the terminal or command prompt. This will create a new branch in the repository that can be used to make changes without affecting the master branch.
 
 # How do I switch between branches in Git?

To switch between branches in Git, you can use the command "git checkout [branch name]" in the terminal or command prompt. This will switch to the specified branch and make it the active branch.


# How do I merge branches in Git?
To merge branches in Git, you can use the command "git merge [branch name]" in the terminal or command prompt. This will combine the changes made to the specified branch with the current branch.

# How do I resolve conflicts in Git?

To resolve conflicts in Git, you can use the command "git mergetool" in the terminal or command prompt. This will open a tool that allows you to compare and resolve conflicts between different versions of a file.

# How do I view the history of a Git repository?

To view the history of a Git repository, you can use the command "git log" in the terminal or command prompt. This will show a list of all the commits made to the repository.

# How do I revert a commit in Git?

To revert a commit in Git, you can use the command "git revert [commit hash]" in the terminal or command prompt. This will undo the changes made in the specified commit and create a new commit to reflect the changes.

# How do I delete a branch in Git?

To delete a branch in Git, you can use the command "git branch -d [branch name]" in the terminal or command prompt. This will delete the specified branch from the repository.

# How do I stash changes in Git?

To stash changes in Git, you can use the command "git stash" in the terminal or command prompt. This will temporarily save changes made to the files and directories without committing them.

# How do I apply stashed changes in Git?

To apply stashed changes in Git, you can use the command "git stash apply" in the terminal or command prompt. This will apply the changes that were previously stashed.

# How do I create a tag in Git?

To create a tag in Git, you can use the command "git tag [tag name]" in the terminal or command prompt. This will create a new tag that can be used to mark a specific commit in the repository.

# How do I push a tag to a remote repository?

To push a tag to a remote repository, you can use the command "git push [remote name] [tag name]" in the terminal or command prompt. This will send the specified tag to the remote repository.

# How do I view the status of a Git repository?

To view the status of a Git repository, you can use the command "git status" in the terminal or command prompt. This will show the current state of the repository, including changes that have been made but not yet committed.

# How do I create a remote repository in Git?

To create a remote repository in Git, you can use a service like GitHub or GitLab. This will create a new repository on the remote server that can be accessed by other users.

# How do I add a remote repository in Git?

To add a remote repository in Git, you can use the command "git remote add [remote name] [repository URL]" in the terminal or command prompt. This will add the specified repository as a remote that can be accessed and pushed to.

# How do I remove a remote repository in Git?

To remove a remote repository in Git, you can use the command "git remote remove [remote name]" in the terminal or command prompt. This will remove the specified repository as a remote that can be accessed and pushed to.

# How do I configure Git?

To configure Git, you can use the command "git config" in the terminal or command prompt. This allows you to set various settings for your Git installation, such as your name and email.

# How do I check out a specific commit in Git?

To check out a specific commit in Git, you can use the command "git checkout [commit hash]" in the terminal or command prompt. This will change the current branch to reflect the state of the repository at the time of the specified commit.

# How do I create a patch file in Git? 

To create a patch file in Git, you can use the command "git format-patch [commit hash]" in the terminal or command prompt. This will create a file that contains the changes made in the specified commit.

# How do I resolve a merge conflict in Git?

To resolve a merge conflict in Git, you can use a text editor to manually edit the conflicting files and resolve any issues. Once the conflicts have been resolved, you can use the command "git add" to stage the changes, and "git commit" to finalize the merge.

# How do I view the commit history in Git?

To view the commit history in Git, you can use the command "git log" in the terminal or command prompt. This will display a list of all commits made to the repository, along with the commit message, author, and date.

# How do I view the difference between two commits in Git?

To view the difference between two commits in Git, you can use the command "git diff [commit hash 1] [commit hash 2]" in the terminal or command prompt. This will display the changes made between the two specified commits.

# How do I cherry-pick a commit in Git?

To cherry-pick a commit in Git, you can use the command "git cherry-pick [commit hash]" in the terminal or command prompt. This will apply the changes made in the specified commit to the current branch.

# How do I rebase a branch in Git?

To rebase a branch in Git, you can use the command "git rebase [branch name]" in the terminal or command prompt. This will reapply the commits made on the current branch onto the specified branch.

# How do I merge a branch in Git?

To merge a branch in Git, you can use the command "git merge [branch name]" in the terminal or command prompt. This will combine the changes made on the specified branch with the current branch.

# How do I squash commits in Git?

To squash commits in Git, you can use the command "git rebase -i [commit hash]" in the terminal or command prompt. This will open an editor where you can specify which commits to squash together.

# How do I rename a branch in Git?

To rename a branch in Git, you can use the command "git branch -m [old branch name] [new branch name]" in the terminal or command prompt. This will change the name of the specified branch.

# How do I view the branches in a Git repository?

To view the branches in a Git repository, you can use the command "git branch" in the terminal or command prompt. This will display a list of all branches in the repository.

# How do I view the remote branches in a Git repository?

To view the remote branches in a Git repository, you can use the command "git branch -r" in the terminal or command prompt. This will display a list of all remote branches in the repository.

# How do I view the current branch in Git?

To view the current branch in Git, you can use the command "git branch" in the terminal or command prompt. The current branch will be indicated with an asterisk (*) next to its name.

# How do I clone a repository in Git?

To clone a repository in Git, you can use the command "git clone [repository URL]" in the terminal or command prompt. This will create a copy of the specified repository on your local machine.
