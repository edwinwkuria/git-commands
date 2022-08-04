
## Commonly used git commands

Knowing and understanding the git commands can be a boost to you. I have shared a list of common git commands and how you can use them. If you notice something missing be sure to add it. This list is not exhausive but I plan to keep adding to it. 

> Git is an open source distributed version control system.

`git init` => Creates a new git repository in the current folder.

`git add <filename>` => adds the specified file to staging and creates an index for tracking.
`git add .` => Adds all the file to staging for tracking.

`git status` =>Shows the current state of Staged, Working Directory and committed files.
`git status -s`/`git status --short` =>Shows a status shorthand. A - Added, M - Modified, D - Deleted. 

`git commit -m <Commit message>` => Moves staged files to committed state.
`git commit -a -m <Commit message>` => Stages all tracked files and commits them.