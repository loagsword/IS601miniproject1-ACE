# Forking vs Cloning   


Forking and cloning are Github features. A fork is a copy of a repository that allows you to freely experiment with changes without affecting the original project, while a clone allows you to create a local copy of the repository on your computer so that you can sync between both the local and remote locations of the project. A forked repository differs from a clone in that a connection exists between your fork and the original repository itself and you can contribute back to the original project using pull requests. Unlike forking, you won't be able to pull down changes from the original repository you cloned from, and if the project is owned by someone else you won't be able to contribute back to it unless you are specifically invited as a collaborator.   

* Forking a repository   

To create a fork for a project in GitHub, simply click the Fork button in the header of a repository. Once the process is complete, you'll be taken right to your forked copy of the project.    
1.	On GitHub, navigate to the repository.
2.	In the top-right corner of the page, click Fork.    


 * Cloning
 Step by step guide to clone a repository, go to the main page of the project to be cloned.
1.	On GitHub, navigate to the main page of the repository.
Note: If the repository is empty, you can manually copy the repository page's URL from your browser and skip to step four.
2.	Under the repository name, click Clone or download.     
 
3.	To clone the repository using HTTPS, under "Clone with HTTPS", click 
. To clone the repository using an SSH key, including a certificate issued by your organization's SSH certificate authority, click Use SSH, then click   

 
•  Open Git Bash.    
•  Change the current working directory to the location where you want the cloned directory to be made.   
•  Type git clone, and then paste the URL you copied in Step 2.    
$ git clone https://github.com/chisolum/IS601miniproject1-ACE  
•  Press Enter. Your local clone will be created.   
$ git clone https://github.com/chisolum/IS601miniproject1-ACE> Cloning into `Spoon-Knife`...   
> remote: Counting objects: 10, done.    
> remote: Compressing objects: 100% (8/8), done.    
> remove: Total 10 (delta 1), reused 10 (delta 1)    
> Unpacking objects: 100% (10/10), done.     


