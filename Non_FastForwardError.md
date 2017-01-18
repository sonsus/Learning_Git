##Dealing with non-fast-forward errors

######Errormessage

````git
To https://github.com/USERNAME/REPOSITORY.git
 ! [rejected]        master -> master (non-fast-forward)
error: failed to push some refs to 'https://github.com/USERNAME/REPOSITORY.git'
To prevent you from losing history, non-fast-forward updates were rejected
Merge the remote changes (e.g. 'git pull') before pushing again.  See the
'Note about fast-forwards' section of 'git push --help' for details.
````

######check remote first just in case
````git
git remote -v   // check remote repo  
git remote rm origin(or remote name) 
git remote add origin (remote address) // add new remote
`````

#####Key
````git
git pull origin master(or current branch name)
or 
git fetch origin

git status
git add (updated !! even for deleted)
git commit -m "(commit message)"
git push -u (current branch) origin

````