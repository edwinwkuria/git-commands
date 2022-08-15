##### Intermediate Git. 
`git add <folder name>/` =>Adds a folder to git tracking.    
`echo "string"` `git hash-object -stdin` generates a SHA1 hash like the one used in git.     
`git branch -m main` => renames master branch to main.     
`git cat-file <hash>` => displays content of a hash/commit in git.     
*Options: `-p` peek ,  `-t` type, `-p` print (at the end).*       
`git count-objects` => Counts the number of objects.      
*Object types {Blobs, Trees, Commits, Tags}*        

>Branch => reference to a commit.      
*found in .git/refs/<branchname>*     
**Current branch is found in HEAD file**      
`git checkout <commit>/<tag>` => Switches to a commit or tag.      
`git merge` => Normal commit with two parents.      
*Fast-forward => reuse an existing commit.*          
   
###### git rebase
>rebases the commit to look like a single branch.