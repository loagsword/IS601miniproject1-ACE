# Git Branching
Git branching is a version control feature that allows you to make changes to your project without breaking your working code. Git branching feature is more important for collaboration projects, it allows you to verify changes made to the project and select which to add to the project.   

## Creating a Branch

 	$ git -b newbranch 
Adds a branch called `newbranch`.

	$ git checkout -b newbranch 
Adds a branch  `newbranch` and checks it out.
    
	      >$ git status   
Use to verify that you are on the new branch you just created.

## Deleting a Branch 

	$ git branch -d newbranch # 
Deletes the local branch, only if you have already pushed and merged it with your remote branches.

	$ git branch -D newbranch # 
Deletes the branch regardless of its push and merge status.
**NOTE:** The `-d` option is an alias for `--delete`. 
The `-D` option is an alias for `--delete --force`.

## Deleting a Remote Branch
	$ git push <remote_name> --delete <branch_name> 
Deletes a remote branch.

	$ git push <remote_name> :<branch_name>  
Also deletes a remote branch.
**NOTE:** These options can also be used to delete a “tag”.

RESOURCES:
1. [Create and manage git branches](https://github.com/Kunena/Kunena-Forum/wiki/Create-a-new-branch-with-git-and-manage-branches)
2. [More on git management](https://git-scm.com/book/en/v2/Git-Branching-Branch-Management)
