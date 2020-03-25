Git commands
============
___

_A list of the most used Git commands_

### Obtaining & Creating Projects

| Command | Description |
| ------- | --------- |
| `git init` | Initializes a local Git repository |
| `git clone ssh: //git@github.com/ [user] / [repository-name] .git` | Creates a local copy of a remote repository |

### Basic

| Command | Description |
| ------- | --------- |
| git status | Check the status |
| `git add [filename-file.txt]` | Adds a file to the stage area |
| `git add -A` | Adds all new or modified files to the stage area |
| `git commit -m" [Commit message] "` | Commit the changes |
| `git rm -r [filename-file.txt]` | Removes a file (or folder) |

### Branching & Merging

| Command | Description |
| ------- | --------- |
| git branch | Lists the branches (the asterisk denotes the current branch) |
| `git branch -a` | List all branches (local and remote) |
| `git branch [name of branch]` | Create a new branch |
| `git branch -d [branch name]` | Delete a branch |
| `git push origin --delete [name of branch]` | Delete a remote branch |
| `git checkout -b [branch name]` | Create a new branch and switch to it |
| `git checkout -b [branch name] origin / [branch name]` | Clone a remote branch and switch to it |
| `git checkout [branch name]` | Select a branch |
| `git checkout -` | Switch to the last branch |
| `git checkout - [filename-file.txt]` | Discards modifications to a file |
| `git merge [name of branch]` | Merge a branch into the current branch |
| `git merge [source branch] [target branch]` | Merge one branch into another branch |
| git stash | Get the dirty state out of your working directory |
| git stash clear | Removes all 'stash' entries |

### Sharing & Updating Projects

| Command | Description |
| ------- | --------- |
| `git push origin [branch name]` | Submit a branch to your remote repository |
| `git push -u origin [branch name]` | Send changes from the reported branch to a remote repository (and select the branch) |
| git push | Send changes to the remote repository (current branch) |
| `git push origin --delete [name of branch]` | Deleting a remote branch |
| git pull | Updates the local repository to the last commit |
| `git pull origin [branch name]` | Receive changes from the remote repository |
| `git remote add origin ssh: //git@github.com/ [user] / [repository-name] .git` | Add a remote repository |
| `git remote set-url origin ssh: //git@github.com/ [user] / [repository-name] .git` | Set a repository from the origin branch to SSH |

### Inspection & Comparison

| Command | Description |
| ------- | --------- |
| git log | View changes |
| `git log --summary` | See changes (detailed) |
| `git diff [original branch] [target branch]` | Preview changes before merging |

