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

        o - o       
    o <        > o => `git merge`      
        o - o 

    o - o - o - o  => `git rebase`
       

`git rebase <branchname>` => Adds current branch on top of branch.
> A merge preserve history but never lies, rebases refactor history.      

###### git tags
>A pointer to a commit. 
`git tag <name>` => A light weight tag that points to a commit.     
`git tag <name> -a -m <message>` => Annotated tags, branch like.    
`git checkout <tag>`  => Goes to a specific tag.     
>Path : .git/refs/tags.     

###### Distributed version control      
>Path : packed-refs => Remote branches not in refs.   
`git push -f` => Ignore remotes and use local.      
`git fetch` => Get commit and related objects. 
`git pull` => fetch and merge.      
 
