
# Resolving Merge Conflicts   
You must resolve all merge conflicts before you can merge a pull request on GitHub. If you have a merge conflict between the compare branch and base branch in your pull request, you can view a list of the files with conflicting changes above the Merge pull request button. The Merge pull request button is deactivated until you've resolved all conflicts between the compare branch and base branch.   

To resolve a merge conflict, you must manually edit the conflicted file to select the changes that you want to keep in the final merge. There are a couple of different ways to resolve a merge conflict:  

* You can resolve conflict on GitHub using the conflict editor. follow the below steps to resolve conflicts on GitHub   

![Resolving a merge conflict on GitHub](/https://help.github.com/en/articles/resolving-a-merge-conflict-on-github)   

* you can also resolve conflicts from the command line. See below..   
1. Manually remove the conflicting line in my_conflict.md in the new_branch and Commit the changes     

    >$ git checkout new_branch  
    >$ git add my_conflict.md   
    >$ git commit -m ‘Task: removing conflict file in new_branch’   
    >$ git push origin master


2.	 Merge the new branch to master   
     >$ git merge new_branch   

 Below terminal ouput shows the resut of the merge

 ![](/images/merge.JPG)




