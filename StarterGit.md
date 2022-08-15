
## Commonly used git commands

Knowing and understanding the git commands can be a boost to you. I have shared a list of common git commands and how you can use them. If you notice something missing be sure to add it. This list is not exhausive but I plan to keep adding to it. 

> Git is an open source distributed version control system.

`git init` => Creates a new git repository in the current folder.   
`git config --list` => Show the current git configuration in a list.  
`git help` =>Show a list of mostly used commands.   

`git remote add <name> <link>` => Add a remote repository to the local repository.

`git add <filename>` => adds the specified file to staging and creates an index for tracking.   
`git add .` => Adds all the file to staging for tracking.

`git status` => Shows the current state of Staged, Working Directory and committed files.   
`git status -s`/`git status --short` => Shows a status shorthand. A - Added, M - Modified, D - Deleted. 

`git commit -m <Commit message>` => Moves staged files to committed state.   
`git commit -a -m <Commit message>` => Stages all tracked files and commits them.     

`git rm --catched <filename>` => Stop tracking a file.    
`git push -u <remote> <branch>` => Push changes from local branch to remote.   
`git pull` => Pull changes from remote branch to local branch.    

File States: Working Directory > Staged > Committed.

`git diff --staged` => Shows the difference between ommitted vs staged files.   
`git diff` => Shows the difference between working directory vs staged files.    

`git switch <branch_name>` => Go to specified branch.
`git checkout <branch_name>` => Go to specific branch.    
`git checkout -b <branch_name>`  => Create a new branch and go to that branch     
`git merge <branch_name>` => Merge current branch with the specified branch.          

`git log` => Shows a log of the previous commits.    
`git log -<number>` => Shows the last defined number of commits.     
`git log --oneline` => Shows logs as a list of commits with less details.     
`git log --stat` => Shows a more detailed log statement.     
`git log --patch` => Show full difference by file.     

`git stash` => Saves working directory and index.    
`git stash list` => Shows the list of stashed items.     
`git stash show` =>     
`git stash pop` => Unstashes the last in the stack".     

`git reset --soft` => Moves commits back to staging.     
`git reset` / `git reset --mixed` => Move commits back to finacle.     
`git reset --hard` => Deletes changes.