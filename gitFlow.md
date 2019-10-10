# About gitFlow


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






