#ProGit Chapters Summaries

##Chapter 2: Git Basics


###Getting a Git Repository

**git init** This creates a new subdirectory named .git that contains all of your necessary repository files. At this point, nothing in your project is tracked yet.

**git add** Add a file to the staging area. Use it insted of full path to add al changes file from current directory down into directory tree. 

**git commit** Create new commit from changes added to the staging area. Confirms changes to files and uploads them as a new version.

**git clone** Use it in case you want to get a copy of an existing Git repository.


###Recording Changes to the Repository

**git status** See the status of ypur work. New, staged, modified files. Current branch.

**gitingnore** You can create a file listing patterns to match the unnecesary files. To ignore them.

**git diff** It is to know exactly what you changed, not just which files were changed.

**git rm** Removez a file from Git. It removes it from your tracked files and then commit.

**git mv** it is used when you want to rename a file in Git.



###Viewing the Commit History

**git log** In case you want to look back to see what has happened after you have created several commits, or if you have cloned a repository with an existing commit history.

**git log -p** shows the difference (the patch output) introduced in each commit. You can also limit the number of log entries displayed, such as using -2 to show only the last two entries.


###Undoing Things

**git commit --amend** It is if you want to redo that commit, make the additional changes you forgot, stage them, and commit again.

**git reset** Get the file back from staging area to working directory.

**git checkout** Disard changes in working directory. This operation is unrecoverable.


###Working with Remotes

**git remote** To see which remote servers you have configured.

**git fetch pb** You can use the string pb on the command line if you want to fetch all the information that everyone have but that you don’t yet have in your repository.

**git remote show <remote>** If you want to see more information about a particular remote.

**git remote rename** To change a remote’s shortname.

**git push** The command doesn’t transfer tags to remote servers.



###Tagging

**git tag** This command lists the tags in alphabetical order; the order in which they are displayed has no real importance.

**git show** You can see the tag data along with the commit that was tagged.

**git tag -d <tagname>** To delete a tag on your local repository.



###Git Aliases

**git config** If you don’t want to type the entire text of each of the Git commands, you can easily set up an alias for each command using it.



##Chapter 3: Git Branching

###Branches in a Nutshell

**blobs** Staging the files computes a checksum for each one, stores that version of the file in the Git repository.

**master** It is The default branch name in Git. As you start making commits, you’re given a master branch that points to the last commit you made.

**git branch** To create a new branch.

**HEAD** to know what branch you’re currently on.

**git log** command that shows you where the branch pointers are pointing

**git checkout** To switch to an existing branch.

**git log --oneline --decorate --graph --all** it will print out the history of your commits.



###Basic Branching and Merging

**git merge** To make sure the nnew banch is what you want, and finally merge the branch back into your master branch to deploy to production.

**git mergetool** helps to solve issues with graphical tools.



###Branch Management

**git branch** Does more than just create and delete branches. If you run it with no arguments, you get a simple listing of your current branches.

** *master** The * character that prefixes the master branch: it indicates the branch that you currently have checked out.

**git branch -v** To see the last commit on each branch.

**--merged and --no-merged** They can filter this list to branches that you have or have not yet merged into the branch you’re currently on.

**git branch --merged** To see which branches are already merged into the branch you’re on.

**git branch --no-merged** To see all the branches that contain work you haven’t yet merged in.



###Branching Workflows

**develop or next** They work from or use to test stability.



###Remote Branches

**git ls-remote <remote>** You can get a full list of remote references explicitly for remote branches as well as more information.
**git remote show <remote>** You can get a full list of remote references explicitly for remote branches as well as more information.
