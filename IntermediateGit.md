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
 
###### branches
`git -m <currentname> <newname>` | `git -m <newname>`  => Renames branch | renames current branch      
`git -d <branchname>` | `git -D <branchname>` => Delete branch | force delete branch      

###### merging
>Target branch => To merge to, Source branch => To merge from.       
`git merge <sourcebranch>`  => Merge.    
`git show <hash> ` => shows the files.
file marker (---), file marker (+++), dev/null for new or deleted files, @@ markers for chunk headers.      
<<<<<<HEAD (current branch) ====== (separate the two)  merge branch >>>>>>>>Main       
`git merge --abort` => Stop merge.     
{Evil commit} => Code added as part of a merge.        

###### git diff
`git diff` | `git diff -w` | `git diff <commit>` | `git diff <branch1> <branch2>` | `git diff <commit> <commit>` => Changed and not staged for commit. | Ignore whitespaces          
`git diff --cached` | `git diff --cached <commit>` =>  Staged changes | staged changes for a commit.     
`git diff HEAD` => All changes       

###### gitignore
Link to documentation [Gitignore] (https://github.com/github/gitignore)    
>Uses regular expressions.    

##### git rebase
`git rebase` => Clean up local history.     
`git merge -base <source> <destination>`  =>      
`git rebase -i <sha>` =>     
pick, squash, ....     
`git rebase <branch>` =>     
`git reflog ` =>      
`git pull --rebase` => pull when remote is rebased. 

##### git cherry pick
>Can be used to pick a bugfix across versions.      
`git cherry-pick <commit-sha>` => appends commit.    


