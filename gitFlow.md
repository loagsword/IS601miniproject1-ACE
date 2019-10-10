# About gitFlow

## First what is Git flow and gitFlow Workflow? 
GitHub flow is a lightweight, branch-based workflow that supports teams and projects where deployments are made regularly. _*GitFlow*_ is a branching model created by Vincent Driessen that allows developers to develop in parallel, by isolating new development from finished work. 
To accomplish this, the project development structure is divided into five different classes of git branches: Feature branches, the develop branch, release branches, hotfixes, and the master. In the workflow, new development (e.g new features & non-emergency bug fixes) are built in the *feature branches*. Feature branches are branched off of the *develop branch*, and finished features and fixes are merged back into the develop branch when they’re ready for release. When it is time to make a release, a release branch is created off of develop and then revised and tested until it is ready for deployment. When the release is finished, the release branch is merged into master and also into develop too. This is to make sure that all changes made in the release branch are reflected in both the master branch and development branch.. 
[insert image here]
![Gitflow workflow](~/images/gitflow.png)


## Repositories
A git repository is a collection of the files and folders within a project, along with the version and change history of each file. To initialize a repository or to convert an existing unversioned project directory into a Git repository, the  `git init` command can be used. Executing `git init` creates a .git subdirectory in the current working directory, which will contain all the necessary Git metadata to track the new repository.

```
git init
```

## Git Clone
`git clone` is used to create a copy of an existing local or remote repository to a local directory. It is useful for developers looking to have a working copy of a repository which can be edited separately from the main repository. The version controls of the clone are managed on the local repository.
Example, 
```
git clone [repository clone address]
```

## Git Fork
Creating a “fork” is producing a personal copy of someone else’s project. Forks act as a bridge between the original repository and your personal copy. You can submit Pull Requests to help make other people’s projects better by offering your changes up to the original project. To fork a repository on GitHub, click the Fork button in the header of the repository. 
![Git fork example](../images/gitfork.png)
 
## Git Branching
Branching is the creation of a development environment separate from the main line of development. It is ideal for trying out new ideas and to do work without messing with the main line. Changes made on a branch can later be merged with the master if, when, or after it is ready to be published or reviewed by a collaborator.
Example
```
git branch newBranch
$ git checkout newBranch
```
The above command creates a new branch called newBranch and then checks out the created branch. This set of commands can also be achieved using `git checkout -b iss53`

## Git Commit
A `git commit` functions like taking a snapshot.  It saves the snapshot to the project history and completes the change-tracking process. Anything that has been staged with a `git add’ will become a part of the snapshot with `git commit`. When committing, use the `-m` option to add a description for the commit.
Example:
```
git commit -m ‘added a new commit’
```

## Git Merge
`git merge` merges the lines of development together. This command is typically used to combine changes made on two distinct branches. For example, a developer would merge when they want to combine changes from a feature branch into the master branch for deployment.
Example:
```
git merge branch1 branch2 
```

## Git Checkout
`git checkout` navigates between the branches created by git branch. Checking out a branch updates the files in the working directory to match the version stored in that branch, and it tells Git to record all new commits on that branch.

## Git Push
`git push`  is used for updating the remote repository with any commits that have been made locally to a branch.
Example:
```
git push origin master
```

## Git Pull
The `git pull` command updates the local line of development with updates from its remote counterpart. This command is useful if a teammate has made commits to a branch on a remote, and they would like to reflect those changes in their local environment. 
Example:
```
git pull
```


## Git Status   
The `git status` command displays the status of the working tree. It shows the which changes have been staged and which files are untracked. The command is useful in checking what's going on with git add and git commit.   

Example   

 >$ git status   


 ![](/images/status.JPG)  

## Git Master Branch
The git master branch is the repository's default branch. After cloning(downloading) a project from a remote server, the resulting local repository has a single local branch: the so-called "master" branch. master branch is the main working branch of a repository.  


