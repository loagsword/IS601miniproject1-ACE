  # Merge Conflicts   
  Merge conflicts happen when you merge branches that have competing commits, and Git needs your help to decide which changes to incorporate in the final merge.
Git can often resolve differences between branches and merge them automatically. Usually, the changes are on different lines, or even in different files, which makes the merge simple for computers to understand. However, sometimes there are competing changes that Git can't resolve without your help. Often, merge conflicts happen when people make different changes to the same line of the same file, or when one person edits a file and another person deletes the same file.

 *How to create a merge conflict*   

Follow the below steps to create a merge conflict in your project. This is only for illustration purposes.  


1.	Make a new directory  named conflict on the repository   

  >$ mkdir conflict   
  >$ cd conflict


2.	Create a new file named my_conflict   

$ touch my_conflict.md  


3.	Add a line “creating a conflict” to my_conflict.md and Commit the new file to the repository    

      >$ git add my_conflict.md   
      >$ git commit -m ‘Task: creating my conflict file’   
      >$ git push origin master   

4.	Create and checkout a new branch  names new_branch from master   

     >$ git checkout -b new_branch   


5.	Add a line “ this better work” to my_conflict.md and Commit the changes in the new branch   
     
     >$ git add my_conflict.md   
     >$ git commit -m 'Task: updating my conflict file in new branch'   
     >$ git push origin master   

6.	Checkout the master    


      >$Git checkout master   


7.	Add a line “ update the conflict file” to my_conflict.md in the master branch and Commit the changes in the master   

       >$ git add my_conflict.md    
       >$ git commit -m ‘Task: updating my conflict file in master’    
       >$ git push origin master   


8.	 Merge the new branch to master   


        >$ git merge new_branch   

The above steps will produce a merge conflict, the terminal image below shows the error message

![](/images/conflict.JPG)   


